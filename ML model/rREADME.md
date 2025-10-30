# Xây dựng mô hình dự đoán khách hàng gửi tiền

## Giới thiệu

Dự án sử dụng bộ dữ liệu **Bank Marketing** để dự đoán khả năng khách hàng sẽ gửi tiền vào ngân hàng sau các chiến dịch marketing.  
Mô hình được xây dựng bằng **XGBoost Classifier**, phân loại khách hàng thành hai nhóm:

- **Gửi tiền** (`y = 1`)  
- **Không gửi tiền** (`y = 0`)

## **Hiệu quả mô hình**

**Mô hình:** XGBoost Classifier  
**Accuracy:** 83.4% | **ROC-AUC:** 0.796  

| Class | Precision | Recall | F1-score | Support |
|:------|:----------:|:-------:|:---------:|:--------:|
| 0 (Không gửi tiền) | 0.95 | 0.86 | 0.90 | 6796 |
| 1 (Gửi tiền) | 0.36 | 0.61 | 0.45 | 851 |

**Tổng kết:**  
- Mô hình phát hiện được **61% khách hàng thực sự gửi tiền** (**Recall = 0.61**).  
- **Precision = 0.36**, cao gấp khoảng **3 lần tỉ lệ thành công thực tế (11,27%)**
- Mô hình **hỗ trợ ngân hàng sàng lọc nhóm khách hàng tiềm năng**, giúp **tập trung nguồn lực marketing hiệu quả hơn**.

