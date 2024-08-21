---
term: BITVM
---

Protocol được giới thiệu bởi Robin Linus vào năm 2023, nhằm mở rộng khả năng phát triển ứng dụng của Bitcoin. BitVM cho phép thực hiện bất kỳ hoạt động tính toán nào một cách tùy ý và sử dụng tính toán này để điều khiển các bitcoin liên quan. Protocol này di chuyển tất cả các tính toán ra khỏi chuỗi (off-chain) trong khi vẫn cho phép việc tranh chấp tính toán trên chuỗi (on-chain) nếu bên kia tuyên bố kết quả gian lận. Như vậy, BitVM cung cấp cho Bitcoin khả năng tính toán gần như Turing-complete, mà không yêu cầu bất kỳ sửa đổi nào ở cấp độ đồng thuận. BitVM tái tạo hành vi của cổng logic `NAND` thông qua việc sử dụng kết hợp các opcode `OP_BOOLAND` (tái tạo hành vi của cổng logic `AND`) và `OP_NOT` (tái tạo hành vi của cổng logic `NOT`). Thực tế, cổng logic `NAND` này có thể được sử dụng trong chuỗi để tái tạo hành vi của tất cả các cổng logic khác hiện có. Đây là những gì được gọi là "cổng vạn năng". Theo cách mở rộng, một chuỗi các cổng logic `NAND` có thể do đó tái tạo bất kỳ mạch tính toán nào. Ý tưởng với BitVM là lưu trữ những chuỗi tính toán `NAND` này như là lá trong MAST của một giao dịch Taproot.