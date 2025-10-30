# Bank Marketing Dataset

## Giới thiệu
Dataset này liên quan đến các chiến dịch marketing trực tiếp (qua điện thoại) của một tổ chức ngân hàng tại Bồ Đào Nha. Mục tiêu của chiến dịch là thuyết phục khách hàng đăng ký sản phẩm tiền gửi có kỳ hạn (term deposit).

## Nguồn dữ liệu
- **Nguồn**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing) / Kaggle
- **Trích dẫn**: Moro et al., 2014
- **Số lượng mẫu**: 41,188 (phiên bản đầy đủ)
- **Số lượng thuộc tính**: 20 thuộc tính đầu vào + 1 biến mục tiêu

## Mô tả các cột dữ liệu

### 1. Thông tin Khách hàng (Bank Client Data)

| Tên cột | Kiểu dữ liệu | Mô tả | Giá trị |
|---------|--------------|-------|---------|
| `age` | Numeric | Tuổi của khách hàng | - |
| `job` | Categorical | Loại nghề nghiệp | admin., blue-collar, entrepreneur, housemaid, management, retired, self-employed, services, student, technician, unemployed, unknown |
| `marital` | Categorical | Tình trạng hôn nhân | divorced, married, single, unknown |
| `education` | Categorical | Trình độ học vấn | basic.4y, basic.6y, basic.9y, high.school, illiterate, professional.course, university.degree, unknown |
| `default` | Binary | Có nợ xấu không? | yes, no, unknown |
| `housing` | Binary | Có vay mua nhà không? | yes, no, unknown |
| `loan` | Binary | Có khoản vay cá nhân không? | yes, no, unknown |
| `balance` | Numeric | Số dư tài khoản trung bình hàng năm (euro) | - |

### 2. Thông tin Chiến dịch hiện tại (Current Campaign)

| Tên cột | Kiểu dữ liệu | Mô tả | Giá trị |
|---------|--------------|-------|---------|
| `contact` | Categorical | Phương thức liên lạc | cellular, telephone, unknown |
| `month` | Categorical | Tháng liên hệ cuối cùng trong năm | jan, feb, mar, apr, may, jun, jul, aug, sep, oct, nov, dec |
| `day` | Numeric | Ngày liên hệ cuối cùng trong tháng | 1-31 |
| `duration` | Numeric | Thời lượng cuộc gọi cuối cùng (giây) | - |
| `campaign` | Numeric | Số lần liên hệ trong chiến dịch này (bao gồm lần cuối) | - |

### 3. Thông tin Chiến dịch trước (Previous Campaign)

| Tên cột | Kiểu dữ liệu | Mô tả | Giá trị |
|---------|--------------|-------|---------|
| `pdays` | Numeric | Số ngày đã trôi qua kể từ lần liên hệ cuối trong chiến dịch trước | 999 = chưa từng được liên hệ trước đó |
| `previous` | Numeric | Số lần liên hệ với khách hàng trước chiến dịch này | - |
| `poutcome` | Categorical | Kết quả của chiến dịch marketing trước | failure, nonexistent, success, unknown |

### 4. Chỉ số Kinh tế - Xã hội (Social and Economic Context)

| Tên cột | Kiểu dữ liệu | Mô tả | Tần suất cập nhật |
|---------|--------------|-------|-------------------|
| `emp.var.rate` | Numeric | Tỷ lệ biến động việc làm | Quý |
| `cons.price.idx` | Numeric | Chỉ số giá tiêu dùng (CPI) | Tháng |
| `cons.conf.idx` | Numeric | Chỉ số niềm tin người tiêu dùng | Tháng |
| `euribor3m` | Numeric | Lãi suất Euribor 3 tháng | Ngày |
| `nr.employed` | Numeric | Số lượng nhân viên | Quý |

### 5. Biến Mục tiêu (Target Variable)

| Tên cột | Kiểu dữ liệu | Mô tả | Giá trị |
|---------|--------------|-------|---------|
| `y` | Binary | Khách hàng có đăng ký tiền gửi có kỳ hạn không? | yes, no |

