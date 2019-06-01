# Hoạt động của CPU

<img src=https://i.imgur.com/dVweEqm.png>

- **CPU** bao gồm 5 thành phần chính :
    - **ALU - Arimetic Logic Unit** : thực hiện các phép tính toán như cộng , trừ , nhân ...  và các phép logic như đúng sai . **ALU** giữ vai trò tính toán trong **CPU** .
    - **CU - Control Unit** : điều khiển các câu lệnh – tập lệnh của hệ thống . Chứa khối giải mã ( cho phép giải mã các lệnh và xác định thao tác mà lệnh đang yêu cầu ) , logic và xung nhịp ( đồng bộ hóa các thao tác xử lý của CPU trong 1 khoảng thời gian nhất định ) . Hơn thế **CU** cho phép nhận tín hiệu từ **System Bus** , giải quyết và đáp ứng yêu cầu đó .
    - **Registry Array** ( *thanh ghi* ) : bộ nhớ đệm bên trong **CPU** . Bộ nhớ này có dung lượng nhỏ , tốc độ truy cập cao cho phép CPU lưu trữ tạm thời các hạng toán , kết quả v…v… Bao gồm : Bộ đếm chương trình ( chứa các lệnh tiếp theo để xử lý ) , thanh ghi lệnh ( chứa các lệnh đang xử lý), thanh ghi địa chỉ bộ nhớ , thanh ghi AX ( lưu trữ dữ liệu của bộ nhớ ) , thanh ghi chỉ dẫn .
    - **System Bus** : Bus hệ thống cho phép chuyển dữ liệu giữa các thành phần trong hệ thống . Bao gồm 3 loại Bus chính : Bus địa chỉ ( lưu trữ địa chỉ các bộ nhớ , các cổng vào ra của thiết bị ngoại vi v…v… cho phép CPU gửi hoặc nhận dữ liệu từ các thiết bị này), Bus dữ liệu (cho phép truyền dữ liệu), Bus điều khiển ( Bus điều khiển phục vụ truyền tải các thông tin dữ liệu để điều khiển hoạt động của hệ thống )
    - **Memory** : bộ nhớ thực không cấu trúc thành phần cứng của CPU mà được đặt trên Main , nhưng do các phương thức thực thi câu lệnh + lưu trữ thông tin nằm trong bộ nhớ nên nó cũng là một thành phần quan trọng trong việc thực thi chương trình . 
