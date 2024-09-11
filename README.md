# Dự Đoán Giá Thuê Căn Hộ

## Giới Thiệu

### Bối Cảnh và Mục Tiêu
Trong bối cảnh thành phố đông đúc với nhu cầu thuê căn hộ ngày càng cao, việc định giá căn hộ trở nên thách thức đối với người cho thuê và môi giới bất động sản. Dữ liệu bao gồm thông tin về giá thuê, diện tích, số phòng ngủ, số phòng tắm và nhiều yếu tố khác. Mục tiêu của phân tích này là xây dựng mô hình dự đoán giá thuê căn hộ chính xác, giúp người cho thuê và môi giới định giá hợp lý theo nhu cầu thị trường.

## Phương Pháp Xử Lý Dữ Liệu

### Phân Tích Thống Kê và Trực Quan Hóa
- **Phân Tích Exploratory Data Analysis (EDA)**: Khám phá các mẫu, xu hướng và mối quan hệ qua biểu đồ như scatter plots, box plots và pair plots.
- **Phân Phối Chuẩn Hóa và Biểu Đồ Histogram**: Hiểu rõ tính phân phối của biến số và phát hiện bất thường.
- **Phân Tích Tương Quan**: Xác định các biến quan trọng và ảnh hưởng của chúng qua ma trận tương quan và scatter plot.

### Tiền Xử Lý Dữ Liệu
- **Xử Lý Giá Trị Thiếu**: Điền giá trị thiếu hoặc loại bỏ các mẫu dữ liệu chứa giá trị thiếu.
- **Chuyển Đổi Định Dạng Dữ Liệu**: Chuyển các biến chuỗi thành số và biến thời gian thành dạng datetime.
- **Biến Đổi Log**: Áp dụng log-transform để cải thiện phân phối dữ liệu và giảm ảnh hưởng của giá trị cực đoan.
- **Tạo Biến Giả**: Chuyển các biến phân loại thành biến số.
- **Chuẩn Hóa Dữ Liệu**: Sử dụng kỹ thuật chuẩn hóa để đảm bảo các biến số nằm trong cùng phạm vi giá trị.
- **Xử Lý Giá Trị Ngoại Lai**: Xác định và xử lý giá trị ngoại lai bằng IQR hoặc boxplot.

## Xây Dựng và Đánh Giá Mô Hình

### Các Phương Pháp
- **Chia Dữ Liệu**: Tập huấn luyện và tập kiểm tra với tỷ lệ 70-30 hoặc 80-20.
- **Cross-Validation**: Áp dụng k-fold cross-validation để giảm bias và variance.
- **Đánh Giá Hiệu Suất**: Sử dụng các chỉ số như RMSE, MAE và R-squared.

### Kiểm Tra và Tối Ưu Hóa
- **Kiểm Tra Giả Định Mô Hình**: Đảm bảo tính tuyến tính, đồng nhất phương sai và phân phối chuẩn của phần dư.
- **Loại Bỏ Giá Trị Ngoại Lai**: Phân tích biểu đồ thặng dư và Cook’s distance để loại bỏ các điểm dữ liệu ngoại lai.
- **Mở Rộng Mô Hình**: Cân nhắc hồi quy đa thức, hồi quy splines, GAM để cải thiện độ chính xác.

## Kết Quả và Ứng Dụng

- **Dự Đoán Giá Thuê**: Cung cấp dự đoán chính xác, hỗ trợ quyết định kinh doanh và tối ưu hóa lợi nhuận từ việc cho thuê căn hộ.
- **Insights Về Thị Trường**: Phân tích phân phối và mối quan hệ giữa giá thuê, diện tích, số phòng ngủ và số phòng tắm, cung cấp thông tin quan trọng về thị trường.

## Các Mục Tiêu Cần Đạt Được

1. **Xử Lý Dữ Liệu Hiệu Quả**: Đảm bảo dữ liệu sạch sẽ và hoàn chỉnh.
2. **Biến Đổi Dữ Liệu Để Cải Thiện Phân Phối**: Giảm thiểu ảnh hưởng của giá trị cực đoan.
3. **Xử Lý Các Biến Phân Loại**: Giúp mô hình hồi quy tuyến tính hiểu các biến phân loại.
4. **Phân Tích và Loại Bỏ Giá Trị Ngoại Lai**: Đảm bảo các giá trị ngoại lai không ảnh hưởng lớn đến mô hình.
5. **Phân Tích Tương Quan và Quan Hệ Giữa Các Biến**: Hiểu rõ mối quan hệ giữa các biến chính.
6. **Xây Dựng và Đánh Giá Mô Hình Dự Đoán**: Xây dựng mô hình chính xác và đánh giá hiệu suất.
7. **Tối Ưu Hóa Mô Hình và Đưa Ra Dự Đoán Chính Xác**: Tối ưu hóa mô hình để cung cấp dự đoán chính xác.
8. **Cung Cấp Hiểu Biết Quan Trọng Về Thị Trường**: Phân tích để cung cấp thông tin chi tiết về nhu cầu và xu hướng thị trường.

Việc xử lý và phân tích dữ liệu khoa học sẽ giúp xây dựng mô hình dự đoán giá thuê căn hộ chính xác và hiệu quả, hỗ trợ định giá căn hộ hợp lý và tối ưu hóa lợi nhuận từ hoạt động kinh doanh bất động sản.

