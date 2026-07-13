# Diabetes Risk Prediction & Analysis

Dự án phân tích dữ liệu sức khỏe cộng đồng và xây dựng mô hình học máy nhằm dự báo các yếu tố nguy cơ dẫn đến bệnh tiểu đường (Diabetes Mellitus), tập trung vào việc giải quyết bài toán dữ liệu mất cân bằng trong y học dự phòng

## 🛠 Tech Stack
* **Ngôn ngữ:** R
* **Thư viện chính:** `tidyverse`, `ggplot2`, `janitor`
* **Thuật toán ML:** XGBoost, Multinomial Logistic Regression (MLR), Linear Discriminant Analysis (LDA)
* **Kỹ thuật xử lý:** SMOTE, Undersampling, Winsorization, VIF Analysis

## 🚀 Các giai đoạn chính

* **Tiền xử lý và làm sạch dữ liệu:** Kiểm soát giá trị ngoại lệ (outliers) bằng kỹ thuật Winsorization, thực hiện chuẩn hóa dữ liệu và xử lý vấn đề mất cân bằng lớp (Class Imbalance) nhằm đảm bảo chất lượng đầu vào cho mô hình.
* **Phân tích thống kê & Kiểm định giả thuyết:** Sử dụng thống kê mô tả và các kiểm định phi tham số (Chi-square cho biến định danh, Kruskal-Wallis cho biến thứ bậc và liên tục) để xác định mức độ ảnh hưởng của các nhân tố lâm sàng đối với tình trạng bệnh
* **Xây dựng & Đánh giá mô hình dự báo:** Triển khai đa mô hình, tối ưu hóa khả năng nhận diện các nhóm nguy cơ cao (Prediabetes và Diabetes) thông qua chiến lược *Balanced Prior* và phân tích tương tác giữa các biến số.
* **Tổng kết & Thảo luận:** Đánh giá hiệu năng mô hình dựa trên các chỉ số y sinh quan trọng (Sensitivity, ROC, AUC), từ đó rút ra kết luận về các yếu tố nguy cơ hàng đầu (BMI, GenHlth) và đề xuất hướng can thiệp sớm

## 📊 Kết quả nổi bật
* **Xử lý dữ liệu:** Nâng cao khả năng phát hiện lớp thiểu số (Prediabetes) từ 0% lên 45.3% thông qua các kỹ thuật lấy mẫu hybrid (SMOTE + Undersampling)
* **Hiệu suất mô hình:** Đạt chỉ số ROC-AUC > 0.82 cho mô hình phân loại tiểu đường, đáp ứng tốt yêu cầu về sàng lọc y tế

---
