# **BÀI 3: KIẾN TRÚC SƯ HẠ TẦNG CLOUD SERVER**

## **1\. Các lệnh PowerShell thực hiện theo đúng thứ tự**

### **Bước 1: Tạo cấu trúc thư mục**

mkdir .\\Farm-Manager\\code\\app \-Force

 Tạo thư mục code\\app bên trong Farm-Manager.

mkdir .\\Farm-Manager\\database\\db \-Force

 Tạo thư mục database\\db.

mkdir .\\Farm-Manager\\logs\\guides \-Force

 Tạo thư mục logs\\guides.

Tham số \-Force giúp tạo thư mục và không báo lỗi nếu thư mục đã tồn tại.

### **Bước 2: Tạo 3 file rỗng trong thư mục app**

New-Item .\\Farm-Manager\\code\\app\\main.py \-ItemType File \-Force

 Tạo file main.py.

New-Item .\\Farm-Manager\\code\\app\\models.py \-ItemType File \-Force

Tạo file models.py.

New-Item .\\Farm-Manager\\code\\app\\utils.py \-ItemType File \-Force

 Tạo file utils.py.

### **Bước 3: Sao lưu toàn bộ thư mục logs**

Copy-Item .\\Farm-Manager\\logs \-Destination .\\Farm-Manager\\logs-backup \-Recurse \-Force

 Sao chép toàn bộ thư mục logs sang logs-backup, bao gồm cả thư mục con guides và các file bên trong.

\-Recurse: sao chép đệ quy toàn bộ thư mục con và file bên trong.

\-Force: cho phép sao chép/ghi đè các mục cần thiết mà không bị cản trở bởi thuộc tính thông thường.

## **2\. Kiểm tra kết quả**

Dùng lệnh:

ls .\\Farm-Manager  
Farm-Manager  
├── code  
│   └─ app  
│       ├── main.py  
│       ├─ models.py  
│       └── utils.py  
├── database  
│   └── db  
├── logs  
│   └── guides  
└─ logs-backup  
    └── guides

## **3\. Giải thích đường dẫn**

Các lệnh sử dụng:

.\\Farm-Manager\\...

đây là **đường dẫn tương đối**, nghĩa là PowerShell bắt đầu từ thư mục hiện tại rồi đi đến Farm-Manager.

