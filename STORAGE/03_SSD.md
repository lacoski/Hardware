# SSD - Solid State Drive
## **1) Khái niệm**
- **SSD ( Solid State Drive )** là một loại ổ cứng thể rắn có cấu tạo và nguyên lý hoạt động tương tự như bộ nhớ RAM hay các loại thẻ nhớ , **USB** đó là sử dụng các chip nhớ **flash** .
- **SSD** được tạo ra nhằm cạnh tranh với các ổ cứng **HDD** truyền thống , cải thiện về sức mạnh tốc độ , nhiệt độ , độ an toàn dữ liệu , điện năng tiêu thụ cũng như kích thước nhỏ gọn hơn .
## **2) Cấu tạo SSD**
- **SSD** là sự kết hợp của ba thành phần chính : **vi mạch điều khiển** , chip **DRAM** và bộ nhớ **flash NAND** . Trong đó , thành phần quan trọng quyết định hiệu suất của ổ cứng **SSD** là **Flash NAND** và **vi mạch điều khiển ( Controller )** .

    <img src=https://i.imgur.com/5CJytPd.png>

- Cấu tạo của **Flash NAND** trên ổ cứng **SSD** gồm nhiều **bóng bán dẫn** ( **transitor** ) . Được thiết kế để có thể giữ nguyên trạng thái khi không cấp nguồn .
## **3) Cấu trúc Flash NAND trên ổ cứng SSD**

<p align=center><img src=https://i.imgur.com/D6dPsvJ.png width=70%></p>

- Cấu trúc **NAND** được chia theo mô hình lưới :
    - **Die** : là tấm bán dẫn màu đen ( có thể nhìn thấy )
    - **Plane** : 1 **die** chứa một đến hai **plane** . Các **plane** có thể ( nói chung ) thực hiện các hoạt động giống hệt nhau cùng nhau .
    - **Block** : các **plane** chứa 1 số lượng **block** khác nhau.  Các ô **Flash NAND** chỉ có thể bị xóa ở cấp độ **block** .
    - **Page** : các **block** thường chứa khoảng `128 ` **page** . các **page** là các đơn vị nhỏ nhất có thể được lập trình ( hoặc viết thành ) . Mỗi **page** bao gồm `512` - `4096 bytes`
    - **Cell** : trong **page** có nhiều **cell** . Mỗi **cell** nắm giữ `1` - `4 bytes` tùy vào công nghệ **NAND** được **SSD** sử dụng .
>  Để tăng kích thước ổ cứng **SSD** nhà sản xuất thường tăng kích thước của **page** và **block**
## **4) Các công nghệ NAND**
- Có 4 công nghệ **NAND** trên ổ cứng **SSD** hiện đang sử dụng **SLC** , **MLC** , **TLC** và **QLC** . Sự khác nhau giữa các công nghệ này là mật độ bit dữ liệu chứa trong các chip nhớ , độ trễ và độ bền dựa theo chu kì ghi xóa ( **P/E cycle - Program-erase** ) .

    <img src=https://i.imgur.com/KACOI3U.jpg>

