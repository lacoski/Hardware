# CPU Features
## **1) Speed**
- **Xung nhịp ( *frequency* )** của **CPU** chính là **tốc độ ( *speed* )** mà các thành phần bên trong nó hoạt động .
- **Tốc độ** này được đo bằng **Gigahertz** ( `GHz` )
- Những **CPU** hiện tại của **Intel** và **AMD** có thể đạt được tốc độ từ `1.8 GHz` đến hơn `4.4 GHz` .
## **2) Socket và Chipset**
- Những **socket** quan trọng của **Intel**là : **LGA1150** , **LGA1155** , **LGA1156** , **LGA2011** , **LGA1366** và **LGA775** .
- Những **socket** quan trọng của **AMD** là : **AM4** , **AM3+** , **AM3** , **AM2+** , **AM2** , **FM1** , **FM2+** và **FM2** .
## **3) Architecture ( `32bit` / `64bit` )**
- Tất cả các **CPU** của PC và Laptop hiện nay đều sử dụng **`x86_64`** , có thể xử lý `32bit` hay `64bit` dữ liệu tại 1 thời điểm .
- **CPU** này có thể chạy được hệ điều hành `32bit` và cả `64bit` .
## **4) Multiprocessing ability**
- Các nhà thiết kế ra **CPU** sáng tạo ra 1 số phương thức giúp **CPU** làm được nhiều việc hơn tại 1 thời điểm .
- 4 phương thức phổ biến là :
    - **Multiprocessing** ( đa xử lý ) : 
        - 2 **ALUs** được gắn trong 1 **CPU** được gọi là **multiprocessing** . 
        - **Pentium** là **CPU** đầu tiên chứ trong mình 2 **ALUs** , khiến cho nó có thể thực thi 2 lệnh cùng 1 lúc .
    - **Multithreading** ( đa luồng ) : 
        - Mỗi **CPU** hoặc mỗi nhân ( **core** ) xử lý 2 luồng ( **thread** ) tại cùng 1 thời điểm . Khi Windows chuyển giao 1 task cho **CPU** , nó được gọi là 1 **thread** và có thể bao hàm 1 số lệnh trong đó .
        - Để xử lý 2 **threads** , **CPU** đòi hỏi tăng thêm **registers** hoặc vùng nhớ tạm để sử dụng cho việc nhảy qua lại giữa các **thread** .
        - **Intel** gọi công nghệ này là **Hyper-Threading** và **AMD** gọi nó là **HyperTransport** .
    - **Multicore processing** ( đa nhân ) :
        - Nhiều **CPU ( core )** có thể được tích hợp trong 1 khối **CPU** được gọi là **multicore processing** .
        - Một khối **CPU** có thể chứa đựng tới **`8` cores** :
            - **Dual-core** ( 2 )
            - **Triple-core** ( 3 )
            - **Quad-core** ( 4 )
            - **Octo-core** ( 8 )
        - **VD :** **CPU quad-core** sau chứa đựng `4` **core** bên trong . Sử dụng **multithreading** , mỗi **core** có thể tạo ra `2` **thread** => Tạo ra `8` **CPU** logic có thể xử lý được `8` **thread** của hệ điều hành cùng 1 lúc :

            <img src=https://i.imgur.com/xOpKsl3.png>

    - **Dual processors** ( đa CPU ) :
        - Một **mainboard** server có thể có tới 2 **socket CPU** được gọi là **dual processors** hoặc **multiprocessor platform** :

            <img src=https://i.imgur.com/HxxnQC2.png>

## **5) Memory Cache**
- Là lượng bộ nhớ bên trong khối **CPU** .
- **CPU** ngày nay có 1 ít bộ nhớ trên chip xử lý ( gọi là **die** ) . Bộ nhớ trên **die** gọi là **Level 1 cache ( L1 cache )** .
- Bộ nhớ ở trong khối **CPU** , nhưng không nằm trên **die** , gọi là **Level 2 cache ( L2 cache )** .
- Một số **CPU** sử dụng thêm loại **cache** thứ 3 , xa chip xử lý hơn , nhưng vẫn nằm trong khối **CPU** , gọi là **Level 3 cache ( L3 cache )** .
    <img src=https://i.imgur.com/pNAVcVZ.png>
- Loại bộ nhớ sử dụng làm **cache** trong **CPU** là **static RAM ( SRAM )** .
- Loại bộ nhớ trên **mainboard** làm mất dữ liệu nhanh chóng và phải refresh thường xuyên , gọi là **volatile memory ( *bộ nhớ khả biến* )** hoặc **dynamic RAM ( DRAM )** .
- **SRAM** nhanh hơn **DRAM** bởi nó không cần phải refresh , nó có thể lưu lại dữ liệu cho đến khi mất điện .
## **6) Security**
- **Excute Disable Bit ( EDB )** ( cũng có thể gọi là **eXecute Disable ( XD )** theo **Intel** , **Enhanced Virus Protection** theo **AMD** hoặc **disable excute bit** theo **CompTIA** ) là 1 chuẩn bảo mật được tích hợp trong **CPU** để nó có thể  làm việc với hệ điều hành và xác định vùng bộ nhớ đê lưu dữ liệu và lệnh .
- Khi một khu vực được xác định là để lưu dữ liệu , các lệnh lưu trong khu vực đó sẽ không thể thực thi , do đó ngăn chặn được **buffer overflow attack** ( tấn công tràn bộ đệm ) bởi phần mềm độc hại .
- **EDB** yêu cầu hệ điều hành phải tương thích với nó .
- Có thể bật tính năng này trong **BIOS** họăc màn hình cài đặt **UEFI** :

    <img src=https://i.imgur.com/x35vpFt.png>

- Tuy nhiên , **EDB** chỉ ngăn **malwares** thực thi lệnh chứ không thể gỡ bỏ nó . Vẫn nên sử dụng thêm cả trình diệt virus để gỡ bỏ **malwares** .
## **7) Memory Support ( RAM )**
- Những loại **module DRAM** có thể sử dụng trên **mainboard** bao gồm cả **DDR** , **DDR2** , **DDR3** , **DDR4** .
- Bên cạnh loại **RAM** , **CPU** có thể hỗ trợ chính xác lượng **RAM** , tốc độ , số channel .
## **8) Support Virtualization**
- Là tính năng giúp một máy tính có thể tạo ra và quản lý nhiều máy tính ảo khác .
- Hầu hết các **CPU** hiện nay đều hỗ trợ ảo hóa , và tính năng này phải được bật trong **BIOS/UEFI** .

    <img src=https://i.imgur.com/3WGwuab.jpg>

## **9) Integrated graphics**
- Một **CPU** có thể tích hợp **GPU** trong đó .
- **GPU - graphics processing unit** là vi xử lý làm việc với dữ liệu đồ họa để xuất ra hình ảnh trên màn hình .
- **GPU** có thể ở trên **card đồ họa** , có thể trên **mainboard** , hoặc có thể tích hợp trong khối **CPU** . Khi ở bên trong **CPU** , nó gọi là **integrated graphics** ( card đồ họa tích hợp ) .
- Rất nhiều **CPU AMD** và hầu hết **CPU Intel** từ thế hệ 2 trở lên đều được tích hợp card đồ họa .
    <p align=center><img src=https://i.imgur.com/G6Sa9Jp.png width=30%></p>