# HDD - Hard Disk Drive
- **HDD ( Hard Disk Drive )** thường được gọi là ổ cứng ( **hard drive** ) là dạng ổ cứng truyền thống .
## **1) Phân loại**
- Có 2 loại kích thước thường dùng trong máy tính là :
    - **3.5"** dùng cho PC
    - **2.5"** dùng cho Laptop cá nhân , có thể dùng được cho PC

        <img src=https://i.imgur.com/KlkMyDG.png>
        
## **2) Cấu tạo**
- Là loại ổ cứng từ tính ( **magnetic hard drive** ) .
- Một ổ cứng từ ( **magnetic hard drive** ) có một , hai hoặc nhiều **đĩa từ** ( ***platter*** ) được xếp chồng lên nhau và cùng xoay tròn bên trong 1 **vỏ bọc kim loại** , chứa **firmware** điều khiển việc đọc , ghi dữ liệu vào **ổ cứng** và điều khiển việc giao tiếp với **mainboard** . Mặt trên và mặt dưới của mỗi đĩa có 1 **đầu đọc/ghi** di chuyển trên bề  mặt **đĩa** trong khi tất cả các đĩa xoay quanh 1 **trục** ( ***spindle*** ) . Tất cả các **đầu đọc/ghi** được điều khiển bởi 1 bộ phận truyền động , điều khiển việc di chuyển các đầu đọc ghi trên khắp bề mặt **đĩa** . Bề mặt **đĩa** được phủ 1 lớp từ tính có thể chứa dữ liệu dưới dạng các điểm từ .

    <img src=https://i.imgur.com/rplxXOx.png>

- Tốc độ trục xoay thường là **`5400`** , **`7200`** hoặc **`10000 RPM`** ( ***revolutions per minute*** - vòng trên phút ) . Trục quay càng nhanh , ổ cứng hoạt động càng hiệu quả .
> Còn phần **jumper** ?
## **3) Các đơn vị của ổ cứng**

<img src=https://i.imgur.com/9Pdu1Jg.jpg>

### **3.1) Tracks**
- Trên một mặt của đĩa từ chia ra làm nhiều vòng tròn đồng tâm gọi là các **track** .
- Thường mỗi đĩa từ có từ 321 đến 2048 **track** .
### **3.2) Sectors**
- Mỗi **track** lại được chia thành các đoạn `4096 bytes` gọi là các **sector** ( hay còn được gọi là các **record** ) .
- Một số ổ cứng cũ sử dụng **sector** gồm `512 bytes` .
- Mỗi một **sector** có địa chỉ riêng ( được quy định bằng số **track** cộng với số **sector** ), dùng để tổ chức và định vị dữ liệu .
### **3.3) Clusters**
- Các **sector** trên cùng một **track** kết hợp với nhau tạo thành **cluster** và dữ liệu sẽ được lưu trữ trên các **cluster** .

    <p align=center><img src=https://i.imgur.com/Jvo7Dkg.png width=50%></p>
- Thường khi format thì 1 **cluster** = `8` **Sector** ( `4Kb` )
    - Trên Windows gọi đơn vị này là **cluster** .
    - Trên Linux gợi đơn vị này là **inode** .
- Khi lưu trữ 1 tập tin vào đĩa cứng **HDD** , ổ cứng **HDD** sẽ tìm kiếm các **cluster** còn trống kế tiếp nhau để ghi dữ liệu lên . Trong trường hợp các **cluster** không liên nhau thì nó sẽ kiếm các **cluster** còn trống kế tiếp đó nữa ( đây chính là nguyên nhân của sự phân mãnh trên đĩa cứng **HDD** )
### **3.4) Cylinders**
- Tất cả các **track** có cùng khoảng cách đến tâm đĩa tạo thành 1 **cylinder** .
- Mỗi đĩa từ có nhiều track nên trên một ổ đĩa cứng **HDD** sẽ có nhiều **cylinder**
## **4) Cách tổ chức dữ liệu**
- **Firmware** nằm trong 1 bo mạch bên trong vỏ ổ cứng , chịu trách nhiệm việc ghi và đọc dữ liệu vào các **track** , **sector** và giữ cho dữ liệu được lưu trữ trên các **track** này . Một số ổ cứng bảo vệ bảng mạch bên trong 1 lớp vỏ bọc .
- Trước khi **ổ cứng** xúât xưởng , **track** và **sector** được ghi lên **ổ cứng** thông qua quá trình gọi là **low-level formatting** ( định dạng ở mức thấp ) . **Firmware** , **UEFI/BIOS** trên **mainboard** và hệ điều hành sử dụng 1 hệ thống đánh số tuần tự gọi là đánh số địa chỉ logic ( **LBA - logical block addressing** ) để đánh dấu tất cả các **sector** trên ổ cứng . Kích cỡ của mỗi **block** và số các **block** trên ổ cứng phụ thuộc vào dung lượng của ổ cứng . Ngày nay , dung lượng ổ cứng thường được tính bằng **`GB`** ( gigabytes ) hoặc **`TB`** ( terabytes = 1024 gigabytes ) . Ổ đĩa từ có dung lượng lưu trữ lớn hơn nhiều lần so với ổ **SSD** .

