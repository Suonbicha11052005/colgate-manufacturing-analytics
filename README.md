# Colgate Manufacturing Analytics 📊

## Overview

Kho lưu trữ này chứa một giải pháp phân tích toàn diện cho **Colgate Manufacturing** tập trung vào tối ưu hóa hiệu suất nhà máy. Dự án kết hợp phân tích dữ liệu, trí tuệ kinh doanh và trực quan hóa dữ liệu tương tác.

**Team:** Sigma Seeker  
**Competition:** RBAC 2025 - Round 2

---

## 📁 Project Structure

```
colgate-manufacturing-analytics/
├── README.md                                    # File này
├── Data dictionary.xlsx                         # Từ điển dữ liệu hoàn chỉnh với định nghĩa trường
├── RBAC 2025 - Factory Performance.pbix         # Bảng điều khiển Power BI để phân tích hiệu suất nhà máy
├── [RBAC 2025] CASE STUDY ROUND 2.pdf          # Báo cáo trường hợp chi tiết và phân tích
├── [RBAC 2025] - Round 2 - Team Sigma Seeker.pdf # Bản trình bày nhóm và phát hiện
│
├── raw data/                                    # Dữ liệu gốc
│   ├── production_data.csv                      # Dữ liệu sản xuất hàng ngày
│   ├── equipment_logs.csv                       # Nhật ký hoạt động thiết bị
│   ├── quality_control.csv                      # Dữ liệu kiểm soát chất lượng
│   ├── factory_operations.csv                   # Dữ liệu hoạt động nhà máy
│   └── defect_records.csv                       # Ghi chép lỗi sản phẩm
│
├── cleaned data/                                # Dữ liệu đã xử lý và làm sạch
│   ├── production_cleaned.csv                   # Dữ liệu sản xuất đã làm sạch
│   ├── equipment_cleaned.csv                    # Dữ liệu thiết bị đã xử lý
│   ├── quality_cleaned.csv                      # Dữ liệu chất lượng đã xử lý
│   ├── merged_dataset.csv                       # Tập dữ liệu hợp nhất tất cả nguồn
│   └── quality_metrics.csv                      # Chỉ số chất lượng tính toán
│
└── notebooks/                                   # Sổ ghi chép Jupyter để phân tích
    ├── 01_EDA.ipynb                             # Phân tích dữ liệu khám phá
    ├── 02_Data_Cleaning.ipynb                   # Quy trình làm sạch dữ liệu
    ├── 03_Statistical_Analysis.ipynb            # Phân tích thống kê và kiểm định giả thuyết
    ├── 04_Performance_Metrics.ipynb              # Tính toán chỉ số hiệu suất
    └── 05_Visualization.ipynb                   # Tạo các biểu đồ và trực quan hóa
```

---

## 🎯 Project Objectives

Mục đích dự án bao gồm:
- Phân tích các chỉ số hiệu suất nhà máy trên nhiều chiều khác nhau
- Xác định các nút thắt hoạt động và cơ hội tối ưu hóa
- Phát triển các khuyến nghị dựa trên dữ liệu để cải thiện hiệu quả sản xuất
- Tạo các trực quan hóa tương tác cho việc ra quyết định của các bên liên quan
- Hỗ trợ lập kế hoạch chiến lược dựa trên bằng chứng thực nghiệm

---

## 📊 Key Deliverables

### 1. **Data Dictionary** (`Data dictionary.xlsx`)

Tài liệu toàn diện cho tất cả các trường dữ liệu, bao gồm:
- Tên trường và mô tả chi tiết
- Loại dữ liệu và định dạng
- Định nghĩa kinh doanh và bối cảnh
- Chỉ số chất lượng dữ liệu

### 2. **Power BI Dashboard** (`RBAC 2025 - Factory Performance.pbix`)

Bảng điều khiển tương tác với các tính năng:
- Các KPI hiệu suất nhà máy
- Chỉ số sản xuất thời gian thực
- Phân tích so sánh giữa các cơ sở
- Triển khai Kiểm soát truy cập dựa trên vai trò (RBAC)
- Khả năng khoan sâu để phân tích chi tiết

### 3. **Case Study Report** (`[RBAC 2025] CASE STUDY ROUND 2.pdf`)

Phân tích sâu bao gồm:
- Tuyên bố vấn đề và các câu hỏi nghiên cứu
- Phương pháp dữ liệu và cách tiếp cận
- Các phát hiện và insight chính
- Các khuyến nghị chiến lược

### 4. **Team Presentation** (`[RBAC 2025] - Round 2 - Team Sigma Seeker.pdf`)

Tóm tắt cấp quản lý bao gồm:
- Tổng quan dự án và mục tiêu
- Kết luận và phát hiện chính
- Lộ trình triển khai
- Các bước tiếp theo và cơ hội trong tương lai

---

## 🛠️ Technical Stack

- **Data Processing:** Python (Jupyter Notebooks)
- **Data Visualization:** Power BI
- **Data Analysis:** Phân tích thống kê và phân tích dữ liệu khám phá
- **Data Management:** Excel cho từ điển dữ liệu và tài liệu bổ sung

---

## 📈 Data Sources

### Raw Data (`raw data/`)

