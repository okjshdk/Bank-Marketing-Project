# Bank Marketing Campaign Analysis

## Mục tiêu
- Phân tích **hiệu quả chiến dịch** và **nhóm khách hàng tiềm năng**.
- Xây dựng mô hình học máy **dự đoán khả năng khách hàng gửi tiền**.

---

## Kết quả phân tích

| Chỉ tiêu | Kết quả |
|-----------|----------|
| **Khách hàng liên hệ** | ~ 41.000 |
| **Thành công** | 4.640 |
| **Tỉ lệ chuyển đổi gốc** | 11,27% |

## Kết quả mô hình

|-----------|----------|
| **Model Accuracy** | 83,4% |
| **ROC-AUC** | 0.796 |
| **Recall (khách gửi tiền)** | 0.61 |
| **Precision (khách gửi tiền)** | 0.36 |

📈 So với tỉ lệ thành công gốc chỉ **11%**, mô hình giúp **tăng ~3 lần khả năng xác định đúng khách hàng tiềm năng**, hỗ trợ ngân hàng **tập trung marketing vào nhóm khách hàng hiệu quả hơn**.

---

## Insight từ phân tích dữ liệu

### Nhóm khách hàng tiềm năng
- **Độ tuổi:** >65 (46,85%) và <25 (20,95%) có tỉ lệ gửi tiền cao nhất.  
- **Tình trạng hôn nhân:** Độc thân có tỉ lệ thành công cao hơn (14%).  
- **Công việc:** Student (31,4%) và Retired (25,2%) hiệu quả nhất.  
- **Học vấn:** University degree đạt 13,7%, cao hơn trung bình.  

*→ Tập trung nhóm độc thân, học vấn cao, Student/Retired trong chiến dịch kế tiếp.*

---

### Hiệu quả chiến dịch
- **Tỉ lệ chuyển đổi cao nhất** trong **2 cuộc gọi đầu tiên** (13,0% và 11,5%).  
- **Cellular** hiệu quả **gấp 2.8 lần** so với Telephone.  
- **Ngày hiệu quả nhất:** Thứ 3 → Thứ 5 (11,7% – 12,1%).  
- Khi quy mô liên hệ quá lớn trong tháng, chất lượng cuộc gọi giảm thì **tỉ lệ thành công giảm rõ rệt**.  

*→ Tập trung chất lượng trong 2 cuộc gọi đầu, ưu tiên kênh Cellular, đảm bảo quy mô và chất lượng cuộc gọi.*

---

## Mô hình dự đoán
**Model:** XGBoost Classifier  

| Class | Precision | Recall | F1-score | Support |
|:------|:----------:|:-------:|:---------:|:--------:|
| 0 (Không gửi tiền) | 0.95 | 0.86 | 0.90 | 6,796 |
| 1 (Gửi tiền) | 0.36 | 0.61 | 0.45 | 851 |

---

## Cấu trúc dự án

| Thư mục / Tệp | Mô tả |
|----------------|-------|
| `data/` | Dữ liệu từ [Kaggle - Bank Marketing Dataset](https://www.kaggle.com/datasets/henriqueyamahata/bank-marketing) |
| `dashboard/BankMarketingProject.pbix` | Dashboard trực quan (Power BI) |
| `insight marketing campaign customers.md` | Phân tích nhóm khách hàng tiềm năng |
| `insight marketing campaign performance.md` | Phân tích hiệu quả chiến dịch |
| `ML model/Identifying_Potential_Customers.ipynb` | Notebook mô hình XGBoost |
| `README.md` | Tổng quan dự án |

---

## 🚀 Kết luận
- Mô hình giúp **nâng cao hiệu quả gấp 3 lần** so với marketing đại trà.  
- **Cellular** và **2 cuộc gọi đầu tiên** là chiến lược tối ưu.  
- **Nhóm khách hàng tiềm năng:** Student, Retired, độ tuổi cao, độc thân, học vấn cao.  
- **Ứng dụng:** Hỗ trợ ngân hàng **tập trung nguồn lực marketing chính xác hơn và giảm chi phí đáng kể.**