## **5) Các chuẩn ổ cứng HDD**
### **5.1) IDE / EIDE / ATA - PATA**
- Chuẩn **IDE - Integrated Drive Electronics** sử dụng phương thức truyền tải dữ liệu song song ( parallel )
    - Ưu điểm : tốc độ cao. Trong cùng một thời điểm có thể truyền tải nhiều bit dữ liệu hơn so với truyền tải nối tiếp .
    - Nhược điểm : Sử dụng nhiều dây dẫn để truyền các bit dữ liệu đi nên gây ra hiện tượng tạp âm nhiễu. Đó là lý do vì sao **ATA-66** sử dụng lên đến `80` dây dẫn . Bởi vì giữa các dây truyền tín hiệu là các dây mát nằm xen kẽ dây tín hiệu để chống nhiễu .
- Chuẩn **EIDE - Enhanced IDE** : Do chuẩn **IDE** bị giới hạn dung lượng đĩa cứng tối đa , Nên người ta sử dụng chuẩn **EIDE** để thay thế
    - Chia làm 2 kênh ( **primary** và **secondary** ) và 2 kênh này sử dụng 2 đường **bus** riêng .
    - Trên mỗi kênh lại chia làm 2 cấp ( **master** và **slave** ) trên cùng 1 kênh . Vì cả 2 thiết chỉ được phép sử dụng 1 đường **bus** trong cùng 1 thời điểm .
    - **EIDE** không có khả năng cho phép nhiều thiết bị sử dụng cùng 1 **bus** trong cùng 1 thời điểm . Nên các thiết bị sẽ được cấp phép để sử dụng tuần tự đường **bus** .
- **ATA - Advanced Technology Attachment** ( còn được gọi là **PATA** – **Parallel ATA** ) sử dụng một giao tiếp gồm `40` chân cắm và cáp `80` dây :

    <img src=https://i.imgur.com/1c36O93.png>

- Chuẩn **ATA** có dung lượng thấp và tốc độ truyền thấp. Được phát triển và mở rộng dần dần từ **ATA1** đến **ATA7** . Để nâng cao hiệu suất của **EIDE** mà không làm tăng chi phí, không còn cách nào khác người ta phải thay thế kiểu truyền song song bằng kiểu nối tiếp ( serial ) . Kết quả là chuẩn **SATA** ra đời .

    | **ATA Standard** | **Throughput** |
    |------------------|----------------|
    | **ATA1** | 8.3 MBps |
    | **ATA2** | 16.6 MBps |
    | **ATA3** | 16.6 MBps |
    | **ATA4** | 33 MBps | 
    | **ATA5** | 66 MBps |
    | **ATA6** | 100 MBps |
    | **ATA7** | 133 MBps |
### **5.2) SATA / AHCI**
- 27/5/2009 tổ chức **ATA** đã chính thức công bố chuẩn **SATA 3.0 ( Serial ATA )** với băng thông dữ liệu lên đến `6Gb/s` và nó cho phép tương thích ngược với các chuẩn cũ ( **SATA 1.0** , **SATA 2.0** ) .

    | **SATA Standard** | **Throughput** |
    |-------------------|----------------|
    | **SATA 1** | 1,5 Gbps |
    | **SATA 2** | 3 Gbps |
    | **SATA 3** | 6 Gbps |
