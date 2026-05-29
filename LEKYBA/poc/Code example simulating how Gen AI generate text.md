---
tags:
  - proof_of_concept
---

<h1 style="color: blue">File name: text_generator.py</h1>

```
# STEPs

# 1. Train

# Split a paragraph to an array of words

# 2. Build model

# Create an object (dictionary). Go through the array, with each word, store the word right after to an array.

# 3. Generate

# Choose a word to begin, look at the memory, choose a random word in array and repeat

  

import random

  

text_data = """

Tôi đi học lập trình.

Tôi đi làm ở công ty phần mềm.

Lập trình rất thú vị nhưng cũng rất khó.

Tôi thích học AI và làm hệ thống.

"""

  

def build_markov_model(text):

    words = text.split()

    model = {}

  

    for i in range(len(words) -1):

        current_word = words[i]

        next_word = words[i + 1]

  

        if current_word not in model:

            model[current_word] = []

  

        model[current_word].append(next_word)

  

    return model

  

def generate_text(model, start_word, length=10):

    current_word = start_word

    result = [current_word]

  

    for _ in range(length - 1):

        # Nếu từ hiện tại có trong từ điển, bốc random 1 từ tiếp theo

        if current_word in model:

            next_words = model[current_word]

            current_word = random.choice(next_words)

            result.append(current_word)

        else:

            break

  

    return ' '.join(result)

  

# --- THỰC THI ---

# Bước 1: Cho "AI" học dữ liệu

ai_model = build_markov_model(text_data)

print("Não bộ của AI (Markov Model):")

print(ai_model)

print("-" * 30)

  

# Bước 2: Bắt AI sinh tạo văn bản mới bắt đầu bằng chữ "Tôi"

print("Văn bản AI tự sinh ra:")

generated_sentence = generate_text(ai_model, start_word="Tôi", length=8)

print(generated_sentence)
```
