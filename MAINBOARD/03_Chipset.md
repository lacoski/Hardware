# Chipset ( North Bridge + South Bridge )
- **Chipset** là tập hợp các chip ( vi mạch ) điều khiển bộ nhớ , bus trên mainboard và một số thiết bị ngoại vi .
- Một số nhà sản xuất mainboard như **Intel** và **AMD** sử dụng **chipset** riêng của họ . Các nhà sản xuất khác sử dụng **chipset** cho các hãng khác sản xuất . Các hãng sản xuất **chipset** lớn là **Intel** , **AMD** , **NVIDIA** , **SiS** .
- Bắt đầu từ loạt **chipset Intel i800** , một hub ( trục ) được sử dụng để kết nối tới các bus . Tất cả các bus I/O được kết nối với 1 hub . Hub này có kế nối tới system bus . Hub này được gọi là ***hub interface*** và kiến trúc này được gọi là kiến trúc ***hub gia tốc ( accelerated hub architecture )*** .
- Đầu nhanh của hub , có chứa bus điều khiển đồ họa và bộ nhớ , kết nối tới system bus , được gọi là **North Bridge** .
- Đầu chậm hơn của hub , được gọi là **South Bridge** có chứa bus I/O . Tất cả các thiết bị I/O , ngoại trừ màn hình và bộ nhớ , kết nối hub thông qua **South Bridge** .
- Khe cắm **PCI Express** chính được thiết kế cho card video có quyền truy cập trực tiếp đến **North Bridge** , các **PCI Express** khác phải truy cập **CPU** qua **South Bridge** chậm hơn .
- Hiện tại , phần lớn **mainboard** đã lược bỏ **North Bridge** , chỉ còn **South Bridge** do sự tiến bộ của **CPU** .
- Một **chipset** sẽ có danh pháp 3 phần , ví dụ như **Intel** có **chipset** “**`Z370`**” thì trong đó :
    - **`Z`** là chữ cái thể hiện tính năng cơ bản của dòng **mainboard** đó 
    - Số **`3`** thể hiện thế hệ và chuẩn **socket**
    - Số **`70`** thể hiện phân khúc của nó .
## **1) Chipset Intel**
- Hiện tại , **Intel** có một số những dòng **chipset** trên PC phổ biến như **`H` , `B` , `Z` , `X`** :
    - **`H`** : thường là dòng **mainboard** phổ thông ,  bị hạn chế một số tính năng để ưu tiên về mức giá .
    - **`B`** : là dòng **mainboard** tầm trung và được tích hợp tương đối đầy đủ tính năng và công nghệ của các nhà sản xuất .
    - **`Z`** : là dòng **mainboard** cao cấp , có hiệu năng mạnh mẽ , có hỗ trợ ép xung và thường được dùng chung với những **CPU** cao cấp có khả năng ép xung .
    - **`X`** : là dòng **mainboard** đặc biệt , thường có chuẩn **socket** khác hẳn với những dòng còn lại trong cùng một thế hệ . Dòng **`X`** có thể xem là trùm trong các dòng **mainboard** và thường đi chung với những **CPU** rất mạnh .
    - **`C`** : là dòng **chipset** dành cho **mainboard** Server . Được hỗ trợ công nghệ ảo hóa **Intel vPro** .
- Bảng các **chipset** của **Intel** :