- **SATA** sử dụng công nghệ khác cho phép truyền tải theo chế độ nối tiếp ( serial ).
- Các chip điều khiển **SATA** đều hỗ trợ chuẩn giao tiếp **AHCI** ( ***Advanced Host Controller Interface*** ) làm giao tiếp chuẩn , hỗ trợ các tính năng nâng cao như **hot-swap** . Tính năng này chỉ hỗ trợ khi thiết bị chạy chế độ **AHCI** . Những hệ điều hành từ Windows Vista hoặc mới hơn thì mới hỗ trợ **AHCI** . Có thể enable tính năng này trong **BIOS** .
- Thường sử dụng cho các thiết bị máy tính cá nhân . Sử dụng cable `7` chân và chỉ có `7` sợi nên gọn hơn nhiều so với **ATA** . Điều này giúp ích rất nhiều đến khía cạnh tỏa nhiệt của máy tính , vì sử dụng nhiều cáp mỏng hơn sẽ làm cho không khí lưu thông bên trong case của máy tính được dễ dàng hơn .

    <img src=https://i.imgur.com/q2ewZPd.png>

### **5.3) SCSI**
- **SCSI - Small Computer System Interface** ( còn được gọi là **parallel SCSI** ) . Là chuẩn sử dụng phương thức truyền tải dữ liệu song song .
- Thường sử dụng trong các server lưu trữ và truyền dữ liệu với tốc độ cao .
- Là chuẩn giao tiếp thường dùng để kết nối với ổ cứng , máy in , CD-ROM,…

    <img src=https://i.imgur.com/9pq9fyD.png>

- **SCSI** có nhiều kiểu chân kết nối :

    <img src=https://i.imgur.com/GqSe669.jpg>

- **SCSI** không quan tâm đến thiết bị nó kết nối đến là gì . Nó chỉ quan tâm thiết bị đó có làm việc được với chuẩn **SCSI** không .
- Ổ cứng **SCSI** có bộ điều khiển **SCSI** có vi xử lý riêng để xử lý việc truyền nhận dữ liệu và công việc của các thiết bị liên quan mà không cần sử dụng **CPU** chính để xử lý . Điều này giúp **CPU** không phải tốn tài nguyên để xử lý các công việc truyền tải mà sử dụng tài nguyên cho việc khác .
- Bởi vì những hạn chế của phương thức truyền tải dữ liệu song song . Nên kể từ năm `2005` **Parallel SCSI** đã được thay thế bằng một chuẩn sử dụng phương thức truyền tải dữ liệu nối tiếp là **Serial Attached SCSI** .
### **5.4) SAS**
- **Serial Attached SCSI ( SAS )** là giao thức nối tiếp point-to-point dùng để truyền dữ liệu từ máy tính đến các thiết bị lưu trữ .
- **SAS** là chuẩn giao tiếp mới , ra đời sau nhưng lại có nhiều cải tiến về hiệu suất và tốc độ . Nó cho phép nhiều thiết bị ( hơn 128 thiết bị ) với các kích thước khác nhau được kết nối đồng thời vào 1 sợi cáp mỏng .

    <img src=https://i.imgur.com/DfGzQfR.png>
- Chân kết nối của **SAS** có phần gần giống với **SATA** :
    <p align=center><img src=https://i.imgur.com/zhY4jHA.jpg></p>
- Ưu điểm :
    - **SAS** rất mạnh trong việc quản lý dữ liệu , cho phép người dùng thao tác dễ dàng với dữ liệu .
    - **SAS** cho phép làm việc với nhiều file dữ liệu cùng lúc.
    - Hỗ trợ cơ chế **hot-swap** .
- **SAS** cho phép kết nối lên đến `65.535` thiết bị với chiều dài cáp tối đa `10m` .
- **SAS** bao gồm 3 giao thức vận chuyển ( transport protocol ) cho phép kết nối với các thiết bị **SCSI**, **SATA** và **SAS** .
    - **Serial SCSI Protocol (SSP)** : Giao tiếp ở mức độ lệnh với các thiết bị **SCSI**
    - **Serial ATA Tunneling Protocol (STP)** : giao tiếp command-level với các thiết bị **SATA**
    - **Serial Management Protocol (SMP)** : quản lý **SAS fiber**
