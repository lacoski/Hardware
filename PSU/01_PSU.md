# PSU - Power Supply Unit
## **1) Khái niệm**
- **Bộ cấp nguồn** , còn được gọi là **đơn vị cấp nguồn** ( **PSU - *power supply unit*** ) có hình dạng 1 cái hộp bên trong **case** máy tính , cấp điện cho **mainboard** và các thiết bị khác .
- **PSU** hoạt động với vai trò của bộ chỉnh lưu và của máy biến áp để chuyển đổi dòng điện xoay chiều dân dụng thành dòng điện 1 chiều và sau đó giảm điện áp từ `110V` hoặc `220V` xuống `3.3V` , `5V` , `12V` .
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
    | <img src=https://i.imgur.com/C5NEaoP.png width=30%> | +3.3V , &plusmn;5V , &plusmn;12V | **20-pin P1 connector** . Là dây nguồn tổng cho **mainboard** sử dụng cho các chuẩn **ATX** cũ |
    | <img src=https://i.imgur.com/SBRFo33.png width=30%> | +3.3V , &plusmn;5V , &plusmn;12V | **24-pin P1 connector** ( hay cũng gọi là **20+4 pin connector** ). Là dây nguồn tổng cho **mainboard** sử dụng cho các chuẩn **ATX** mới |
    | <img src=https://i.imgur.com/Kzej2Qh.jpg width=30%> | +12V | **4-pin 12-V connector** . Được sử dụng để cấp nguồn 12V thứ cấp cho **CPU** |
    | <img src=https://i.imgur.com/IezlXN0.jpg width=30%> | +12V | **8-pin 12-V connector** . Là dây cắm phụ 12V để cấp nguồn thêm cho **CPU** , cung cấp công suất lớn hơn so với các loại dây 4-pin cũ |
    | <img src=https://i.imgur.com/AuyXMDu.png width=30%> | +5V , +12V | **4-pin Molex connector** . Được sử dụng để cấp nguồn cho ổ **IDE** cũ hoặc một số ổ **SATA** có hỗ trợ |
    | <img src=https://i.imgur.com/rxef2qY.jpg width=30%> | +3.3V , +5V , +12V | **Sata power connector** sử dụng để cấp nguồn cho các ổ cứng chuẩn **SATA** |
    | <img src=https://i.imgur.com/3VsMMZX.jpg width=30%> | +5V , +12V | **4-pin Berg connector** sử dụng để cấp nguồn cho ổ đĩa mềm ( **FDD** ) cũ |
    | <img src=https://i.imgur.com/t5SkkrZ.jpg width=30%> | +12V | **PCIe 6-pin connector** cung cấp thêm đường điện `12V` cho card đồ họa công suất cao sử dụng **PCIe 1.0** |
    | <img src=https://i.imgur.com/pnEeXS5.jpg width=30%> | +12V | **PCIe 8-pin connector** cung cấp thêm đường điện `12V` cho card đồ họa công suất cao sử dụng **PCIe 2.0** |
- Nếu **PSU** không có **connector** cần thiết , có thể sử dụng **converter** để chuyển đổi sang dạng **connector** khác :

    <p align=center><img src=https://i.imgur.com/I7VAfTz.png width=50%></p>

- Một số **PSU** sử dụng các dây riêng biệt để kết nối vào chúng . Việc này làm giảm việc trong **case** có các dây dẫn không cần thiết => **case** gọn hơn => tản nhiệt tốt hơn :

    <img src=https://i.imgur.com/JeoBENO.png>

### **2.4) Fans inside the PSU**
- Tất cả các bộ nguồn đêu có 1 quạt tản nhiệt bên trong nó ; một số loại có tới 2 quạt tản nhiệt .
- Kích cỡ quạt rộng khoảng `80mm -> 150mm` .

    <p align=center><img src=https://i.imgur.com/UUYX69d.jpg width=70%></p>
- Quạt càng lớn thì tản nhiệt càng tốt và chạy càng êm .
- Một số loại **PSU** có thêm tính năng tự điều chỉnh tốc độ quạt dựa theo nhiệt độ đo được bên trong nó .
### **2.5) Dual voltage options**
- Một số **PSU** có công tắc chuyển đổi chế độ nguồn đầu vào giữa `115V` ở Mĩ và `220V` ở các quốc gia khác .

    <img src=https://i.imgur.com/eAJwmhl.jpg>

### **2.6) Extra features**
- Nên xem xét chế độ bảo hành và chất lượng tổng thể của **PSU** .
- Một số **PSU** được thiết kế để hỗ trợ 2 card đồ họa cho các máy tính gaming . Hai công nghệ hỗ trợ 2 card đồ họa là **SLI** của **NVIDIA** và **Crossfire** của **AMD** .
- Những **PSU** càng đắt tiền hơn thì càng chạy êm hơn , bền hơn và không bị nóng như những **PSU** rẻ tiền .
- Ngoài ra , một **PSU** tốt có thể bảo vệ hệ thống khỏi bị quá áp
## **3) Tính toán công suất cần thiết cho PSU**
- Khi quyết định về công suất cần thiết cho bộ nguồn , cần tính đến **tổng công suất** cho tất cả các thành phần bên trong **case** và cả những thiết bị lấy nguồn từ **mainboard** như **USB** , **Firewire** .
- **Card đồ họa** tiêu tốn nhiều điện năng nhất , và chúng sử dụng từ nguồn `12V` . Nếu máy tính có card đồ họa , cần chú ý công suất tiêu thụ của đường `12V` ghi trên **PSU** . Xu hướng máy tính hiện nay thường đi kèm các cổng hiển thị gắn trên **mainboard** , vì vậy giảm đi lượng công suất tiêu tốn . Card đồ họa được sử dụng chính cho các máy tính gaming và các hệ thống yêu cầu cao về đồ họa .
- Công suất chịu đựng **PSU** nên cao hơn khoảng `30%` so với tổng công suất cần thiết . Điều này giúp kéo dài hiệu năng và tránh bị quá nhiệt . Tuy nhiên , không phải **PSU** công suất cao thì tốn nhiều điện . Các bộ phận chỉ sử dụng phần điện năng nó cần .<br>**VD :** **PSU** `1000W` và đang tiêu thụ `500W` sẽ bền hơn và tỏa nhiệt ít hơn là **PSU** `750W` và tiêu thụ `500W` .
- Bảng công suất tiêu thụ của các thành phần trong máy tính :

| **Thiết bị** | **Công suất xấp xỉ** |
|-------------|----------------------|
| **Mainboard** , **CPU** , **RAM** , **chuột** , **bàn phím** | `200-300W` |
| **Quạt tản nhiệt** | `5W` |
| **Ổ cứng SATA** | `15-30W` |
| **Ổ DVD/CD** | `20-30W` |
| **Card đồ họa PCI** | `50W` |
| **Card PCI khác** | `20W` |
| **Card đồ họa PCIe x16** | `150-300W` |
| **Card PCIe x16 khác** | `100W` |