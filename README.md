# Colgate Manufacturing Analytics 📊

This project focuses on analyzing operational inefficiencies in Colgate-Palmolive’s toothbrush manufacturing process, with an emphasis on machine downtime, production performance, and product quality control.

Nhà máy sản xuất đang gặp các vấn đề như:
- Downtime xảy ra thường xuyên
- Tỷ lệ rework và defect cao
- Hiệu suất vận hành chưa ổn định
- Thiết bị có độ tin cậy thấp
- Changeover và shift transition gây mất thời gian sản xuất

Các vấn đề này làm giảm Overall Equipment Effectiveness (OEE), ảnh hưởng đến throughput và làm tăng chi phí vận hành.

Dự án sử dụng dữ liệu sản xuất, maintenance logs và dữ liệu vận hành để:
- Đánh giá hiệu suất hoạt động của nhà máy
- Xác định nguyên nhân gốc rễ gây downtime và defect
- Đo lường mức độ tổn thất sản xuất
- Tìm ra các machine, line và shift có rủi ro cao
- Đề xuất các chiến lược tối ưu hóa hiệu suất vận hành

Phân tích bao gồm:
- Exploratory Data Analysis (EDA)
- Root Cause Analysis
- Manufacturing KPI Analysis
- Time Series Analysis (VAR & FEVD)
- Interactive Power BI Dashboarding

---

# 📁 Project Structure

```text
colgate-manufacturing-analytics/
│
├── README.md
├── .gitignore
│
├── cleaned data/
│   └── final_df_cleaned.csv
│
├── notebooks/
│   ├── RBAC_Coding_File_Question_1_+_Question_2_+_Question_3.ipynb
│   └── RBAC_FINAL_CODE_CLEANED.ipynb
│
├── raw data/
│   ├── cross_reference.csv
│   ├── maintenance_order.csv
│   └── production_logs.csv
│
├── [RBAC 2025] - Round 2 - Team Sigma Seeker.pdf
├── [RBAC 2025] CASE STUDY ROUND 2.pdf
├── Data dictionary.xlsx
└── RBAC 2025 - Factory Performance.pbix
```

---

# 📊 Key Metrics

## Overall Equipment Effectiveness (OEE)

Đo lường hiệu quả vận hành tổng thể của hệ thống sản xuất thông qua:
- Availability
- Performance
- Quality

OEE được sử dụng để đánh giá mức độ hiệu quả của dây chuyền sản xuất và xác định các nguồn gây tổn thất.

---

## Downtime Rate

Đo lường tỷ lệ thời gian máy không hoạt động trong thời gian sản xuất.

Downtime được phân tích theo:
- Production line
- Shift
- Product type
- Downtime reason
- Machine category

---

## Defect Rate

Đo lường tỷ lệ sản phẩm lỗi trong quá trình sản xuất.

Phân tích defect giúp:
- Xác định sản phẩm có tỷ lệ lỗi cao
- Tìm machine gây lỗi nhiều nhất
- Đánh giá sự ổn định của quy trình sản xuất

---

## Production Throughput Yield

Đo lường tỷ lệ sản phẩm đạt chất lượng đầu ra mà không cần rework.

Chỉ số này phản ánh:
- Hiệu quả vận hành
- Chất lượng quy trình
- Khả năng duy trì output ổn định

---

## Reliability Metrics

Bao gồm:
- MTBF (Mean Time Between Failures)
- MTTR (Mean Time To Repair)

Các metrics này được dùng để đánh giá:
- Độ ổn định của thiết bị
- Tốc độ xử lý sự cố
- Hiệu quả maintenance

---

# 🔍 Key Findings

## Factory Performance Below Industry Benchmark

Factory có mức OEE trung bình khoảng 50%, thấp hơn benchmark FMCG industry (~60–70%).

Nguyên nhân chính:
- Frequent downtime
- Low performance efficiency
- Rework-related interruptions
- Unstable equipment reliability

