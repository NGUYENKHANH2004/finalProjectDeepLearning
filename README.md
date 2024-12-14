# Deep Learning Final Project

Institute of Artificial Intelligence, University of Engineering and Technology, Vietnam National University.

Dự án tập trung vào phân loại ung thư da bằng cách sử dụng các mô hình học sâu.

**Thành viên nhóm 23:**
| Thành viên          | MSV       |
|---------------------|-----------|
| Nguyễn Trọng Khánh  | 22022603  |
| Lê Anh Tiến         | 22022528  |
| Thái Thị Thùy Linh  | 22022631  |
| Nguyễn Văn Trường   | 22022571  |
| Ngô Đức Hùng        | 22022652  |


## Tổng Quan Dự Án

Dự án này nhằm mục đích phát triển và đánh giá các mô hình học sâu để phân loại các tổn thương da từ hình ảnh soi da. Việc phát hiện sớm và chính xác ung thư da là rất quan trọng để điều trị hiệu quả và cải thiện kết quả cho bệnh nhân. Dự án này khám phá hiệu suất của một số kiến trúc mạng nơ-ron tích chập (CNN) trong việc phân loại các loại tổn thương da khác nhau.

## Dataset

Dataset sử dụng cho dự án này là [bộ dữ liệu HAM10000](https://www.kaggle.com/datasets/surajghuwalewala/ham1000-segmentation-and-classification). Bộ dữ liệu này bao gồm 10.015 hình ảnh soi da các tổn thương da có sắc tố, được phân loại thành 7 lớp:

*   Actinic keratoses và ung thư biểu mô nội biểu mô / bệnh Bowen (AKIEC)
*   Ung thư tế bào đáy (BCC)
*   Các tổn thương giống u sừng lành tính (BKL)
*   U xơ da (DF)
*   U hắc tố (MEL)
*   Nốt ruồi hắc tố (NV)
*   Tổn thương mạch máu (VASC)

## Models

1.  **Baseline CNN:** Một mạng nơ-ron tích chập đơn giản với một vài lớp để trích xuất đặc trưng cơ bản và phân loại.
2.  **ResNet-50:** Một mạng dư với 50 lớp, được biết đến với khả năng huấn luyện hiệu quả các mạng rất sâu.
3.  **DenseNet-121:** Một mạng kết nối dày đặc với 121 lớp, nhằm tối đa hóa dòng thông tin và tái sử dụng đặc trưng.
4. **ResNet-50 loại bỏ residual block**: Một mô hình ResNet50 loại bỏ cơ chế residual block được dùng trong thí nghiệm phụ.
