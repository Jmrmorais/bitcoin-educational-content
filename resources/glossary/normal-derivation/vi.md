---
term: NORMAL DERIVATION
---

Quá trình tạo ra các khóa con trong ví HD. Normal derivation sử dụng khóa công khai của cha mẹ làm đầu vào cho hàm `HMAC-SHA512`, cho phép tạo ra các khóa công khai con từ khóa công khai của cha mẹ và mã chuỗi của cha mẹ. Quá trình này bao gồm việc nối khóa công khai của cha mẹ và một chỉ số nhỏ hơn $2^{31}$, tiếp theo là áp dụng `HMAC-SHA512` với mã chuỗi của cha mẹ. Kết quả được chia thành hai phần: 256 bit đầu tiên được cộng vào khóa riêng tư của cha mẹ để thu được khóa riêng tư của con, trong khi 256 bit còn lại tạo thành mã chuỗi của con. Phương pháp này đảm bảo rằng khóa công khai mở rộng có thể được sử dụng để tạo ra các khóa công khai con. Trong quá trình derivation chuẩn, normal derivation được sử dụng ở tất cả các cấp độ derivation từ độ sâu tài khoản. Trong ký hiệu của đường dẫn derivation, một normal derivation được xác định khi chỉ có chỉ số mà không có dấu nháy đơn `'`.