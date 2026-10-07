***Phần 1:  Các lỗi sai của Nam***  
Lỗi 1: tên thư mục có khoảng trống và không đặt trong dấu ngoặc kép   
Lỗi 2: tạo thư mục con trong khi đó thư mục cha src chưa tồn tại  
Lỗi 3: sao chép src khi lệnh tạo src trước đó đã thất bại

***Phần 2: Hoàn thiện***  
**PS C:\\Student\>**     mkdir "Shopee Projects"  
**PS C:\\Student\>**     cd "Shopee Projects"  
**PS C:\\Student\>**      mkdir "src\\assets\\images" \-Force; Copy-Item src \-Destination src-backup \-Recurse

