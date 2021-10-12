# Giới thiệu
## 1.1 Mục đích
## 1.2 Phạm vi
Tài liệu này được áp dụng cho Hệ thống dịch vụ xe ôm công nghệ ( HTDVXOCN), sẽ được phát triển bởi nhóm bài tập PTTKHT của chúng tôi. HTVXOCN sẽ công cấp dịch vụ và ứng dụng di động tìm xe ôm thuận tiện thông minh, có nhiều ưu điểm so với hệ thống xe ôm truyền thống
## 1.3 Định nghĩa, viết tắt
- HTDVXOCN - Hệ thống dịch vụ xe ôm công nghệ
- PTTKHT - Phân tích thiết kế hệ thống
## 1.4 
---
# 2. Tình trạng
## 2.1 Cơ hội kinh doanh
Trong thời đại phát triển công nghệ số, hiện đại hoá ngày nay, nhiều phát minh, ứng dụng đã khiến cuộc sống của con người ngày càng thuận tiện, nhẹ nhàng hơn thông qua các ứng dụng dịch vụ hiện đại sử dụng công nghệ tiên tiến như Đám mây, API, Android...
Việc sử dụng dịch vụ xe ôm không nằm ngoài những dịch vụ có thể cải thiện chất lượng thông qua những công nghệ đó. Nếu áp dụng thành công, chi phí cho người sử dụng dịch vụ, và thu nhập của người cung cấp dịch vụ (tài xế) đều có thể tăng thêm. Đồng thời, chúng ta (bên thứ 3) có thể làm trung gian giữa 2 bên và tạo cơ hội kinh doanh từ đó.


## 2.2 Nêu vấn đề
| Vấn đề | Cơ chế truyền thống của dịch vụ xe ôm hiện nay còn lạc hậu|
|---|---|
|Ảnh hưởng| Với hệ thống xe ôm truyền thống, người sử dụng dịch vụ và người cung cấp dịch vụ |
| Ảnh hưởng | Nhu cầu sử dụng dịch vụ xe ôm thấp hơn so với tiềm năng thị trường |
| Biện pháp cải thiện| Một bên thứ 3 quản lý, tìm kiếm tài xế và khách đi xe thông qua công nghệ|

## 2.3 Sản phẩm
| Dành cho | Người có nhu cầu sử dụng dịch vụ xe ôm |
| --- | --- |
| Ứng dụng đặt xe thông minh | là một ứng dụng phần mềm |
| Có tính năng | Tìm kiếm tài xế, sử dụng dịch vụ xe ôm và đánh giá tài xế sau mỗi chuyến |
| Không giống | Dịch vụ xe ôm truyền thống, không có cơ chế đảm bảo cho người sử dụng dịch vụ và cả tài xế |
| Sản phẩm của chúng ta | Cung cấp một trải nghiệm người dùng thật tốt, giao diện trực quan dễ hiểu, hướng tới mọi lứa tuổi, có cơ chế đánh giá tài xế, người sử dụng dịch vụ|

# 3. Các bên liên quan & miêu tả người dùng
## 3.1 Thị trường nhân khẩu học
## 3.2 Tổng hợp các bên liên quan
| Tên | Miêu tả | Trách Nhiệm|
|---|---|---|
| Kĩ sư nghiệp vụ | Làm việc với khách hàng và cách bên lên quan khác để đưa ra yêu cầu cho hệ thống| Xác định nghiệp vụ, yêu cầu vận hàng và yêu cầu không-vận-hành|
| Kĩ sư kiến trúc phần mềm| Giữ vai trò dẫn dắt chính cho dự án| Chịu trách nghiệm thiết kế hệ thống bao quát, và hướng dẫn bao quát thiết kế và cách vận hành hệ thống đó|
| Quản lý dự án| Bên dẫn dắt sự phát triển của UDDXTM| Lên kế hoạch, quản lý, phân công tài nguyên, quyết định ưu tiên phát triển của dự án. Làm việc với bên liên quan và giữ cho team định hướng| 

## 3.3 Người dùng

| Tên | Miêu tả | Trách Nhiệm| Bên liên quan|
|---|---|---|---|
|Tài xế| Người sử dụng chính của hệ thống | Sử dụng ứng dụng để kết nối đến máy chủ, đưa đón hành khách khi được thông báo ghép cặp| Chính họ |
| Hành khách| Người sử dụng chính của hệ thống|  Sử dụng ứng dụng để tìm kiếm tài xế phục vụ việc đi lại| Chính họ|
| Quản trị viên | Người sử dụng hệ thống | Sử dụng các công cụ của hệ thống, quản trị tài nguyên, lái xe, hàng khách, quản trị hoá đơn trực tuyến| Chính họ |
| Tổng đài viên | Người sử dụng hệ thống | Sử dụng hệ thống để giải quyết, trả lời các thắc mắc, xử lý các vụ việc xảy ra trong quá trình ứng dụng vận hành|

## 3.4 Môi trường người dùng
1. Hành khách muốn sử dụng dịch vụ xe ôm sử dụng UDDXTM để tìm kiếm tài xế. Người dùng chọn điểm đón và điểm đến cho hành trình.
2. Hệ thống sẽ tìm kiếm và gắp cặp tài xề phù hợp nhất cho người dùng
3. Tài xế điểm đến điểm đón và đưa người dùng tới điểm đến.
4. Hệ thống ghi nhận quá trình sử dụng dịch vụ của hành khách.
5.  Hành khách có thể đánh giá dịch vụ, tài xế trên hệ thống

