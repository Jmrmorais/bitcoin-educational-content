---
term: BIP47
---

Được Justus Ranvier đề xuất vào năm 2015, giao thức này nhằm giải quyết vấn đề nghiêm trọng về việc tái sử dụng địa chỉ Bitcoin, một thực hành làm suy giảm nghiêm trọng quyền riêng tư của người dùng trên hệ thống. Satoshi Nakamoto, trong Bản Trắng Bitcoin, đã nhấn mạnh tầm quan trọng của việc sử dụng các cặp khóa riêng biệt cho mỗi giao dịch để duy trì sự tách biệt trong các hành động khác nhau của người dùng. BIP47 giới thiệu khái niệm về mã thanh toán có thể tái sử dụng, cho phép người dùng nhận nhiều khoản thanh toán mà không cần phải tạo ra một địa chỉ Bitcoin mới cho mỗi giao dịch. Những mã này hoạt động như các bộ nhận dạng ảo, được suy ra từ hạt giống ví của người dùng và nằm ở cấp độ tài khoản trong cấu trúc phát sinh của một ví HD. Từ sự kết hợp của mã thanh toán của cả hai bên, mỗi bên có thể suy ra một số lượng lớn địa chỉ duy nhất thuộc về bên kia, mà không cần phải liên lạc lại với họ. Cốt lõi của giao thức này dựa trên thuật toán ECDH (*Elliptic-Curve Diffie-Hellman*), một biến thể của sự trao đổi khóa Diffie-Hellman được thiết lập trên các đường cong elliptic, cho phép cả hai bên thiết lập một bí mật chung để tạo ra các địa chỉ nhận duy nhất. Mặc dù BIP47 chưa được thêm vào Bitcoin Core và đã nhận được phản ứng trái chiều từ cộng đồng, các triển khai như PayNym trên Samourai Wallet và Sparrow Wallet đã áp dụng nó và hoàn toàn tích hợp vào hệ sinh thái công cụ bảo mật của họ.