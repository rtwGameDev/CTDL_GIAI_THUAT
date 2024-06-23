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
## HƯỚNG DẪN SỬ DỤNG
### LOGIN: Trang đăng nhập 
![z5566111907141_cf6a4eb4b19737c6f0cfe04445f3d425](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/dbbe929c-50e7-43a5-8e3c-acf79cfe1187)
#### - Đăng nhập vào ứng dụng, nhấn login
----------------------------------------------------------------------------------------------------------------------------------------
### PASSENGER: Trang giao diện hành khách.
![z5566111941960_26f8a0333d40996179c7dc1cee76baa6](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/f4a7eff3-10f2-45a6-89ba-76f95c96b23c)
#### - Hiển thị danh sách chuyến bay, lựa chọn 1 chuyến bay để xem danh sách hành khách trên chuyến bay đó. Trên mỗi phần tử chuyến bay chưa thông tin về MÃ SỐ CHUYẾN BAY, THỜI GIAN KHỞI HÀNH - Ngày Tháng Năm Giờ Phút Địa điểm tới.
#### - Khung "FILTER_BY_FIELD" lọc các chuyến bay theo thời gian và địa điểm.
#### - Tính năng "ALL PASSENGER" cho phép dẫn đến trang xem toàn bộ hành khách đã từng đặt vé máy bay.
#### - Tính năng "RESET ALL" cho phép đặt tất cả ô tìm kiếm và khung lọc về mặc định.
#### - Thanh tìm kiếm theo mã chuyến bay. (SPECIAL)
#### - Đồng hồ cập nhật theo thời gian thực.
#### - LogOut giúp thoát ứng dụng trở lại trang Login
----------------------------------------------------------------------------------------------------------------------------------------
### ALL-PASSENGER: Trang hiển thị tất cả thông tin các hành khách đã từng đặt vé máy bay.
![z5566111941925_50b7a127d2fa708051e31665ea799ef7](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/97946691-205d-4d16-a18c-4eb00ad0c9b6)
#### - Mỗi hành khách gồm các thông tin: Mã căn cước công dân, họ và tên, giới tính.
#### - Các chức năng sắp xếp danh sách hành khách theo, mã căn cước, theo họ, theo tên, theo giới tính.
#### - Khung "INFOMATION" hiển thị chi tiết thông tin cũng như tiện cho việc sửa và thêm hành khách
#### - Thanh tìm kiếm hành khách theo Mã căn cước.
#### - Tính năng chỉnh sửa thông tin hành khách (Edit).
#### - Tính năng thêm hành khách (ADD Passenger)
#### - Back cho phép quay lại trang chính của Passenger Page
----------------------------------------------------------------------------------------------------------------------------------------
### EDIT PASSENGER: Chỉnh sửa thông tin hành khách
![z5566111941951_8b69fe26d1098deb5cba6f1ab0137ab9](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/2df57ee0-d5b8-48e6-bcca-86499a69c7f2)
#### - Tính năng cho phép chính sửa lại căn cước, họ tên, giới tính, đảm bảo không trùng lặp CCCD, không bỏ trống bất kì thông tin nào
----------------------------------------------------------------------------------------------------------------------------------------
### ADD PASSENGER: Cho phép nhập thêm thông tin hành khách, đảm bảo đầy đủ thông tin và không trùng lặp.
![z5566111941966_92cabdb383aa95f09ae038699773dbd2](https://github.com/rtwGameDev/CTDL_GIAI_THUAT/assets/127731925/f36fc183-3b13-419e-9367-529e39a4565c)
----------------------------------------------------------------------------------------------------------------------------------------
