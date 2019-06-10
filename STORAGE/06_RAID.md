# RAID - Redundant Array of Independent Disks
## **1) Các loại RAID**
- Có nhiều loại **RAID** được định nghĩa , trong đó 4 loại phổ biến nhất là **RAID 0** , **RAID 1** , **RAID 5** , **RAID 10** . 
### **1.1) Spanning**
- **Spanning** ( thi thoảng còn được gọi là **JBOD - just a bunch of disks** ) , sử dụng 2 ổ cứng để tạo thành 1 **Windows volume** riêng biệt .
- Dữ liệu được ghi lên ổ cứng thứ nhất trước , và sau khi ổ cứng thứ nhất đầy , dữ liệu mới tiếp tục được ghi lên ổ thứ hai .
    <p align=center><img src=https://i.imgur.com/bJC142K.png></p>

### **1.2) RAID 0**
- **RAID 0** cũng sử dụng 2 hoặc nhiều ổ cứng vật lý để tăng thêm không gian lưu trữ cho 1 **volume** .
- **RAID 0** ghi dữ liệu qua lần lượt tất cả các ổ cứng vì vậy không ổ nào có đầy đủ dữ liệu toàn vẹn => cải thiện hiệu năng .
- Windows gọi **RAID 0** là **striped volume** .
- **RAID 0** được ưu tiên hơn **spanning** .
    <p align=center><img src=https://i.imgur.com/uYe2ji9.png></p>

### **1.3) RAID 1**
- **RAID 1**là 1 dạng nhân bản dữ liệu : dữ liệu sẽ được nhân bản từ 1 ổ cứng sang ổ cứng còn lại với vai trò là ổ cứng chịu lỗi ( **fault tolerance** ) .
- Mỗi ổ cứng sẽ chia ra các **volume** ( hay các **partition** ) . 2 **volume** ở 2 ổ khác nhau tạo thành 1 **mirror** .
- Nếu 1 ổ cứng bị hỏng , ổ cứng còn lại sẽ hoạt động tiếp và dữ liệu không bị mất .
- Windows gọi **RAID 1** là **mirror volume** .
    <p align=center><img src=https://i.imgur.com/y3GV1sG.png></p>

### **1.4) RAID 5**
- **RAID 5** chia dữ liệu ra 3 hoặc nhiều hơn 3 ổ cứng và sử dụng bit **parity** để sửa lỗi .
- Nếu 1 ổ bị hỏng , các ổ khác có thể dựa vào **parity** để tái tạo lại dữ liệu trên ổ bị hỏng .
- Dữ liệu trong **RAID 5** sẽ không bị nhân bản , do đó , **RAID 5** giúp lưu trữ dữ liệu được nhiều hơn .
- **RAID 5** cung tăng cường hiệu năng và cung cấp khả năng chịu lỗi ( **fault tolerance** ) .
- Windows gọi những **volume** sử dụng **RAID 5** là **RAID 5 volume** .
    <p align=center><img src=https://i.imgur.com/StuRDC9.png></p>
### **1.5) RAID 10**
- **RAID 10** hay còn gọi là **RAID 1+0** , phát âm là "RAID một không" ( không phải "RAID mười" ) , là 1 sự kết hợp của **RAID 1** và **RAID 0** .
- **RAID 10** cần ít nhất 4 ổ cứng để tạo thành 1 **volume** .
- Dữ liệu được nhân bản qua các cặp ổ cứng , thêm vào đó , 2 cặp ổ được **striped** với nhau .
    <p align=center><img src=https://i.imgur.com/WmgJ4m7.png></p>

## **2) Cách triển khai RAID cứng**
- Khi triển khai hệ thống **RAID cứng** ( *hardware RAID* ) , để đảm bảo hiệu năng tốt nhất , tất cả ổ cứng thành phần cần được đồng nhất về : 
    - ***Brand*** : hãng sản xuất
    - ***Size*** : dung lượng ổ
    - ***Speed*** : tốc độ đọc ghi , tốc độ vòng quay ( HDD )
- Nếu như Windows được cài đặt trên 1 ổ đĩa sử dụng **RAID** , thì **RAID** phải được tiến hành trước khi cài đặt Windows .
- Trước khi thực hiện , phải đảm bảo rằng **mainboard** hỗ trợ **RAID** .
> ### **VD :** thực hiện **RAID 5** với ổ cứng **SATA** trên **mainboard**
- **B1 :** Cắm 3 ổ cứng **SATA** vào 3 cổng **SATA** trống ở trên **mainboard** :

    <img src=https://i.imgur.com/HLRt9xf.png>

- **B2 :** Boot vào hệ thống và đi vào cài đặt **UEFI/BIOS** .
    - Trong cửa sổ ***Advanced setup*** , kiểm tra xem 3 ổ cứng đã được nhận dạng chưa . 
    - Chọn tùy chọn ***Configure SATA*** và chọn ***RAID***

    <img src=https://i.imgur.com/ssDudcU.png>

- **B3 :** Reboot lại máy . Sau khi máy khởi động lên sẽ có 1 thông điệp hiện ra : " `Press <Ctrl+I> to enter the RAID
Configuration Utility` " . Gõ `Ctrl` + `I` để vào cấu hình **RAID** . Chú ý : trạng thái của các ổ phải là **Non-RAID**

    <img src=https://i.imgur.com/IacTb5q.png>

- **B4 :** Chọn ***1. Creat RAID Volume*** . Cửa sổ mới hiện ra , nhập tên **volume** :

    <img src=https://i.imgur.com/bqYWok0.png>

- **B5 :** Ở phần ***RAID Level*** , chọn ***RAID5 (Parity)*** . Do chỉ cắm 3 ổ đĩa , nên tùy chọn chọn ổ đĩa để **RAID** sẽ không hiện ra . Tất cả các ổ đĩa sẽ được thực hiện **RAID** .
- **B6:** Chọn giá trị ***Strip Size*** . Đây là khoảng đơn vị dữ liệu cho mỗi **strip** khi đi qua các ổ . Các lựa chọn là : ***32KB , 64KB , 128KB*** .
- **B7 :** Nhập vào kích thước **volume** tạo ra  ( ***Capacity*** ) . Khoảng không gian trống còn lại sẽ dùng để tạo các **RAID volume** khác .
- **B8 :** Chọn ***Creat Volume*** để hoàn thành cấu hình **RAID** . 1 cảnh báo sẽ hiện ra " `If you proceed , all data on all three hard drives will be lost`" . Gõ `Y` để tiếp tục . **RAID volume** sẽ được tạo ra sau khi reboot .

