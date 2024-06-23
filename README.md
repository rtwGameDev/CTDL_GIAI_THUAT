# CTDL_GIAI_THUAT
## ĐỀ BÀI
### Máy bay (Airplane)
#### - Mảng con trỏ tối đa 300 máy bay
#### - Mỗi máy bay có các thông tin: Số hiệu MB(C15), loại máy bay(C40), số dãy, số dòng
#### - Mỗi máy bay có 1 số hiệu duy nhất
#### - Số chỗ = sỗ dãy * số dòng (số chỗ >= 20)
### Chuyến bay (Flight)
#### - Danh sách liên kết đơn (Mã CB(C15), Ngày giờ khởi hành, sân bay đến, trạng thái, Số hiệu MB, danh sách vé) 
#### - Mỗi chuyến bay có 1 mã duy nhất
#### - Trạng thái chuyến bay bao gồm: 0 --> hủy chuyến, 1 --> còn vé, 2 --> hết vé, 3 --> hoàn tất
#### - Danh sách vé cho biết thông tin vé trên chuyến bay, và số CMND của hành khách đã đặt vé đó
#### - Danh sách vé được cấp phát bộ nhớ tự động dựa vào số chỗ của máy bay thực hiện chuyến bay
#### - Danh sách chuyến bay luôn có sẵn thứ tự theo mã chuyến bay
### Hành khách (Passenger)
#### Cây nhị phân tìm kiếm cân bằng(Số CMND , Ho, Ten,  Phai)
### Chương trình có các chức năng sau
#### a/ Cập nhập danh sách các máy bay (thêm / xóa / hiệu chỉnh)
#### b/ Cập nhật chuyến bay: cho phép lập chuyến bay mới, hiệu chỉnh ngày giờ khởi hành của chuyến bay, sân bay đến, số hiệu máy bay, hủy chuyến.
#### c/ Đặt vé: cho phép đặt vé trên 1 chuyến bay; nếu thông tin hành khách chưa có thì tự động cập nhật vào danh sách hành khách, nếu có rồi thì in ra màn hình để kiểm tra. Mỗi vé đều phải ghi nhận số CMND của hành khách; nếu hành khách chưa có số CMND thì yêu cầu nhập thông tin hành khách trước. Trên 1 chuyến bay, mỗi hành khách chỉ được mua 1 vé.
#### d/ Hủy vé: cho phép hủy vé đã đặt của hành khách.
e/ In danh sách các hành khách thuộc 1 chuyến bay dựa vào mã chuyến bay. Kết xuất:¬¬¬¬
DANH SÁCH HÀNH KHÁCH THUỘC CHUYẾN BAY ######
Ngày giờ khởi hành: dd/mm/yyyy hh:mm.  Nơi đến : xxxxxxxxxxx

	STT  	SỐ VÉ  	SỐ CMND  	HỌ TÊN  	PHÁI
#### f/ In danh sách các chuyến bay khởi hành trong  ngày dd/mm/yyyy đến nơi XXXX   (cho biết cụ thể số lượng các vé còn trống và giờ khởi hành)
#### g/ In danh sách các vé còn trống của 1 chuyến bay có mã chuyến bay là X. 
#### h/ Thống kê số lượt thực hiện chuyến bay của từng máy bay theo thứ tự  số lượt thực hiện giảm dần. Kết xuất:
	Số hiệu máy bay		Số lượt thực hiện chuyến bay
### Lưu ý: Chương trình cho phép lưu các danh sách vào file; Kiểm tra các điều kiện khi nhập liệu làm dữ liệu bị sai.

## HƯỚNG DẪN CÀI ĐẶT
https://wide-lunch-878.notion.site/Setup-v-c-i-t-337a59ce1ea1450d9560c0fd434d79e0?pvs=4
## HƯỚNG DẪN SỬ DỤNG![image](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/62b49bd6-a58d-4019-89bd-895ca031315e)






