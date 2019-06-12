# PSU - Power Supply Unit
## **1) Khái niệm**
- **Bộ cấp nguồn** , còn được gọi là **đơn vị cấp nguồn** ( **PSU - *power supply unit*** ) có hình dạng 1 cái hộp bên trong **case** máy tính , cấp điện cho **mainboard** và các thiết bị khác .
- **PSU** hoạt động với vai trò của bộ chỉnh lưu và của máy biến áp để chuyển đổi dòng điện xoay chiều dân dụng thành dòng điện 1 chiều và sau đó giảm điện áp từ `110V` hoặc `220V` xuống `3.5V` , `5V` , `12V` .
## **2) Các đặc điểm của PSU**
### **2.1) Form-factor ( ATX or Micro-ATX )**
- Chuẩn **PSU** quyết định kích cỡ **PSU** và vị trí các lỗ bắt vít của **PSU** để cố định **PSU** vào **case** .

    <img src=https://i.imgur.com/qcqT96A.png>

### **2.2) Wattage ratings**
- **PSU** có thông số về tổng công suất tiêu thụ đầu ra tối đa ( vd : `500W` , `850W` , `1000W` ) và mỗi mức **điện áp ( *voltage* )**  cho từng dây đầu ra . Thông số về các mức điện áp này thường được liệt kê trên phần thông tin trên mặt của **PSU** .

    <img src=https://i.imgur.com/LRg6rEr.png>

- Khi chọn **PSU** , đặc biệt chú ý đến công suất cho dây ( **rail** ) `+12V` . Các dây `+12V` là dây được sử dụng nhiều nhất , đặc biệt trong hệ thống gaming cao cấp . Đôi khi cần chọn bộ nguồn có công suất cao hơn tổng công suất cần thiết để có đủ công suất trên dây này .
- **PSU** có công suất từ `1000W` trở lên có thể có 2 dây `+12V` và gọi là ***dual rail power supply*** . Dây thứ 2 này dùng để đảm bảo an toàn rằng dây 1 không bị quá tải .
### **2.3) Number and type of connectors**
- Cần chú ý số lượng và loại dây connector mà **PSU** cung cấp .

    <img src=https://i.imgur.com/yKT1eT6.png>

- Bảng một số **connector** phổ biến :

    | **Connector** | **Điện áp** | **Mô tả** |
    |---------------|-------------|-----------|
    | <img src=https://i.imgur.com/C5NEaoP.png width=50%> | +3.3V , &plusmn;5V , &plusmn;12V | **20-pin P1 connector** . Là dây nguồn tổng cho **mainboard** sử dụng cho các chuẩn **ATX** cũ |
    | <img src=https://i.imgur.com/SBRFo33.png width=50%> | +3.3V , &plusmn;5V , &plusmn;12V | **24-pin P1 connector** ( hay cũng gọi là **20+4 pin connector** ). Là dây nguồn tổng cho **mainboard** sử dụng cho các chuẩn **ATX** mới |
    | <img src=https://i.imgur.com/Kzej2Qh.jpg width=50%> | | **4-pin 12-V connector** . Được sử dụng để cấp nguồn 12V thứ cấp cho **CPU** |
    | <img src=https://i.imgur.com/IezlXN0.jpg width=50%> | | **8-pin 12-V connector** . Là dây cắm phụ 12V để cấp nguồn thêm cho **CPU** , cung cấp công suất lớn hơn so với các loại dây 4-pin cũ |
    | <img src=https://i.imgur.com/AuyXMDu.png width=50%> | | **4-pin Molex connector**
- Nếu **PSU** không có **connector** cần thiết , có thể sử dụng **converter** để chuyển đổi sang dạng **connector** khác :

    <p align=center><img src=https://i.imgur.com/I7VAfTz.png width=50%></p>

- Một số **PSU** sử dụng các dây riêng biệt để kết nối vào chúng . Việc này làm giảm việc trong **case** có các dây dẫn không cần thiết => **case** gọn hơn => tản nhiệt tốt hơn :

    <img src=https://i.imgur.com/JeoBENO.png>

