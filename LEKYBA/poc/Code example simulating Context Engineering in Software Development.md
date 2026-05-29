---
tags:
  - proof_of_concept
---

<h1 style="color: blue">File name: rag_embedding_poc.py</h1>

```
import google.generativeai as genai
import numpy as np

# 1. Cấu hình API
# LƯU Ý BẢO MẬT: Trong dự án thực tế, KHÔNG BAO GIỜ hardcode API Key như thế này nhé, hãy dùng file .env!
genai.configure(api_key="Google studio API Key")
chat_model = genai.GenerativeModel('gemini-2.5-flash')

def vectorize(text): 
    result = genai.embed_content(
        model="models/gemini-embedding-001", # Model chuyên tạo Vector của Google
        content=text,
        task_type="retrieval_document"
    )
    return result['embedding']

#  Chương trình chính
company_knowledge_base = [
    "Công ty cho phép nhân viên làm việc remote (từ xa) tối đa 2 ngày/tuần.",
    "Quy định nghỉ phép: Nhân viên chính thức được 12 ngày phép năm. Hết năm không dùng sẽ bị hủy, không cộng dồn.",
    "Trợ cấp ăn trưa là 50.000 VNĐ/ngày, thanh toán vào kỳ lương cuối tháng."
]

print("⚙️ Đang vector hóa Database...")
db_vectors = [vectorize(chunk) for chunk in company_knowledge_base]

user_question = input("\nNhập câu hỏi: ")

print("🔍 Hệ thống đang tính toán độ tương đồng ngữ nghĩa (Cosine Similarity)...")
query_vector = vectorize(user_question)

# Tính Dot Product (Tích vô hướng) - Do vector của Gemini đã chuẩn hóa, Dot Product chính là Cosine Similarity
similarities = [np.dot(query_vector, doc_vector) for doc_vector in db_vectors]

# Tìm ra đoạn text có điểm tương đồng cao nhất
best_match_index = np.argmax(similarities)
highest_score = similarities[best_match_index]

# Đặt một ngưỡng (Threshold) để chống ảo giác: Nếu điểm quá thấp tức là không có text nào liên quan
THRESHOLD = 0.65 

if highest_score >= THRESHOLD:
    relevant_context = company_knowledge_base[best_match_index]
    print(f"🎯 Điểm tương đồng: {highest_score:.2f}")
else:
    relevant_context = "Không tìm thấy thông tin trong hệ thống."
    print(f"⚠️ Điểm tương đồng cao nhất chỉ đạt {highest_score:.2f} (Dưới ngưỡng cho phép).")

print(f"📦 Context lôi ra được: '{relevant_context}'\n")

# --- BƯỚC 5 & 6 GIỮ NGUYÊN NHƯ CŨ ---
engineered_prompt = f"""
Bạn là một trợ lý nhân sự tận tâm của công ty. Hãy trả lời câu hỏi của nhân viên DỰA VÀO ngữ cảnh nội bộ được cung cấp dưới đây. 

QUY TẮC CỨNG: 
1. Nếu ngữ cảnh chứa "Không tìm thấy thông tin", hãy trả lời: "Xin lỗi, tôi chưa được cung cấp thông tin về quy định này." Tuyệt đối không bịa đặt (No hallucination).
2. Trả lời ngắn gọn, lịch sự.

[NGỮ CẢNH NỘI BỘ]:
{relevant_context}

[CÂU HỎI TỪ NHÂN VIÊN]:
{user_question}
"""

print("🤖 AI đang phân tích Context và trả lời...")
response = chat_model.generate_content(engineered_prompt)
print(f"✅ Trả lời: {response.text}")
```