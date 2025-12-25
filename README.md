**Khai thác dữ liệu (Data Mining):** là một lĩnh vực xuất hiện khi lượng dữ liệu 
ngày càng nhiều và phức tạp. Hiểu một cách gần gũi, đây là quá trình tìm kiếm những 
thông tin quan trọng ẩn bên trong các tập dữ liệu lớn mà mắt thường hoặc cách phân 
tích thông thường khó nhận ra. Người ta áp dụng nhiều kỹ thuật khác nhau, từ thống 
kê, học máy cho đến các phương pháp phân tích truyền thống, nhằm phát hiện ra các 
xu hướng, mối liên hệ hay mô hình có ích cho việc nghiên cứu hoặc ra quyết định.
```
# Bài toán phân lớp
- xác định đặc trưng
- tìm tìm liệu: màu của các cái lớp, ví dụ chụp ảnh toàn bộ các cái ảnh, lưu trên insets
- liệt kê toàn bộ các cái đặc trưng, ví dụ bánh xe, loại xe, màu,...
- trích xuất các cái đặc trưng ra => thiết kế hàm f(a1, a2,... an) => ... ? true : false; ( dùng công thức toán học, tổ hợp hàm đơn)
```bash
=> tìm ra hàm f thì nó là mô hình phân lớp
```
Bài toán kinh điển: xác định email có spam hay không spam
# Mô hình Decision Tree
## giải thuật tìm được Free
- sort lại theo một thể thống nhất
- underfitting && overfitting
- có những trường hợp đoán đúng lỗi này nó quan trọng hơn đoán đúng loại kia nên là cần phải tách ra
### Buổi 3
**MODEL:** Cây quyết định
### Buổi 4
bài toán phân lớp( bài toán học máy)
- dữ liệu huấn luyện: dữ liệu được chuẩn bị từ trước, được thu thấp
- nguyên tác: khó liên kết tất cả thông tin bên trong bảng( khó nhất quán khi chuyển đổi)
Các nhóm mô hình sẽ tương ứng với ý tưởng khác nhau của bài toán phân lớp
1. Mô hình kinh điển ? success thì done : sáng tạo ra mô hình mới;
- **MODEL:** KNN: ý tưởng đơn giản nhất -> tư duy ghi lại từ trước (thường được gọi là rote-learner: mô hình học vẹt - learest neighbor classifier)
- tư duy viết code:
- 1.1 database
- 1.2 cần một hàm khoảng cách xem ông nào giống ông nào - distance (ex: khoảng cách eclid, khoảng cách cosin,...)
- 1.3 k (số lượng gần nhất để truy xuất)
```bash
- Nếu k quá nhỏ thì kết quá dự đoán bị ảnh hưởng rất nhiều, kết quả bị nhiễu
- nếu k quá lớn thì có thể dính các class gần
```
2. 
**MODEL:** Support Vector Machines => dự đoán đúng 100%
- tư duy viết code: chia không gian sao cho phân biệt giữa các value nhất có thể -> dùng phương trình đường thẳng để so sánh nó
- (hyperplane: siêu mặt phẳng) => thường làm việc với phương trình siêu mặt phẳng
some problem:
- thực tế dữ liệu phức tạp -> tách dữ liệu rất khó -> (khi dữ liệu nhiễu thì bỏ qua) + thêm một biến mở rộng (slack variables) => bỏ các điểm nhiễu
- giải pháp khi một đường thẳng cong dạng para => dùng kernel trick => chuyển sang đường thẳng

3.
**MODEL:** Logistic regression => hồi quy logistic
4. 
**MODEL:** Bayes Classifier
#### Noted: 
Crowd-sourcing: gán nhãn dữ liệu







  