## 3.5 Hồ sơ các bên liên quan
### Tài xế
- **Miêu tả** :  Người sử dụng chính của UDDXTM
- **Loại**: Người tài xế xe ôm thông thường có thể không có kinh nghiệm sử dụng smartphone
-  **Trách nhiệm**: Trong quá trình sử dụng, bật chế độ tìm kiếm trong UDDXTM dành cho tài xế, khi được hệ thống tìm kiếm 1 khách hàng, đến điểm đón khách hàng đó và đưa họ tới điểm đến đã được xác định
-  **Đánh giá thành công**: Tài xế đăng kí, được nhận thu nhập từ hệ thống, tiếp tục sử dụng hệ thống lâu dài
-   **Mang lại**: Dịch vụ chính trong nghiệp vụ của hệ thống
-   **Nhận xét**: Không

### Hành khách
- **Miêu tả** :  Người sử dụng chính của UDDXTM
- **Loại**: Người sử dụng thông thường có thể không có kinh nghiệp sử dụng smartphone
-  **Trách nhiệm**:  Sử dụng ứng dụng, xác định điểm đón và điểm đến trong hành trình, di chuyển ra khu vực điểm đến chờ tài xế. Thực hiện hành trình và có thể đánh giá lại tài xế.
-  **Đánh giá thành công**: Khách hàng tiếp tục sử dụng dịch vụ
-   **Mang lại**: Không
-   **Nhận xét**: Không

### Người quản trị hệ thống
- **Miêu tả** :  Người sử dụng HTDVLXTM
- **Loại**:  Người quản trị đã được đào tạo, hướng dẫn sử dụng hệ thống
-  **Trách nhiệm**:  Sử dụng công cụ hệ thống để quản trị, kiểm soát các bên liên quan
-  **Đánh giá thành công**: Không
-   **Mang lại**: Không
-   **Nhận xét**: Không

### Tổng đài viên
- **Miêu tả** :  Người sử dụng HTDVLXTM
- **Loại**:  Người quản trị đã được đào tạo, hướng dẫn sử dụng hệ thống
-  **Trách nhiệm**: Sử dụng hệ thống để giải quyết, trả lời các thắc mắc, xử lý các vụ việc xảy ra trong quá trình ứng dụng vận hành
-  **Đánh giá thành công**: Không
-   **Mang lại**: Không
-   **Nhận xét**: Không

## 3.7 Ưu tiên nghiệp vụ
| Cần | Ưu tiên | Quan tâm | Giải pháp hiện tại | Giải pháp đề ra |
|---|---|---|---|---|
| Dễ dàng sử dụng | TB | Cho phép người ít/không có kinh nghiệp sử dụng smart phone cũng có thể thao tác, sử dụng ứng dụng | | Giao diện/UX trực quan, thân thiện |
| Ghép cặp tài xế và hành khách| Cao | Cho phép ghép cặp hành khác-tài xế nhanh, chính xác| | Sử dụng thuật toán hiệu quả, Máy chủ có khả năng tính toán cao |

## 3.8 Các ứng dụng thay thế/cạnh tranh
### 3.8.1 Grab
### 3.8.2 Uber

# 4. Tổng quan sản phẩm
## 4.1 Góc nhìn hệ thống
![[Untitled.drawio.png]]

## 4.2 Tổng quan tính năng
| Lợi ích cho khách hàng | Tính năng phụ trợ |
|---|---|
| Cảm thấy an toàn, yên tâm với tài xế| Xem thông tin tài xế, thời gian đã hoạt động lái xe cho hệ thống |
| Cảm thấy hài lòng, hoặc có thể báo cáo lại tài xế nếu không hài lòng| Đánh giá tài xế sau khi thực hiện hành trình |

## 4.3 Giả thuyết và các phụ thuộc
- Không có

# 5. Tính năng của sản phẩm

## 5.1. Tính năng của ứng dụng cho người dùng
- Chọn lộ trình
- Xem cước phí
- Gọi điện, liên lạc với tài xế
- Đánh giá tài xế
- Liên hệ với tổng đài

## 5.2 Tính năng của ứng dụng cho tài xế
- Thông báo ghép cặp
-  Xem thông tin người dùng, vd: SĐT,...
-  Đánh giá hành khách
-  Xem thu nhập tháng hiện tại
- Liên hệ với tổng đài

## 5.2 Tính năng của ứng dụng cho quản trị viên
- Quản lí các bên liên quan
- Quản lí các hoá đơn online
-  Quản lí thu nhập tài xế

## 5.3 Tính năng của ứng dụng cho tổng đài viên
- Liên hệ, hỗ trợ hành khách, tài xế
# 6. Ưu tiên phát triển
- Tính năng cho ứng dụng của tài xế, hành khách được ưu tiên hơn
# 7.  Hạn chế
## 7.1 Khả năng sử dụng
## 7.2 Performance

# 8. Các yêu cầu khác
## 8.1 Tiêu chuẩn ứng dụng
## 8.2 Yêu cầu hệ điều hành
Ứng dụng trên nền hệ điều hành Android, iOS, Web

# 9. Yêu cầu về tài liệu
## 9.1 Hướng dẫn sử dụng
Với mỗi ứng dụng sẽ có bản hướng dẫn sử dụng (trực tuyến đi kèm). 