# CPU Components
## **1) Các thành phần bên trong CPU**

<img src=https://i.imgur.com/VwhK7ML.png>

- **CPU** bao gồm 5 thành phần chính :
    - **CU - Control Unit** : quản lý tất cả các hoạt động diễn ra trong **CPU** .
    - **ALUs - Arithmetic Logic Units** : một hoặc nhiều **ALU** sẽ thực hiện việc so sánh và tính toán bên trong **CPU** .RAM
    - **Registers** : thanh ghi : hoạt động giống như **RAM** : chứa bộ đếm , dữ liệu , chỉ dẫn và địa chỉ mà **ALU** đang xử lý . 
    - **Internal Memory Caches** ( **L1 , L2** và có thể cả **L3 , L4** ) : chứa dữ liệu chờ đến lượt để **ALU** xử lý .
    - **Bus** : kết nối các thành phần bên trong **CPU** giúp chúng có thể trao đổi được với nhau . Những **bus** này hoạt động ở tần số cao hơn so với **bus** trên **mainboard** - kết nối **CPU** đến **chipset** và **bộ nhớ** .
        - **FSB** sẽ có giá trị bằng `1/4` xung nhịp của **CPU** ( **VD :** nếu **CPU** làm việc ở xung nhịp `3.2GHz` thì **FSB** sẽ là `800MHz` )
## **2) Phân loại CPU**
- Dựa theo hình trên , ta thấy **Internal data bus** có độ rộng là `32bit` có nghĩa là : mỗi khối **ALU** và **register** chỉ có thể xử lý `32bit` dữ liệu tại 1 thời điểm .
- Hầu hết **CPU** của **Intel** hay **AMD** hiện nay đều chứa **ALUs** và **registers** có thể xử lý `32bit` hoặc `64bit` tại cùng 1 thời điểm .<br>
=> Phân thành 3 loại chính :
    - **CPU `32bit`** : 
        - Những **CPU** cũ này được biết đến với cái tên "**vi xử lý `x86`**" bởi vì **Intel** sử dụng số `86` trong các mẫu **vi xử lý** này .
        - **CPU `32bit`** chỉ có thể chạy được hệ điều hành `32bit` .
    - **CPU có thể xử lý `32bit` và `64bit`** :
        - Những **CPU** lai này được gọi là "**vi xử lý `x86_64`**" .
        - **AMD** đã sản xuất ra mẫu **CPU** này đầu tiên ( **Athlon 64** ) và gọi công nghệ này là **AMD64** .
        - **Intel** cải tiến công nghệ này vào **Pentium 4** và gọi là **Extended Memory 64 Technology ( EMT64 )** .
        - **CPU `x86_64`** có thể chạy được cả hệ điều hành `32bit` và `64bit` .
        - Tất cả PC và laptop sản xúât sau năm `2007` đều sử dụng loại **CPU** này .
    - **CPU `64bit`** : 
        - **Intel** tạo ra **vi xử lý `64bit`** cho máy **workstation** và **server** sử dụng hoàn toàn hệ thống `64bit` bao gồm **Itanium** và **Xeon** .
        - **Intel** gọi công nghệ này là **IA64** .
        - Chúng yêu cầu chạy trên hệ điều hành `64bit` và có khả năng chạy được những ứng dụng `32bit` nhờ khả năng giả lập .