| **Tên chipset** | <center>**Tính năng đi kèm**</center> |
|-----------------|----------------------|
| **H370<br>( 2018 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `20` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.1/2.0** ( tối đa `8` luồng **USB 3.1** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID 0,1,5,10**<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Tích hợp **Wireless-AC ( Wifi 5 )**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/h370.html) |
| **H310<br>( 2018 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `6` làn **PCIe** )<br>- Hỗ trợ tối đa `10` luồng **USB 3.1/2.0** ( tối đa `4` luồng **USB 3.1** )<br>- Hỗ trợ `4` cổng **SATA** tốc độ `6Gb/s`<br>- Tích hợp **Wireless-AC ( Wifi 5 )**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/h310.html) |
| **H270<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `20` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `8` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ công nghệ **Intel Optane**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/h270.html) |
| **H110<br>( 2015 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `6` làn **PCIe** )<br>- Hỗ trợ tối đa `10` luồng **USB 3.0/2.0** ( tối đa `4` luồng **USB 3.0** )<br>- Hỗ trợ `4` cổng **SATA** tốc độ `6Gb/s`<br>[Details](https://ark.intel.com/content/www/vn/vi/ark/products/90590/intel-h110-chipset.html) |
| **H81<br>( 2013 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `6` làn **PCIe** )<br>- Hỗ trợ tối đa `10` luồng **USB 3.0/2.0** ( tối đa `2` luồng **USB 3.0** )<br>- Hỗ trợ `2` cổng **SATA** tốc độ `6Gb/s`<br>[Details](https://ark.intel.com/content/www/vn/vi/ark/products/75016/intel-h81-chipset.html) |
| **B365<br>( 2018 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `20` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `8` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID 0,1,5,10**<br>- Hỗ trợ công nghệ **Intel Optane**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/b365.html) |
| **B360<br>( 2018 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `12` làn **PCIe** )<br>- Hỗ trợ tối đa `12` luồng **USB 3.1/2.0** ( tối đa `6` luồng **USB 3.1** )<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Tích hợp **Wireless-AC ( Wifi 5 )**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/b360.html) |
| **B250<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `12` làn **PCIe** )<br>- Hỗ trợ tối đa `12` luồng **USB 3.0/2.0** ( tối đa `6` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ công nghệ **Intel Optane**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/b250.html) |
| **B150<br>( 2015 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `8` làn **PCIe** )<br>- Hỗ trợ tối đa `12` luồng **USB 3.0/2.0** ( tối đa `6` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/b150.html) |
| **Z390<br>( 2018 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `24` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.1/2.0** ( tối đa `10` luồng **USB 3.1** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Tích hợp **Wireless-AC ( Wifi 5 )**<br>- Hỗ trợ **ép xung**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/z390.html) |
| **Z370<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `24` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `10` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Hỗ trợ **ép xung**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/z370.html) |
| **Z270<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `24` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `10` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID 0,1,5,10**<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Hỗ trợ **ép xung**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/z270.html) |
| **Z170<br>( 2015 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `20` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `10` luồng **USB 3.0** )<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID 0,1,5,10**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/z170.html) |
| **X299<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `24` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `10` luồng **USB 3.0** )<br>- Hỗ trợ `8` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID 0,1,5,10**<br>- Hỗ trợ công nghệ **Intel Optane**<br>- Hỗ trợ **ép xung**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/x299.html) |
| **X99<br>( 2014 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `8` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `6` luồng **USB 3.0** )<br>- Hỗ trợ `10` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID RST 14**<br>[Details](https://www.intel.vn/content/www/vn/vi/products/chipsets/desktop-chipsets/x99.html) |
| **C242<br>( 2018 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `10` làn **PCIe** )<br>- Hỗ trợ tối đa `12` luồng **USB 3.1**<br>- Hỗ trợ `6` cổng **SATA** tốc độ `6Gb/s`<br>[Details](https://www.intel.com/content/www/us/en/products/chipsets/server-chipsets/c242.html) |
| **C621<br>( 2017 )** | - Hỗ trợ **PCIe 3.0** ( tối đa `20` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `10` luồng **USB 3.0** )<br>- Hỗ trợ `14` cổng **SATA** tốc độ `6Gb/s`<br>- Tích hợp `5` luồng **LAN**<br>- Hỗ trợ công nghệ **Intel vPro**<br>[Details](https://www.intel.com/content/www/us/en/products/chipsets/server-chipsets/c621.html) |
| **C612<br>( 2014 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `8` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 3.0/2.0** ( tối đa `6` luồng **USB 3.0** )<br>- Hỗ trợ `10` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ **RAID RSTe 4.0**<br>- Hỗ trợ công nghệ **Intel vPro**<br>[Details](https://www.intel.com/content/www/us/en/products/chipsets/server-chipsets/c612.html) |
| **C602<br>( 2012 )** | - Hỗ trợ **PCIe 2.0** ( tối đa `14` làn **PCIe** )<br>- Hỗ trợ tối đa `14` luồng **USB 2.0**<br>- Hỗ trợ `2` cổng **SATA** tốc độ `6Gb/s`<br>- Hỗ trợ công nghệ **Intel vPro**<br>[Details](https://www.intel.com/content/www/us/en/products/chipsets/server-chipsets/c602.html) |
## **2) Chipset AMD**

| **Tên chipset** | <center>**Tính năng đi kèm**</center> |
|-----------------|----------------------|
| **B450** | | |
| **B350** | | |
| **A320** | | |
| **X370** | | |
| **X470** | | |

## **3) Các công nghệ tích hợp trên Chipset**