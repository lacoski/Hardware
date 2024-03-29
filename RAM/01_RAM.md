# RAM
## **1) Khái niệm**
- **RAM - Random Access Memory** ( bộ nhớ truy cập ngẫu nhiên ) chứa dữ liệu tạm thời và các lệnh xử lý cho **CPU** .
- Có 2 loại **RAM** :
    - **SRAM** - **RAM** tĩnh : được dùng cho bộ nhớ đệm trong **CPU** . **SRAM** có thể lưu trữ dữ liệu bao lâu cũng được , miễn là **SRAM** được cấp điện .
    - **DRAM** - **RAM** động : dữ liệu trong **DRAM** bị mất đi nhanh chóng và bộ điều khiển bộ nhớ phải ***refresh*** dữ liệu hàng nghìn lần mỗi giây . <br>=> Cả 2 loại đều bị mất dữ liệu khi không có điện , được gọi là *bộ nhớ khả biến* .
- **RAM** được lưu trữ trên các **module nhớ** , được cắm trên các khe **DIMM** trên **mainboard** .

    <img src=https://i.imgur.com/uKyll2j.jpg>

- Các loại **mainboard** hiện nay đều sử dụng **module nhớ DIMM** .
- **Laptop** sử dụng một phiên bản thu nhỏ của **DIMM** là **SO-DIMM - small outline DIMM** .
- Loại **MicroDIMM** được sử dụng trong các máy tính cỡ nhỏ . Đây là 1 **module nhớ** thu gọn của **SO-DIMM** .
- Hai loại **module nhớ** cũ là **RIMM** ( do Rambus thiết kế ) và **SIMM** đã không còn được sử dụng . Điểm khác biệt chính giữa các loại **module nhớ** này là độ rộng **bus** và cách thức di chuyển dữ liệu từ **system bus** tới **module nhớ** .
## **2) Các loại module nhớ dành cho Desktop**
### **2.1) SIMM ( *Single In-Line Memory Module* )**
- Ra đời năm **`1987`**
- **SIMM** **`30`** chân phải được lắp `4` thanh đồng thời :

    <p align=center><img src=https://i.imgur.com/YCj3FIw.png width=70%></p>

- **SIMM** **`72`** chân phải được lắp `2` thanh đồng thời :

    <p align=center><img src=https://i.imgur.com/KzTUeR6.gif width=70%></p>

### **2.2) RIMM ( *Rambus Inline Memory Module* )**
- Ra đời năm **`1999`**
- **RIMM** có **`184`** chân và 2 rãnh gần trung điểm của cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/dZ92pZw.jpg width=70%></p>

### **2.3) SDRAM ( *Synchronous Dynamic Random Access Memory* )**
- Ra đời năm **`1997`**
- Thanh **SDRAM** **`168`** chân có 2 rãnh . Vị trí của những rãnh này tùy thuộc vào các đặc điểm bộ nhớ mà **DIMM** sử dụng :

    <p align=center><img src=https://i.imgur.com/3NJhO63.gif width=70%></p>

### **2.4) DDR ( *Double Data Rate* )**
#### **2.4.1) DDR** :
- Ra đời năm **`2000`**
- Thanh **DDR** **`184`** chân có thể hỗ trợ ***dual-channel*** hoặc lắp đặt như 1 thanh **DIMM** đơn . Có 1 rãnh ở cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/eR1poL7.png width=70%></p>

#### **2.4.2) DDR2** :
- Ra đời năm **`2004`**
- Thanh **DDR2** **`240`** chân có thể hỗ trợ ***dual-channel*** hoặc có thể được lắp đặt như 1 thanh **DIMM** đơn . Có 1 rãnh nằm gần trung điểm cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/CrveCG9.png width=70%></p>

#### **2.4.3) DDR3** :
- Ra đời năm **`2007`**
- Thanh **DDR3** **`240`** chân có thể hỗ trợ ***quad-channel , triple-channel , dual-channel*** hoặc được lắp đặt như 1 thanh **DIMM** đơn . Nó có 1 rãnh nằm xa trung điểm hơn **DDR2** :

    <p align=center><img src=https://i.imgur.com/AhoMZ8i.png width=70%></p>

#### **2.4.4) DDR4** :
- Ra đời năm **`2014`**
- Hiện tại , **DDR4**  **`288`** chân là loại **module nhớ** có tốc độ nhanh nhất với điện áp yêu cầu thấp nhất . Hỗ trợ ***quad-channel , dual-channel*** hoặc có thể được lắp đặt như 1 thanh **DIMM** đơn . Nó có 1 rãnh gần trung điểm của cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/8EuDRTh.png width=70%></p>

## **3) Các loại module nhớ dành cho Laptop**
- Hiện nay , laptop sử dụng **DDR4** , **DDR3L** , **DDR3** hoặc **DDR2 SO-DIMM** . Tất cả đều có kích cỡ nhỏ hơn **DIMM** .
### **3.1) SO-RIMM**
- Thanh **SO-RIMM** **`160`** chân sử dụng chip nhớ của Rambus và có 2 khứa ( ***notch*** ) .

    <p align=center><img src=https://i.imgur.com/XYxi7IF.png width=60%></p>

### **3.2) SO-DIMM**
- Thanh **SO-DIMM** **`72`** chân và không có khứa .

    <p align=center><img src=https://i.imgur.com/a08MAP2.png width=60%></p>

### **3.3) SDRAM SO-DIMM**
- Thanh **SO-DIMM** sử dụng **SDRAM** có **`144`** chân và có 1 khứa nhỏ ở giữa cạnh tiếp xúc .

    <p align=center><img src=https://i.imgur.com/GxTargU.gif width=60%></p>

### **3.4) DDR SDRAM SO-DIMM**
#### **3.4.1) DDR**
- Thanh **DDR SO-DIMM** **`200`** chân và có 1 khứa ở gần rìa của cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/IFnsFAx.png width=60%></p>

#### **3.4.2) DDR2**
- Thanh **DDR2 SO-DIMM** **`200`** chân và có 1 khứa ở gần rìa cạnh tiếp xúc ( của **DDR** gần hơn ) :

    <p align=center><img src=https://i.imgur.com/uKC5Rbm.png width=60%></p>

#### **3.4.3) DDR3 vs DDR3L**
- Thanh **DDR3/DDR3L SO-DIMM** **`204`** chân và có 1 khứa ở gần giữa cạnh tiếp xúc . **DDR3L** tiết kiệm điện hơn **DDR3** .

    <p align=center><img src=https://i.imgur.com/9sofZwx.png width=60%></p>

#### **3.4.5) DDR4**
- Thanh **DDR4 SO-DIMM** **`260`** chân và có 1 khứa ở gần giữa cạnh tiếp xúc :

    <p align=center><img src=https://i.imgur.com/uKU4gky.png width=60%></p>