---

## Reactive Maintenance Culture

Factory hiện đang hoạt động theo hướng reactive maintenance thay vì preventive maintenance.

Biểu hiện:
- Unplanned downtime chiếm tỷ trọng lớn
- Rework là nguyên nhân downtime hàng đầu
- Downtime spikes xuất hiện nhiều ở Night shift

Điều này làm:
- Giảm tính ổn định của hệ thống
- Tăng production variability
- Làm OEE dao động mạnh

---

## High-Risk Machines and Production Lines

Một số production line có downtime rất cao:
- MKZA1501
- MKZA1502

Một số machine series có defect rate cao:
- MAFT220x

Các product có defect rate cao:
- Renew 360
- Junior Guard Taper
- Oral Care 360

---

# 🛠️ Technical Stack

## Programming & Analytics

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels

---

## Visualization & BI

- Power BI
- Jupyter Notebook

---

## Analytical Techniques

- Exploratory Data Analysis
- Root Cause Analysis
- Time Series Modeling
- VAR & FEVD Analysis
- KPI Analysis

---

# 📈 Data Sources

## production_logs.csv

Chứa dữ liệu vận hành sản xuất:
- Runtime
- Downtime
- Production quantity
- Reject quantity
- Shift information
- Production line information

---

## maintenance_order.csv

Chứa dữ liệu maintenance:
- Equipment ID
- Maintenance order
- Maintenance type
- Maintenance schedule

---

## cross_reference.csv

Bảng mapping giữa:
- Equipment ID
- Production line

---

# 🧠 Analytical Workflow

## 1. Data Cleaning

Thực hiện:
- Remove duplicates
- Handle missing values
- Convert datetime formats
- Standardize categorical values

Sau đó merge các bảng dữ liệu để tạo consolidated dataset phục vụ phân tích.

---

## 2. Exploratory Data Analysis

Phân tích:
- OEE trend
- Downtime trend
- Defect trend
- Shift performance
- Product performance
- Machine efficiency

---

## 3. Root Cause Analysis

Xác định:
- Systemic issues
- Emerging issues
- Main downtime drivers
- Main defect drivers

---

## 4. Impact Quantification

Đo lường:
- Potential production unit loss
- Material waste
- Throughput loss
- Operational inefficiency

---

## 5. Recommendation Development

Đề xuất các giải pháp:
- Preventive & predictive maintenance
- In-process quality control
- SMED optimization
- Shift handover standardization

---

# 📊 Dashboard

Project bao gồm Power BI dashboard:

```text
RBAC 2025 - Factory Performance.pbix
```

Dashboard hỗ trợ:
- OEE monitoring
- Downtime analysis
- Defect analysis
- Throughput tracking
- Shift comparison
- Production line comparison

---

# 🚀 How to Run

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/colgate-manufacturing-analytics.git
```

---

## Open Jupyter Notebook

```bash
jupyter notebook
```

---

## Open Power BI Dashboard

Mở file:

```text
RBAC 2025 - Factory Performance.pbix
```

bằng Power BI Desktop.

---

# 📌 Repository Contents

| File | Description |
|---|---|
| `RBAC_FINAL_CODE_CLEANED.ipynb` | Notebook phân tích chính |
| `final_df_cleaned.csv` | Dataset sau khi làm sạch |
| `RBAC 2025 - Factory Performance.pbix` | Interactive dashboard |
| `Data dictionary.xlsx` | Data dictionary |
| `Team Sigma Seeker.pdf` | Final presentation |
| `CASE STUDY ROUND 2.pdf` | Đề bài case study |

---

# 📄 Disclaimer

Dự án được thực hiện cho mục đích học thuật và phân tích dữ liệu.

Tất cả dữ liệu trong project là dữ liệu giả lập và không đại diện cho dữ liệu thực tế của Colgate-Palmolive.