### **4.1) SLC - single level cell**
- Là công nghệ **NAND** đầu tiên .
- Chỉ chứa `1 bit` dữ liệu ( `0` hoặc `1` ) mỗi **cell** .
- Có độ trễ thấp nhất .
- Độ bền đạt đến **`100.000` P/E cycle**
- Thường sử dụng trong hệ thống lưu trữ , các máy chủ.
### **4.2) MLC - multi level cell**
- Chứa `2 bit` dữ liệu mỗi **cell**
- Chu kì ghi xóa khoảng **`10.000` P/E cycle**
- Thường dùng cho các PC và Laptop
### **4.3) TLC - triple-level cell**
- Chứa `3 bit` dữ liệu mỗi **cell**
- Chu kì ghi xóa khoảng **`3.000` P/E cycle**
- Độ tin cậy thấp .
- Độ trễ cao hơn nhiều so với **SLC** và **MLC** .
### **4.4) QLC - quad-level cell**
- Là công nghệ cao nhất được ứng dụng trong sản xuất ổ cứng **SSD** hiện nay ( **`2018`** ) .
- Chứa `4 bit` dữ liệu mỗi **cell**
- Chu kì ghi xóa khoảng **`1.000` P/E cycle**
- Thường được sử dụng để lưu trữ dữ liệu 
> ### **So Sánh**
- Mật độ bit dữ liệu ( **Density** ): **SLC** < **MLC** < **TLC** < **QLC**
- Dung lượng ( **Capacity** ) : **SLC** < **MLC** < **TLC** < **QLC**
- Tốc độ ghi dữ liệu ( **Writing Speed** ) : **SLC** > **MLC** > **TLC** > **QLC**
- Độ bền ( **Endurance** ) : **SLC** > **MLC** > **TLC** > **QLC**
- Độ tin cậy ( **Reability** ) : **SLC** > **MLC** > **TLC** > **QLC**
- Giá thành  ( **Cost** ) : **SLC** > **MLC** > **TLC** > **QLC**
## **5) Các khái niệm khác**
### **5.1) SSD TRIM**
- **TRIM** là một công nghệ cho phép cải thiện tốc độ ghi và độc dữ liệu trên ổ **SSD** , tương tự như **HDD Defragment** . Các ổ **SSD** hỗ trợ **TRIM** sẽ cải thiện được tốc độ đọc và ghi dữ liệu tốt hơn và đặc biệt là nhanh hơn rất nhiều lần so với ổ truyền thống .
- Sau một thời gian dài sử dụng , hiệu suất của **SSD** sẽ suy giảm dần là bởi vì các bộ nhớ **NAND Flash** không thể ghi đè dữ liệu . Điều đó có nghĩa là muốn ghi lại vào **page** đó thì **chip điều khiển** phải xóa dữ liệu đã ghi trong **page** đó và khi ghi dữ liệu mới, **chip điều khiển** cũng đồng thời xóa đi các dữ liệu muốn xóa, gọi là quá trình *"gom dữ liệu bỏ đi"* .
- **VD** :
    - Các **pages** trên **SSD** không chứa dữ liệu .
    - Người dùng ghi dữ liệu vào các page
    - Khi người dùng xóa dữ liệu :
        - **Page** sẽ được đánh dấu “***not in use***” bởi hệ điều hành .
        - Lúc này , dữ liệu vẫn còn lưu trên **SSD** vì **Controller** đã sao chép toàn bộ nội dung các **page** trong cùng một **block** vào bộ nhớ đệm ( **cache** ) .
    - **Controller SSD** loại bỏ các page “***invalid***” dựa vào thông tin các lệnh TRIM cung cấp .
    - Dữ liệu được ghi trở lại vào các **cell** trên **SSD** và các **page** “***invalid***” lúc này đã được làm trống để ghi dữ cho lần kế tiếp .

### **5.2) Write Amplification**
- Dùng để chỉ sự chênh lệch giữa lượng dữ liệu ghi trên các page vật lý so với dữ liệu cần ghi thực sự .
- **VD :**
    - Khi bạn muốn thay đổi một tin tin văn bản `4Kb` nhiều lần thì vị trí các block chứa dữ liệu sẽ được cập nhập và ghi nội dung mới . Như vậy , sau khi cập nhập nhiều làn file có dung lượng 4Kb có thể tăng lên thành `4 MB` .
    - Nhưng nhờ vào quá trình **gagbage collection** và **TRIM** nên hiện tượng **write amplification** được giảm thiểu . Điều này giúp các **block** không bị phần mảnh , tăng tốc độ truy xuất và giảm thiểu dung lượng lưu trữ lãng phí .
