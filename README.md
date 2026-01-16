# salary_prediction_system
# Tổng quan dự án

## 1. Mục tiêu

Dự án nhằm xây dựng một pipeline Machine Learning hoàn chỉnh cho bài toán phân tích và dự đoán Lương ngành CNTT tại Việt Nam, bao gồm các bước: thu thập dữ liệu, khám phá dữ liệu, tiền xử lý, huấn luyện mô hình, đánh giá, kiểm định thống kê và lưu trữ mô hình.

---

## 2. Cấu trúc thư mục

Cài đặt thư viện cần thiết:
```
pip install -r requirements.txt
```

```text
project-root/
│
├── data/                   # Lưu bộ dữ liệu gốc và dữ liệu đã xử lý
│   ├── raw/                # Dữ liệu thô ban đầu
│   └── processed/          # Dữ liệu sau tiền xử lý
│
├── process/                # Quy trình xử lý và huấn luyện
│   ├── preprocess.py       # Khám phá dữ liệu (EDA) & tiền xử lý
│   └── machine_learning.py # Huấn luyện, fine-tune và đánh giá mô hình
│
├── pipeline/               # Lưu các mô hình ML đã huấn luyện
│   ├── model.pkl
│   └── scaler.pkl
│
└── requirements.txt        # Thư viện sử dụng
```

---

## 3. Một số kết quả

Kinh nghiệm làm việc và nhóm kỹ năng công nghệ là hai yếu tố có ảnh hưởng mạnh nhất đến mức lương IT tại Việt Nam.

Các kỹ năng chuyên sâu như Backend, Data, AI/ML thường gắn với mức lương cao hơn so với các kỹ năng phổ thông.

Yếu tố vị trí địa lý cho thấy sự chênh lệch rõ rệt, trong đó các thành phố lớn có mặt bằng lương cao hơn.

Mô hình học máy phi tuyến (đặc biệt là MLP) cho kết quả dự đoán tốt hơn các mô hình tuyến tính trong bối cảnh dữ liệu nhiều chiều.

Việc kiểm soát đa cộng tuyến và lựa chọn đặc trưng giúp mô hình ổn định hơn và giảm nguy cơ overfitting.