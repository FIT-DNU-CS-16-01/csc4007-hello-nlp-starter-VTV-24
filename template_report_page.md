# Lab0 — 1-page report (Hello NLP, random data)

## Pipeline đã chạy
- Sinh dữ liệu tiếng Việt giả lập (positive/negative) → TF-IDF (ngram 1–2) → Logistic Regression → train/test split (80/20) → đánh giá.

## Kết quả
- Accuracy = 1.0, Macro-F1 = 1.0; confusion matrix không có sai lệch (32/0, 0/28); vocab_size = 112.

## Vấn đề gặp phải + cách xử lý (ví dụ)
- Gặp lỗi OMP (libiomp5md.dll conflict) khi import torch → xử lý bằng cách thiết lập biến môi trường KMP_DUPLICATE_LIB_OK và cấu hình lại môi trường conda để tránh xung đột thư viện.

## Ghi chú
- Dữ liệu được sinh ngẫu nhiên nên mô hình đạt kết quả hoàn hảo, chỉ nhằm mục đích kiểm tra pipeline và môi trường, không phản ánh hiệu năng thực tế.