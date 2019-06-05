# Bus and Expansion Slots

<p align=center><img src=https://i.imgur.com/fByspwH.png width=70%></p>

- Một **Bus** là một đường dây dẫn chung kết nối từ bên này sang bên kia mà dữ liệu có thể di chuyển trong phạm vi máy tính . Đường dẫn này sử dụng cho liên lạc và có thể thiết lập giữa 2 hay nhiều yếu tố của máy tính .

    <p align=center><img src=https://i.imgur.com/zCg7QGR.jpg width=60%></p>

- Trên **mainboard** , một **bus** được tạo thành từ một mê cung các mạch in sẵn .
- **Bus** vận chuyển 4 loại tín hiệu :
    - **Nguồn điện** : chíp trên **mainboard** cần có điện năng để làm việc . Các chip này gắn vào 1 đường năng lượng của **bus** và lấy phần năng lượng cần thiết .
    - **Tín hiệu điều khiển** : một số dây trên **bus** vận chuyển tín hiệu điều phối mọi hoạt động .
    - **Địa chỉ bộ nhớ** : các bộ phận truyền địa chỉ bộ nhớ cho 1 bộ phận khác , cho biết nơi truy cập dữ liệu hoặc các lệnh . Số dây tạo thành địa chỉ bộ nhớ của **bus** , quyết định số bit có thể sử dụng cho địa chỉ này . Vì vậy , số dây giới hạn lượng bộ nhớ mà **bus** có thể gửi .
    - **Dữ liệu** : dữ liệu đi qua **bus** trong 1 nhóm dây cũng giống như địa chỉ bộ nhớ . Số tuyến được sử dụng để truyền dữ liệu trong **bus** quyết định lượng dữ liệu có thể truyền song song trong cùng 1 thời điểm . Số tuyến này phụ thuộc vào loại **CPU** và quyết định số bit trong đường dẫn dữ liệu ( đường dẫn dữ liệu là 1 phần của **bus** để chứa dữ liệu . Nó có thể chứa được `8` , `16` , `32` , `64bit` hoặc nhiều hơn )
## **1) Front-side Bus ( FSB )**
- Đây là **bus** nhanh nhất trong hệ thống , ở tại nhân của **chipset** và **CPU** .
- **Bus** này trước tiên được sử dụng bởi **CPU** để chuyển thông tin qua lại bộ nhớ **cache** hoặc bộ nhớ chính hoặc **North Bridge** .
- Nói chung , đây là **bus** nhanh nhất trên **mainboard** , tốc độ và băng thông tùy thuộc vào sự kết hợp **CPU** và **chipset** cụ thể .
## **2) PCI Bus**
- **Bus PCI - Peripheral Component Interconnect ( *chuẩn ghép nối thành phần ngoại vi* )** 
- Có 3 loại **bus PCI** chính và trong mỗi loại lại có nhiều biến thể
### **2.1) PCI chuẩn ( Conventional PCI )**
- **Bus PCI** đầu tiên có đường dẫn dữ liệu `32bit` , cung cấp `5V` điện năng cho một card mở rộng và hoạt động với tốc độ `33MHz` . Đây là **bus** đầu tiên cho phép những card mở rộng chạy đồng bộ với **CPU** .
- **PCI** phiên bản `2.x` giới thiệu khe cắm **PCI** `64bit` , `3.3V` , nâng băng thông lên gấp đôi .
- Bởi card có thể bị hỏng khi cắm vào khe có điện áp khác , rãnh chứa hình chữ **U** ( ***notch*** ) ở khe cắm **PCI** giúp phân biệt khe `5V` và khe `3.3V` .

    <p align=center><img src=https://i.imgur.com/EkIC2nr.png width=60%></p>

- Card **PCI đa năng** ( **Universal PCI Card** ) có thể sử dụng cả 2 khe cắm `3.3V` và `5V` và có chứa cả 2 rãnh khứa .
- Hiện nay , **PCI chuẩn** có `4` loại khe cắm và `6` cấu hình card **PCI** để sử dụng các khe cắm này .

    <p align=center><img src=https://i.imgur.com/9jXzLfC.png width=80%></p>

### **2.2) PCI-X**
- Thế hệ phát triển tiếp theo của **PCI** là **PCI-X** với 3 phiên bản sửa đổi . Phiên bản mới nhất là **PCI-X 3.0** .
- Tất cả các phiên bản sửa đổi **PCI-X** đều tương thích ngược với card và khe cắm **PCI chuẩn** , ngoại trừ card **PCI** `5V` không còn được hỗ trợ .
- **PCI-X** tập trung vào các công nghệ nhắm tới thị trường Server , vì vậy , sẽ không thấy các khe cắm **PCI-X** trong máy tính để bàn .
- Các **mainboard** sử dụng **PCI-X** thường có vài khe cắm **PCI** `32bit` hoặc `64bit` chạy ở nhiều tốc độ khác nhau .

    <p align=center><img src=https://i.imgur.com/7t3WTut.png width=70%></p>

