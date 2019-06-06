# DIMM Technologies
- **DIMM** sử dụng đường truyền `64bit` ( một số đời đầu sử dụng `128bit` , nhưng đã lỗi thời )
- **DIMM - Dual Inline Memory Module** : sở dĩ có tên như vậy vì nó có các chân độc lập nằm ở 2 mặt đối diện nhau của **module nhớ** .
- Các **SIMM** và **DIMM** đời đầu không chạy đồng bộ với **system bus** vì chúng quá chậm . **Module nhớ DIMM** đầu tiên chạy đồng bộ với **system bus** là **synchronous RAM ( SDRAM )** . **Module** này có 2 rãnh và `168` chân .
- **DDR SDRAM** ( hay **SDRAM II** , **DDR** ) là một phiên bản cải tiến của **SDRAM** . **DDR** chạy nhanh gấp đôi so với **SDRAM** thông thường . Nó có 1 rãnh và `184` chân . Thay vì chỉ xử lý dữ liệu trong 1 chu kỳ clock như loại **SDRAM** thông thường , nó xử lý dữ liệu trong nhịp clock lên và clock xuống , do đó tăng gấp đôi tỷ lệ trao đổi dữ liệu . Nếu tốc độ **bus** của **mainboard** là `200MHz` thì tốc độ **DDR** là `400MHz` .
- 3 phiên bản cải tiến của **DDR** là **DDR2** , **DDR3** , **DDR4** . **DDR2** nhanh hơn và tiêu thụ ít điện năng hơn **DDR** . **DDR3** nhanh hơn và tiêu thụ ít điện năng hơn **DDR2** . **DDR4** nhanh hơn và tiêu thụ ít điện năng hơn **DDR3** . Cả **DDR2** và **DDR3** đều có `240` chân . **DDR4** có `288` chân . Chúng không tương thích với nhau vì các khứa ( ***notch*** ) đặt ở vị trí khác nhau .
- Các yếu tố ảnh hưởng đến dung lượng , đặc điểm và hiệu năng của **DIMM** bao gồm :
    - Số lượng **RAM** trên 1 thanh **DIMM**
    - Cách chíp được lắp đặt và đánh địa chỉ trên **DIMM**
    - Số lượng **channel** được sử dụng
    - Tốc độ
    - Khả năng sửa lỗi
    - Bộ đệm ( **cache** )
    - Thời gian truy cập dữ liệu
## **1) Single , Dual , Triple and Quad Channels**
- Khi nhìn vào **mainboard** , sẽ thấy các khe **DIMM** có màu khác nhau . Những màu này chỉ ra loại **channel** mà slot sử dụng . **Channel** phải quyết định số lượng khe **DIMM** mà bộ nhớ có thể đánh địa chỉ cùng 1 thời điểm .
- Trước đây , **DIMM** chỉ sử dụng ***single-channel*** , có nghĩa bộ nhớ chỉ đánh được địa chỉ cho 1 thanh **DIMM** tại 1 thời điểm .
- Để cải tiến hiệu suất , ***dual channels*** cho phép bộ nhớ giao tiếp với 2 thanh **DIMM** tại cùng thời điểm , làm tăng tốc độ truy cập bộ nhớ . **DDR** , **DDR2** , **DDR3** , **DDR4** có thể sử dụng ***dual channels*** .
- **Mainboard** hỗ trợ ***triple channels*** có thể truy cập 3 thanh **DIMM** tại cùng thời điểm . **DDR3** có thể sử dụng được ***triple channels*** .
- **Quad channels** có thể truy cập 4 thanh **DIMM** tại 1 thời điểm . Cả **DDR3** và **DDR4** đều có thể sử dụng ***quad channels*** .
### **1.1) Dual channels**
- **Mainboard** có 2 **channel** là **channel A** và **channel B** .
- 2 thanh **DIMM** cắm ở 2 khe ghi là **Channel A** sẽ được đánh địa chỉ tại cùng 1 thời điểm . 2 thanh **DIMM** cắm ở 2 khe ghi là **Channel B** sẽ được đánh địa chỉ tại cùng 1 thời điểm .

    <img src=https://i.imgur.com/MMWu6tw.png>