### **5.3) Wear Leveling**
- **Wear leveling** là thuật toán đặc biệt giúp tăng tuổi thọ và độ ổn định cho **SSD** bằng việc phân bổ dữ liệu ghi lên toàn bộ **transistor** của **NAND flash** một cách đồng đều .
- Điều này giúp mức độ hao mòn trên các **transistor** là như nhau và tránh một số **page** bị ghi quá nhiều lần .<br>
=>> **SSD** có dung lượng càng lớn thì tuổi thọ càng cao vì có số lượng **transistor** lớn và tất cả các **transistor** đều được ghi qua một lượt trước khi bắt đầu chu kì ghi xóa mới .
- Tuy nhiên **wear leveling** cũng làm tăng hiện tượng **write amplification** . Bởi vì để phân bổ việc ghi đều khắp các **page SSD** , thỉnh thoảng **wear leveling** cần phải ghi và xóa một số **block** nào đó mặc dù nội dung lưu trữ không thay đổi .
### **5.4) TBW / DTBW**
- Các nhà cung cấp thường cung cấp bảo hành **SSD** chỉ định số  lượng tối đa ổ đĩa được ghi toàn bộ mỗi ngày ( **DWPD** ) hoặc `terabyte` được ghi ( **TBW** )
- **DWPD - Drive Write Per Day** cho biết số lần bạn có thể ghi lên ổ đĩa toàn bộ dung lượng của nó mỗi ngày trong toàn bộ vòng đời của ổ . 
    - **VD :** ổ `200GB` và được bảo hành `5` năm .
        - Nếu **DWPD** là `1` nghĩa là mỗi ngày bạn có thể ghi `200GB` lên ổ đó trong `5` năm tới .
        - Nếu nhân ra, sẽ có được tổng số dung lượng ghi lên ổ này trước khi phải thay ổ :
            ```
            200GB mỗi ngày x 365 ngày/năm x 5 năm = 365TB
            ```
        - Nếu **DWPD** là `10` thì bạn có thể viết mỗi ngày `10` x `200GB` = `2TB` , tức là vòng đời cả 5 năm của nó sẽ ghi được `3650TB` = `2.65PB` .
- **TBW - Terabytes Written** cho biết dung lượng bạn có thể viết lên ổ đó trong suốt vòng đời của nó ( trước khi nó bị hỏng và mất dữ liệu )
    - **Theo VD trên :** 
        - Nếu hạn bảo hành là `5` năm , nghĩa là mỗi ngày sẽ ghi được :
            ```
            365TB / ( 5 năm x 365 ngày/năm ) = 200GB 
            ```
        - Mà ổ có kích thước `200GB` thì tương đương **DWPD** là `1` . Tương tự , nếu ổ có `3.65PBW` = `3.650TBW` thì mỗi ngày ghi được `2TB` , hay **DWPD** là `10` .
> Hai con số này dường như có thể quy ra nhau dễ dàng khi biết được dung lượng ổ và thời gian bảo hành.
## **2) Công nghệ 3D V-NAND**
- Trong bối cảnh chip nhớ **flash NAND 2D** phẳng đang tiến gần tới nhữn giới hạn vật lý , công nghệ **flash V-NAND 3D** là bước đột phá mới , cho phép cải thiện đáng kể dung lượng cũng như hiệu năng của ổ **SSD** .
- **3D V-NAND** , như tên gọi của nó , giúp tăng thêm nhiều lớp bóng bán dẫn để lưu dữ liệu . Bằng cách thêm vào nhiều lớp bóng bán dẫn , có thể lên tới `120` hoặc `144` lớp ( hiện tại vì các ổ **SSD** thông thường chỉ có `3-4` lớp bóng bán dẫn ), chúng ta có thể có gia tăng mật độ và dung lượng bộ nhớ lên đáng kể . Bên cạnh đó còn giúp gia tăng khoảng trống giữa các khối bộ nhớ trên mỗi lớp , giúp tránh phải các vấn đề về vật lí và hiệu năng bộ nhớ . Trên mỗi lớp bóng bán dẫn , các khối bộ nhớ cũng có thể sắp xếp theo dạng đơn cấp hoặc đa cấp như trên bộ nhớ  flash, qua đó có thể tăng dung lượng lên mức cực khủng nếu muốn .
- So với công nghệ **2D NAND Flash** , **3D V-NAND Flash** mang đến 4 ưu điểm dễ dàng nhận ra đó là: dung lượng lưu trữ lớn hơn, độ bên tốt hơn, hiệu năng cao hơn và tiết kiệm điện hơn.