- **PCI Express** đang dần thay thế **PCI-X** .
### **2.3) PCI Express ( PCIe )**
- **PCI Express ( PCIe )** sử dụng kiến trúc hoàn toàn khác với **PCI chuẩn** và **PCI-X** .
- **PCI-e** không tương thích ngược với cả 2 loại trên .
- Trong khi **PCI chuẩn** sử dụng **bus** song song ( ***parallel bus*** ) `32bit` và `64bit` , **PCIe** sử dụng **bus** tuần tự ( ***serial bus*** ) . **Bus** này nhanh hơn **bus** song song bởi nó truyền dữ liệu giữa các dạng gói tương tự như mạng Ethernet , USB . Khe cắm **PCIe** có thể cung cấp 1 hoặc nhiều làn tuần tự như vậy .<br><br>
    <img src=https://i.imgur.com/2U8ZOLx.png>
- Hiện tại , **PCIe** có `4` kích thước khe cắm khác nhau , được gọi là **PCI Express x1** , **x4** , **x8** , **x16** .
- Các khe cắm **PCIe** không cao bằng và các chân nằm sát nhau hơn so với khe cắm **PCI** .
- Khe cắm **PCIe x1** gồm 1 làn dữ liệu đơn tạo thành . Một cặp dây được sử dụng để gửi dữ liệu và cặp còn lại nhận dữ liệu theo từng bit một . Khe cắm **x16** gồm `16` làn , mỗi làn định thời độc lập với các làn khác . Số làn càng nhiều thì lượng dữ liệu được vận chuyển trong 1 thời điểm càng lớn . Vì vậy , khe cắm **x16** nahnh hơn khe cắm **x4** , khe cắm **x4** nhanh hơn khe cắm **x1** .
- Ta có thể cắm **card PCIe** ngắn hơn vào khe cắm **PCIe** dài hơn .

    <p align=center><img src=https://i.imgur.com/B5KxY69.png width=30%></p>
- Các phiên bản **PCIe** bao gồm **PCIe version 1.1** , **PCIe version 2.0 và 2.1** , **PCIe version 3.0** , và **PCIe version 4.0** .
    - **PCIe version 1.0** : là phiên bản nguyên thủy của **PCIe** , cung cấp `150W` cho **PCIe card** ( `75W` trên khe **PCIe** và `75W` từ bộ kết nối `6-pin` từ bộ cấp nguồn ) .
    - **PCIe version 1.1** : tăng lượng điện áp lên `225W` ( `75W` trên khe **PCIe** và cho phép 2 bộ kết nối `6-pin 75W` từ bộ cấp nguồn ) .
    - **PCIe version 2.0** : tăng gấp đôi tần số **bus** của **PCIe** , có nghĩa là tăng gấp đôi băng thông về lý thuyết . Cho phép tối đa `32` làn cho mỗi khe cắm . Điện năng được cung cấp lên đến `300W` ( `75W` trên khe **PCIe** , `150W` từ 1 kết nối `8-pin` và `75W` từ 1 kết nối thứ cấp tới **mainboard** )

        <img src=https://i.imgur.com/BCpLuXO.png width=70%>

    - **PCIe version 3.0 và 4.0** : **PCIe 3.0** gấp đôi tốc độ so với **2.0** và tương thích ngược với **2.0** . **PCIe 4.0** gấp đôi tốc độ của **PCIe 3.0** và cũng tương thích ngược với các version cũ hơn . **PCIe 4.0** được ra mắt vào năm `2019` .

    <img src=https://i.imgur.com/uULOwRk.png>

### **2.4) Mini PCI và Mini PCIe trong Laptop**
- Phiên bản thu nhỏ của **PCI** và **PCIe** được sử dụng trong Laptops , All-in-One PC , hoặc **mainboard** form nhỏ như **Mini-ITX** .
- Khe cắm **Mini PCI** tuân theo chuẩn **PCI** và khe cắm **Mini PCIe** tuân theo chuẩn **PCIe** .
- Để tiết kiệm diện tích , các **mini PCI slot** nằm phẳng và giữ các card **PCI** song song với **mainboard** .
- Khe cắm **mini PCI** có `100` hoặc `124` pins và 1 **notch** ở gần rìa khe cắm :

    <p align=center><img src=https://i.imgur.com/1Jogt9t.jpg width=60%></p>

- Khe cắm **mini PCIe** có `52` hoặc `54` pins và 1 **notch** ở giữa :

    <p align=center><img src=https://i.imgur.com/kcDFZKv.png>

## **3) AGP Bus**
- Khe cắm video và card video trên **mainboard** đã sử dụng chuẩn **AGP ( Accelerated Graphics Port )** trong nhiều năm nhưng **AGP** hoàn toàn đax bị thay thế bởi **PCI Express** .
- Mỗi **mainboard** có khe cắm **PCIe x16** hoặc **AGP** chứ không thể có cả 2 .