- Khi thiết lập ***Dual channels*** , 2 thanh **DIMM** cùng 1 **channel** phải giống nhau về dung lượng , tốc độ , tính năng , và tốt nhất là của cùng 1 nhà sản xuất . Các thanh **DIMM** khác **channel** không nhất thiết phải giống nhau . Nếu 2 thanh **DIMM** cùng 1 **channel** không tương thích với nhau , **mainboard** sẽ tự chuyển thành ***single channel*** .

    <img src=https://i.imgur.com/6c2kdNW.png>

- Theo VD trên : 2 khe **DIMM** màu đen tạo thành **channel** đầu tiên , 2 khe màu xanh tạo thành **channel** thứ 2 . Để sử dụng ***dual channels*** , các cặp **DIMM** giống nhau phải được xếp vào 2 khe xanh , hoặc 2 khe đen .

    <img src=https://i.imgur.com/TIqEQcl.png>

### **1.2) Triple channels**
- Để thiết lập ***triple channels*** , 3 khe **DIMM** phải được gắn bởi 3 thanh **DIMM** giống nhau .

    <img src=https://i.imgur.com/uMXx4AN.png>

- Theo VD trên : 
    - 3 thanh **DIMM** được gắn trên 3 khe màu xanh trên **mainboard** .
    - **Mainboard** còn 1 khe thứ 4 màu đen .
    - Nếu khe màu đen được sử dụng , ***triple channels*** sẽ không hoạt động , làm giảm hiệu năng .
    - Trên **mainboard** này , nếu có 2 cặp **DIMM** giống nhau , có thể sử dụng ***dual channels*** với cả 4 thanh . ***Dual channels*** không nhanh bằng ***triple channels*** nhưng chắc chắn tốt hơn ***single channel*** .
### **1.3) Quad channels**
- Được giới thiệu cùng với **chipset** và **CPU Sandy Bridge** ( 2<sup>nd</sup> generation )

    <img src=https://i.imgur.com/1qlQv8D.png>

- Theo VD trên :
    - **Mainboard Intel** sử dụng **socket LGA2011** cùng với 8 khe **DIMM**
    - 4 khe màu đen có thể được đánh địa chỉ bởi **CPU** như 1 **channel** và 4 khe màu xanh còn lại là 1 **channel** .
    - Để đạt được hiệu suất tốt nhất , nên cắm các thanh **DIMM** sát phía với **CPU** để rút ngắn **bus** .
## **2) DIMM Speeds**
- Tốc độ thanh **DIMM** được tính theo **MHz** ( VD `1333MHz` hoặc `2400MHz` ) hoặc tính theo **PC rating** ( VD `PC6400` ) .
- **PC rating** được tính bằng tổng băng thông ( `MB/s` ) của dữ liệu khi di chuyển từ **module nhớ** tới **CPU** . Để tính **PC rating** của 1 thanh **DIMM** , ta chia tốc độ bởi `8-byte` ( bởi vì **DIMM** có đường dữ liệu `64bit` = `8byte` ) .<br>**VD :** 1 thanh **DDR** hoạt động ở `800MHz` có **PC rating** là `800` * `8` = `6400 MB/s` => **`PC6400`**
- **PC rating** ở **DDR2** được kí hiệu là **PC2** , ở **DDR3** được kí hiệu là **PC3** và ở **DDR4** kí hiệu là **PC4** .

    <img src=https://i.imgur.com/KUuRrA1.png>

<center>

| **Type** | **Speed** | **PC Rating** |
|----------|-----------|---------------|
| **DDR4** | 3200 MHz | PC4-25600 |
| **DDR4** | 3000 MHz | PC4-24000 |
| **DDR4** | 2933 MHz | PC4-23466 |
| **DDR4** | 2666 MHz | PC4-21333 |
| **DDR4** | 2600 MHz | PC4-21300 |
| **DDR4** | 2400 MHz | PC4-19200 |
| **DDR4** | 2133 MHz | PC4-17000 |
| **DDR4** | 1866 MHz | PC4-14900 |
| **DDR4** | 1600 MHz | PC4-12800 |
| **DDR3** | 2000 MHz | PC3-16000 |
| **DDR3** | 1800 MHz | PC3-14400 |
| **DDR3** | 1333 MHz | PC3-10600 |
| **DDR2** | 800 MHz | PC2-6400 |
| **DDR2** | 667 MHz | PC2-5400 |
| **DDR** | 500 MHz | PC4000 |

</center>

## **3) Single-sided và Double-sided DIMMs**

