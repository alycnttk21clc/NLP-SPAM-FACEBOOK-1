# 🛡️ Sử dụng mô hình học máy Naive Bayes để nhận diện spam quảng cáo trong bình luận Facebook

## 📌 Giới thiệu
Dự án này áp dụng **Machine Learning (Naive Bayes)** để tự động phân loại bình luận trên Facebook thành **SPAM** (quảng cáo, lừa đảo) hoặc **HAM** (bình thường).  
Mục tiêu là hỗ trợ quản lý bình luận, loại bỏ các nội dung rác nhằm nâng cao chất lượng tương tác trên mạng xã hội.

## 🏗️ Kiến trúc & Phương pháp
- **Xử lý dữ liệu**: Làm sạch văn bản (loại bỏ ký tự đặc biệt, chuẩn hoá Unicode).
- **Biểu diễn văn bản**: Sử dụng **TF-IDF Vectorizer**.
- **Xử lý mất cân bằng**: Dùng **RandomOverSampler** để cân bằng số lượng mẫu.
- **Mô hình**: Áp dụng **Multinomial Naive Bayes** để phân loại.
- **Đánh giá mô hình**: Sử dụng Accuracy, F1-score, ROC Curve, Precision-Recall Curve.

## 📂 Cấu trúc dự án
- `spam_detector_colab.ipynb` – Notebook chính: tiền xử lý, huấn luyện, đánh giá mô hình.
- `facebook_captions_comments_spam_dataset.csv` – Bộ dữ liệu gồm các caption & comment Facebook đã gán nhãn.
- `README.md` – Tài liệu mô tả dự án.

## 🚀 Cách chạy
Bạn có thể mở trực tiếp project trên Google Colab bằng nút dưới đây:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DcCf-HXAy9nYfbYqI13CK8pFWC7FMN8z?authuser=0#scrollTo=-kXvsxk_gXrj)

Hoặc clone repo về máy và chạy:
```bash
git clone https://github.com/<your-username>/NLP-SPAM-FACEBOOK.git
cd NLP-SPAM-FACEBOOK
jupyter notebook spam_detector_colab.ipynb
