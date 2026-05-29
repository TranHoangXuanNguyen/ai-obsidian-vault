# Tổng quan và So sánh: Agent, Instruction và Skills trong Hệ sinh thái AI

Tài liệu này tổng hợp thông tin từ các tài liệu nghiên cứu trong thư mục `nguyen-raw`, giải thích về ba khái niệm cốt lõi: **Agent** (Tác nhân), **Instruction** (Chỉ dẫn) và **Skills** (Kỹ năng), cùng với sự so sánh chi tiết giữa chúng.

---

## 1. Agent (Tác nhân)

**Agent** là một cấu hình AI chuyên biệt đóng vai trò như một "đồng nghiệp" có chuyên môn cụ thể (ví dụ: Chuyên gia React, Kỹ sư DevOps, Trợ lý nghiên cứu).

*   **Đặc điểm:**
    *   Sở hữu một persona (cá tính/vai trò) nhất định.
    *   Có khả năng gọi các công cụ (tools) hoặc máy chủ MCP (Model Context Protocol).
    *   Thường hoạt động theo mô hình nhóm: **Orchestrator** (Điều phối), **Planner** (Lập kế hoạch) và **Coder** (Lập trình).
*   **Khi nào nên dùng:** Khi bạn có các quy trình công việc lặp đi lặp lại cần tích hợp sâu với công cụ, thực thi lệnh chủ động hoặc cần các rào cản bảo vệ (guardrails) xuyên suốt một phiên làm việc.

---

## 2. Instruction (Chỉ dẫn)

**Instruction** là các quy tắc và bối cảnh nền tảng mà AI sẽ đọc mỗi khi làm việc trên một tệp hoặc dự án (ví dụ: `agents.md`, `CLAUDE.md`, `.cursorrules`).

*   **Đặc điểm:**
    *   Cung cấp thông tin về Tech stack (Cái gì), Mục đích dự án (Tại sao) và Quy tắc thực thi (Làm thế nào).
    *   Có thể được phạm vi hóa theo toàn cục dự án, theo thư mục hoặc theo ngôn ngữ lập trình.
    *   Giúp giảm thời gian chạy (khoảng 28.6%) và lượng token tiêu thụ (khoảng 16.6%) nhờ việc cung cấp bối cảnh ngay từ đầu.
*   **Khi nào nên dùng:** Khi cần các quy chuẩn kỹ thuật lâu dài (coding standards), chiến lược kiểm thử hoặc các quyết định kiến trúc cần được áp dụng nhất quán.

---

## 3. Skills (Kỹ năng)

**Skills** là các gói khả năng có thể tái sử dụng, bao gồm các chỉ dẫn cụ thể, mã nguồn (scripts) và tài nguyên bổ trợ.

*   **Đặc điểm:**
    *   Được cấu trúc trong thư mục riêng với tệp `SKILL.md`.
    *   Có khả năng "tự khám phá": Agent có thể tự động tìm và tải Skill phù hợp với nhiệm vụ (thông qua siêu dữ liệu).
    *   Hỗ trợ "tiết lộ dần dần" (progressive disclosure): Chỉ tải thông tin chi tiết khi thực sự cần thiết để tiết kiệm Context Window.
*   **Khi nào nên dùng:** Khi muốn chuẩn hóa cách AI phản hồi một tác vụ cụ thể, cần các tài nguyên đi kèm (mẫu, lược đồ) hoặc muốn tạo ra các quy trình có thể di chuyển (portable) giữa các hệ thống AI khác nhau.

---

## 4. So sánh chi tiết

| Đặc tính | Agent | Instruction | Skills |
| :--- | :--- | :--- | :--- |
| **Vai trò** | Persona / Người điều phối | Lương tâm / Rào cản bảo vệ | Đôi tay / Công cụ thực thi |
| **Trạng thái** | Theo phiên làm việc | Luôn hoạt động (trong phạm vi) | Theo yêu cầu (On-demand) |
| **Nội dung** | Cấu hình + Công cụ | Văn bản quy tắc | Chỉ dẫn + Mã nguồn + Tài sản |
| **Cơ chế kích hoạt** | Do người dùng chọn/gán | Tự động khớp theo tệp/dự án | Agent tự khám phá hoặc gọi lệnh `/` |
| **Sự tương đương** | Đầu bếp chuyên nghiệp | Nội quy nhà hàng | Các thiết bị nhà bếp |

---

## 5. Cách chúng phối hợp với nhau

Sức mạnh thực sự nằm ở việc kết hợp cả ba lớp:
1.  **Instructions** tạo nền tảng với các rào cản và quy tắc dài hạn.
2.  **Skills** cho phép kích hoạt các quy trình giàu tài nguyên theo yêu cầu.
3.  **Agents** mang lại hành vi có tính định hướng cao nhất, đóng gói các công cụ và chỉ dẫn vào một thực thể có chuyên môn.

*Ví dụ:* Một **Agent** "DevOps" sẽ tuân thủ **Instruction** "luôn chạy test trước khi deploy" và sử dụng **Skill** "deploy-to-aws" để thực hiện công việc.
