

# Comprehensive Guide to AI Configuration Files in a Codebase

This document details the purpose, usage, and differences between various AI configuration components in a software project (e.g., `agents.md`, Custom Agents, Skills, Prompts, Hooks, and Workflows).

---

## 1. Global Project Instructions (`agents.md` & `copilot-instructions.md`)

These are the root configuration files that provide a high-level overview of the entire project to the LLMs.

* **Origin:** Originated from Anthropic's `cloud.md`, now standardized to `agents.md` across multiple AI vendors (OpenAI, Anthropic, etc.).
* **`.github/copilot-instructions.md`:** Specific to GitHub Copilot. Required for the **Copilot Code Reviews** feature to work.
* **Configuration Tip:** Inside `copilot-instructions.md`, simply point the AI to `agents.md` to avoid duplicating information.

### 💡 Best Practices for `agents.md`
* **No Auto-generation:** Using the `/init` command to let an LLM write `agents.md` reduces the success rate by 3% and increases token costs by 20%. The AI will read the source code itself; do not duplicate the directory structure here.
* **Human-written:** Focus on three core elements: **What** (Tech stack), **Why** (Project purpose), and **How** (e.g., "Use `uv` instead of `pip`", or "Use `bun` instead of `npm`").
* **Mono-repos:** Create a separate `agents.md` for each directory or service (e.g., one for Frontend, one for Backend) alongside the global configuration file.

---

## 2. Custom Agents

Agents act as specialized "colleagues" (e.g., Dev Expert, React Frontend Engineer, DevOps).

* **Standard Team Model (Production Setup):**
  * **Orchestrator Agent:** Receives instructions. It does not code or plan; it solely delegates tasks.
  * **Planner Agent:** Receives instructions from the Orchestrator, creates a detailed plan, and returns it.
  * **Coder Agent:** Receives the finalized plan and writes the actual code.
* **Reason for Separation:** Keeps the Context Window of each AI clean and unpolluted, resulting in much more accurate output.
* **Agent Teams:** A newer architecture allowing sub-agents (Planner, Coder) to run in parallel and communicate directly with each other instead of strictly reporting to the Orchestrator.

---

## 3. Hooks (Lifecycle Triggers)

Hooks are automated scripts that execute at specific points within an AI session lifecycle (e.g., `session_start`, `session_end`).

* **How it works:** They run silently in the background *before* or *after* every prompt you make.
* **Real-world Examples:**
  * **Secret Scanner:** Automatically scans the codebase every time you interact with the AI to ensure no API Keys or Passwords are leaked.
  * **Governance Audit:** Checks your code against organizational standards.

---

## 4. Domain-Specific Instructions

These are Markdown files containing deep, specialized guidelines for a particular topic.

* **Examples:** `a11y-instructions.md` (for Accessibility standards) or `localization-instructions.md` (for multi-language support).
* **Crucial Note:** The AI will **NOT** automatically pick up these files. You MUST explicitly reference them inside your global `agents.md` (e.g., *"For accessibility-related topics, please refer to a11y-instructions.md"*).

---

## 5. Custom Prompts

Prompts (typically triggered via a `/` slash command) are predefined behavioral templates for repetitive, micro-level tasks.

* **Example:** Creating a custom `/explain` command.
* **Configuration:** You can enforce a rule that whenever `/explain` is called on a piece of code, the AI must respond in this exact format:
  1. Brief overview.
  2. Step-by-step breakdown.
  3. Explanation of core concepts.

---

## 6. Skills

Skills inject expert-level domain knowledge into the AI to help it execute complex workflows automatically.

* **Example:** The **Breakdown Plan** skill allows the AI to act as a Senior Project Manager. When you ask it to "Introduce a discount coupon feature", it uses this skill to break the feature down into Epics, User Stories, and Features following standard Agile methodologies.
* **Warning:** Skills process a massive amount of data and can quickly consume half of your Context Window. Install only the skills that are strictly necessary for your daily role.

---

## 7. Workflows (AI-driven CI/CD)

Workflows merge AI capabilities with CI/CD pipelines (such as GitHub Actions).

* **How it works:** They run on a schedule (cron job) rather than through direct user chat interaction.
* **Real-world Example:** A daily workflow where the AI automatically reads all open issues, tracks repository activity, and generates a new GitHub Issue summarizing the day's progress for the engineering team.