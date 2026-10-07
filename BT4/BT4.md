# ***bài 4 Quản lý đường dẫn trong hệ thống tệp*** 

# **Phần 1: Phân tích và đề xuất**

            **Tính di động (Portability):** Cao. Không phụ thuộc vào tên User, ổ đĩa hay vị trí tuyệt         đối của thư mục Project. Chỉ cần giữ nguyên cấu trúc thư mục.

**Độ dài câu lệnh:** Ngắn gọn hơn, dễ viết và dễ quản lý trong Script.

**Tính an toàn:** Tốt hơn vì không chứa tên tài khoản Windows hoặc đường dẫn riêng của máy tính.

**Ưu điểm:** Phù hợp khi chia sẻ Project cho nhiều người hoặc chạy Script trên nhiều máy tính khác nhau.

**Nhược điểm:** Phải xác định đúng thư mục hiện tại của chương trình. Nếu vị trí chạy chương trình thay đổi thì đường dẫn tương đối có thể không còn chính xác.

 **Phần 2: Lựa chọn**

An nên chọn Cách  – Relative Path:

../Data/users.csv

Vì cách này không phụ thuộc vào tên User, ổ đĩa hay vị trí cài đặt của máy tính. Khi gửi cả thư mục Project cho người khác, chương trình vẫn có thể chạy nếu giữ nguyên cấu trúc thư mục.

thư mục hiện tại.

thư mục cha.

Trong `../Data/users.csv`, `..` nghĩa là đi lên một thư mục từ `src`, sau đó vào thư mục `Data` để lấy file `users.cs`