Chứa các tập dữ liệu gốc được trích xuất từ các hoạt động sản xuất:
- **production_data.csv** - Chỉ số sản xuất, thời gian làm việc, sản lượng hàng ngày
- **equipment_logs.csv** - Nhật ký hoạt động thiết bị, thời gian chạy, bảo trì định kỳ
- **quality_control.csv** - Dữ liệu kiểm soát chất lượng, tỷ lệ lỗi, tiêu chuẩn
- **factory_operations.csv** - Dữ liệu hoạt động nhà máy, ca làm việc, nhân sự
- **defect_records.csv** - Ghi chép chi tiết lỗi sản phẩm, loại lỗi, nguyên nhân gốc rễ

### Cleaned Data (`cleaned data/`)

Các tập dữ liệu đã xử lý sẵn sàng cho phân tích:
- **production_cleaned.csv** - Dữ liệu sản xuất đã được chuẩn hóa và xử lý giá trị thiếu
- **equipment_cleaned.csv** - Dữ liệu thiết bị đã loại bỏ ngoại lệ và chuẩn hóa
- **quality_cleaned.csv** - Dữ liệu chất lượng đã xử lý và xác thực
- **merged_dataset.csv** - Tập dữ liệu hợp nhất từ tất cả các nguồn
- **quality_metrics.csv** - Các chỉ số chất lượng được tính toán và dẫn xuất

---

## 🔍 Analysis Notebooks (`notebooks/`)

Các sổ ghi chép Jupyter chứa:

- **01_EDA.ipynb** - Phân tích dữ liệu khám phá, thống kê mô tả, trực quan hóa ban đầu
- **02_Data_Cleaning.ipynb** - Quy trình làm sạch dữ liệu, xử lý giá trị thiếu, xử lý ngoại lệ
- **03_Statistical_Analysis.ipynb** - Phân tích thống kê, kiểm định giả thuyết, tương quan
- **04_Performance_Metrics.ipynb** - Tính toán chỉ số hiệu suất chính, KPI, so sánh năng lực
- **05_Visualization.ipynb** - Tạo biểu đồ và trực quan hóa dữ liệu cho báo cáo

---

## 🎓 Key Insights

Phân tích giải quyết các thách thức sản xuất quan trọng:

1. **Performance Optimization**
   - Xác định các cơ sở hoạt động tốt và kém hiệu quả
   - So sánh với tiêu chuẩn ngành

2. **Operational Efficiency**
   - Phân tích nguyên nhân gốc rễ của trì hoãn sản xuất
   - Khuyến nghị phân bổ tài nguyên

3. **Quality Management**
   - Phân tích xu hướng chất lượng
   - Giám sát tỷ lệ lỗi sản phẩm

4. **Strategic Planning**
   - Dự báo dựa trên dữ liệu
   - Ưu tiên hóa đầu tư

---

## 💡 How to Use This Repository

### Cho Các Bên Liên Quan (Stakeholders):
1. Mở **Power BI Dashboard** (`RBAC 2025 - Factory Performance.pbix`) để khám phá tương tác
2. Xem lại **Team Presentation** PDF để có tóm tắt cấp quản lý
3. Tham khảo **Case Study Report** để phân tích chi tiết

### Cho Nhà Phân Tích Dữ Liệu/Nhà Khoa Học Dữ Liệu:
1. Xem lại **Data Dictionary** để hiểu định nghĩa trường
2. Khám phá **Jupyter Notebooks** trong `/notebooks` để hiểu phương pháp phân tích
3. Kiểm tra **Cleaned Data** trong `/cleaned data` để có dữ liệu có thể tái tạo
4. Xem **Raw Data** trong `/raw data` để lấy thông tin nguồn

---

## 🚀 Getting Started

### Prerequisites

Yêu cầu để chạy dự án:
- Python 3.8 trở lên
- Jupyter Notebook
- Power BI Desktop hoặc Power BI Online
- Các thư viện Python cần thiết (xem yêu cầu trong các sổ ghi chép riêng lẻ)

### Installation

Hướng dẫn cài đặt:

```bash
# Sao chép kho lưu trữ
git clone https://github.com/Suonbicha11052005/colgate-manufacturing-analytics.git

# Điều hướng đến thư mục dự án
cd colgate-manufacturing-analytics

# Cài đặt các gói cần thiết
pip install -r requirements.txt
```

---

## 📝 Data Dictionary Reference

Để lấy thông tin chi tiết về các trường dữ liệu và định nghĩa, hãy tham khảo `Data dictionary.xlsx` bao gồm:
- Tên trường và mô tả kinh doanh
- Loại dữ liệu và phạm vi hợp lệ
- Phương pháp tính toán cho các chỉ số dẫn xuất
- Ghi chú về chất lượng và tính hoàn chỉnh

---

## 🤝 Contributing

Thành viên Nhóm: **Sigma Seeker**

Để đóng góp hoặc có câu hỏi:
1. Mở một issue để báo cáo lỗi hoặc yêu cầu tính năng
2. Gửi pull request để cải thiện
3. Cập nhật tài liệu cho bất kỳ thay đổi nào

---

## 📋 License

Dự án này là một phần của đề cử RBAC 2025 vòng 2. Bí mật và chỉ dành cho công nội bộ.

---

## 📞 Contact & Support

Nếu có câu hỏi về dự án này, vui lòng liên hệ với nhóm dự án hoặc mở một issue trong kho lưu trữ này.

---

## 🔗 References

- **Case Study:** [RBAC 2025] CASE STUDY ROUND 2.pdf
- **Presentation:** [RBAC 2025] - Round 2 - Team Sigma Seeker.pdf
- **Dashboard:** RBAC 2025 - Factory Performance.pbix
- **Data Dictionary:** Data dictionary.xlsx

---

**Last Updated:** May 2026  
**Project Status:** Active
