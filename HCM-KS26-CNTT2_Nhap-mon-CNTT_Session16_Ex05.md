**Bài 5 : Tối ưu tiện ích mở rộng cho hệ thống điều phối vận tải** 

**Phần 1\. Phân tích** 

\-JSON Viewer chuyển đổi chuỗi dữ liệu API thô chứa tọa độ GPS thành cấu trúc cây phân cấp và tô màu cú pháp (syntax highlighting). Việc này giúp kỹ sư đọc nhanh, phát hiện lỗi, thiếu sót mảng dữ liệu ngay trên trình duyệt, giúp tiết kiệm thời gian phân tích log API thô, đẩy nhanh tốc độ xử lý sự cố cho hệ thống điều phối

**Phần 2\. Triển khai**

**1\. Phân loại 5 tiện ích (Extensions) thiết yếu**

- Nhóm Dev Suite (Xử lý dữ liệu API):  
+ JSON Formatter: Tự động sắp xếp chuỗi dữ liệu GPS ngoằn ngoèo thành dạng cây đẹp mắt, rõ ràng để dễ đọc.  
    
- Nhóm Productivity (Hỗ trợ đồ họa / UI):  
+ ColorZilla: Công cụ "chấm hút màu" siêu nhẹ, bấm vào điểm bất kỳ trên bản đồ là lấy được ngay mã màu chính xác.  
+ WhatFont: công cụ soi phông chữ (font-size, line-height, font-height,..)  
    
- Nhóm Security (Bảo mật & Tốc độ):  
+ uBlock Origin: Chặn quảng cáo và mã độc cực hiệu quả, tiết kiệm RAM giúp web không bị lag.  
+ Privacy Badger: Tự động phát hiện và chặn các đoạn mã theo dõi ẩn của bên thứ ba.

**Chức năng 2 (Phân quyền)**

Thiết lập Site Access (On click) bảo mật dữ liệu
Để ngăn các extension tự động đọc dữ liệu GPS nhạy cảm trên mọi trang web:

Nhấp chuột phải vào biểu tượng của extension trên Toolbar (hoặc vào chrome://extensions).

Chọn Quyền truy cập trang web (Site Access).

Chuyển thiết lập sang chế độ Khi nhấp vào (On click).

**Phần 3\. Kiểm thử**

+ Mở Task Manager: nhấn Shift \+ Esc ngay trên Google Chorme để mở Task Manager riêng của Google Chorme  
+ Xác định thủ phạm làm tốn RAM: xem cột Memory footprint để tìm Extension đang tiêu thụ nhiều RAM làm chậm trình duyệt khi tải trang.  
+ Vô hiệu hóa và kiểm tra lại: Truy cập chrome://extensions, gạt công tắc tắt đối với tiện ích đang tốn quá nhiều tài nguyên. Nhấn Ctrl \+ F5 để lấy phiên bản mới . Nhìn biểu đồ Waterfall thấy nạp nhanh chóng và hết lag thì vấn đề đã được khắc phục.