- Kiến trúc **SAS** bao gồm 6 layers :
    - **Physical layer** :
        - Xác định các đặc tính điện và vật lý
        - Hỗ trợ nhiều loại kết nối :
            - SFF-8482 – SATA compatible
            - Internal four-lane connectors: SFF-8484, SFF-8087, SFF-8643
            - External four-lane connectors: SFF-8470, SFF-8088, SFF-8644
    - **PHY Layer** :
        - Khởi tạo liên kết, thương lượng tốc độ và thiết lập lại trình tự
        - Hỗ trợ mã hóa dữ liệu `8b/10b` ( tốc độ `3,6` và `12 Gbit/s` ) . Mỗi nhóm `8 bit` được mã hóa thành một số `10 bít` để đạt hiệu quả cho tốc độ clock .
        - Mã hóa gói tin `128b/150b` ( `22.5 Gbit/s` ). Nó bao gồm `2 bit` header , `128 bit` payload và `20 bit` kiểm tra lỗi kết nối .
    - **Link layer** :
    - **Port layer** :
        - Kết hợp nhiều **PHY** cùng địa chỉ vào các ports rộng.
    - **Transport Layer** :
    - **Application Layer** :
- Các kiểu kết nối trong **SAS** :
    - Các máy chủ lưu trữ thường có Backplane để tháo lắp nóng các ổ cứng. Trên backplane có các chân cắm cho phép gắn trực tiếp các ổ cứng vào Backplane mà không cần phải sử dụng day cáp giống như trong PC. Backplane có thể là một kết nối một disk array và một hoặc nhiều controller.
    - Backplane cho các ổ cứng SAS và SATA thương sử dụng giao thức SGPIO để giao tiếp giữa máy chủ và Backplane
    - Các ổ cứng trong hệ thống lưu trữ sẽ được gắn vào chung một backplane. Các backplane được gắn trên mainboard của server của thiết bị lưu trữ để giao tiếp giữa CPU với các đĩa cứng .
    - Cable được gắn internal hoặc External theo dạng
        - Connect Mainboard đến Backplane
        - HBA đến Backplane
        - HBA đến các thiết bị lưu trữ bên ngoài
- **SAS** vẫn còn ít sử dụng hơn **SATA** bởi vì :
    - Giá thành cao .
    - Để tận dụng sức mạnh của **SAS** người dùng phải mất thời gian học để hiêu các quản lý dữ liệu của **SAS** .
### **5.5) FC**
- **FC - Fibre channel** là công nghệ mạng tốc độ cao ( `2,4,8 và 16 Gbps` ) . Hỗ trợ cả cáp quang và cáp đồng để phục vụ cho hệ thống lưu trữ.

    <p align=center><img src=https://i.imgur.com/oleY6UU.jpg></p>
- **FC Protocol** là giao thức vận chuyển ( transport protocol ) dùng để chuyển các tập lệnh **SCSI** trên hạ tầng mạng **FC** .
    - Chuẩn **FC** chia thành 5 lớp từ **FC0** đến **FC4** , không theo mô hình **OSI** .
    - Không tương thích ngược với các thiết bị thấp tốc .
    - Cáp quang tùy loại , có thể dài tới `50km` .
    - Tốc độ truyền dữ liệu có thể thay đổi phụ thuộc vào loại cáp , chiều dài cáp , cấu hình lắp ráp , cần được tính đến khi thiết kế .
- Kiến trúc **FC** :
    - **FC 4 - Protocol-mapping layer** : Các giao thức lớp ứng dụng như **SCSI** hoặc **IP** ,… được đóng gói thành các **PDU** để được phần phối đến **FC2** .
    - **FC3 – Common Services layer** : Thực hiện mã hóa dữ liệu (encryption) hoặc thực hiện các thuật toán **RAID** .
    - **FC2 – Network Layer** : Bao gồm phần lõi của **Fibre channel** và định nghĩa ra các giao thức chính ( giao thức đóng gói frame dữ liệu và điều khiển luồng dữ liệu )
    - **FC1 – Data link layer** : thực hiện mã hóa đường truyền ( line coding ) cho tín hiệu và đồng bộ hóa dữ liệu khi truyền .
    - **FC0 – Physical** : Định nghĩa tốc độ truyền và các phương tiện vật lý bao gồm : cáp , bộ phận kết nối , ổ đĩa …
    - Dữ liệu truyền trong **FC** gọi là **Frame** . Tối đa 1 **Frame FC** là `2148 byte` .
    - Mỗi **frame** chứa nhiều lớp với công dụng khác nhau .
> Tham khảo : [**SAS và FC**](http://svuit.vn/threads/chapter-4-2-cac-chuan-giao-tiep-cua-o-cung-server-1313/)