# Datathon_2026_VinUni

Dự án Khoa học Dữ liệu (Data Science) hoàn chỉnh bao gồm tiền xử lý dữ liệu, phân tích khám phá dữ liệu (EDA) và huấn luyện các mô hình học máy (Machine Learning) cho cuộc thi Datathon 2026.

## Cấu trúc thư mục

Dự án được tổ chức thành các thư mục chính như sau:

```text
DATATHON_2026_VINUNI/
│
├── EDA/                        # Thư mục chứa các Notebook Phân tích Khám phá Dữ liệu
│   ├── DataVisualization_V1.ipynb     
│   ├── DataVisualization_V2.ipynb         
│   ├── DataVisualization_V3.ipynb 
|   ├── DataVisualization_V4.ipynb 
│
├── MultipleChoice/             # Thư mục xử lý các tác vụ trắc nghiệm/dữ liệu phân loại
│   └── multiple-choice.ipynb   # Notebook xử lý phần thi multiple choice
│
├── TrainModel/                 # Thư mục chứa quá trình xây dựng và huấn luyện mô hình
│   └── TrainModelFinal.ipynb   # Notebook huấn luyện mô hình cuối cùng
│
├── Submission/                 # Thư mục chứa kết quả dự đoán để nộp bài
│   └── submission (22).csv     # File kết quả cuối cùng
│
├── .gitignore                  # File cấu hình bỏ qua các file không cần thiết.
├── LICENSE                     # Giấy phép mã nguồn mở của dự án
└── README.md                   # File tài liệu hướng dẫn.
```

## Hướng dẫn chạy lại kết quả (Reproduce Results)

Để tạo ra file kết quả dự đoán cuối cùng dùng để nộp bài, bạn **chỉ cần chạy notebook huấn luyện mô hình chính**.

### 1. Huấn luyện mô hình và tạo Submission
* Đi tới thư mục `TrainModel/`.
* Mở file **`TrainModelFinal.ipynb`** và chạy toàn bộ các cell (`Run All`).
* Quá trình này sẽ tự động thực hiện các bước cần thiết: tải dữ liệu, tiền xử lý, huấn luyện mô hình và dự đoán trên tập test.
### 2. Lấy kết quả nộp bài
* Sau khi code trong `TrainModelFinal.ipynb` chạy xong hoàn tất, file dự đoán sẽ được tự động xuất ra.
* Truy cập vào thư mục và tìm file `submission.csv` là file kết quả.
### 3. Lưu ý
* **Tất cả code load file đều sử dụng đường dẫn dataset trên kaggle.**
* **`EDA/`**: Chứa các notebook dùng để trực quan hóa, phân tích phân phối dữ liệu và tìm ra các insight trong cuộc thi. Bạn có thể mở đọc để hiểu rõ hơn về cách nhóm tiếp cận dữ liệu, **không cần thiết phải chạy lại** để ra file submission.
* **`MultipleChoice/`**: Xử lý phần thi trắc nghiệm.
