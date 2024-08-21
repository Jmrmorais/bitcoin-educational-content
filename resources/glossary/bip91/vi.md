---
term: BIP91
---

Đề xuất bởi James Hilliard (kỹ sư tại Bitmain) nhằm tạo điều kiện cho việc kích hoạt bản cập nhật SegWit thông qua một soft fork, được định nghĩa trong BIP141, BIP143, và BIP147, thông qua một MASF mà không cần đạt ngưỡng yêu cầu 95% sức mạnh tính toán báo hiệu hỗ trợ qua bit 1. BIP91 cho phép các thợ đào gián tiếp báo hiệu sự hỗ trợ của họ cho SegWit bằng cách sử dụng bit 4 trong các khối đã khai thác. Một khi 269 khối trong một cửa sổ của 336 khối đã bao gồm bit 4 (tức là, 80% sức mạnh tính toán), BIP91 được khóa lại, sau đó buộc tất cả các nút tương thích phải từ chối các khối không bao gồm bit 1. Phương pháp này nhằm mục đích làm cho BIP148 (UASF) trở nên lỗi thời và tránh một sự chia rẽ tiềm ẩn của blockchain vào ngày 1 tháng 8 năm 2017. BIP91 cuối cùng đã được kích hoạt vào ngày 23 tháng 7 năm 2017 (tại khối 477,120), ngay trước ngày quan trọng 1 tháng 8 được đặt ra trong BIP148. Điều này buộc các thợ đào phải báo hiệu cho SegWit, cuối cùng đã được khóa vào ngày 9 tháng 8 tại khối 479,808, và sau đó được kích hoạt vào ngày 24 tháng 8 tại khối 481,824. Tóm lại, BIP148 (UASF) được tạo ra như một phản ứng đối với việc các thợ đào không báo hiệu đủ cho SegWit, nhưng cuối cùng không bao giờ được thực hiện. BIP91 (MASF) được tạo ra để đáp lại BIP148 nhằm buộc tay các thợ đào, mà không gặp rủi ro từ UASF của BIP148. BIP91 bản thân đại diện cho một soft fork, cuối cùng sẽ buộc các thợ đào phải khóa SegWit thông qua phương pháp cơ bản (MASF BIP9).