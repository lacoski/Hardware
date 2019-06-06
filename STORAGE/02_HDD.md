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
