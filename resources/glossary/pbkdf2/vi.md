`PBKDF2` là viết tắt của *Password-Based Key Derivation Function 2* (Hàm Dẫn Xuất Khóa Dựa Trên Mật Khẩu 2). Đây là một phương pháp tạo ra khóa mật mã từ một mật khẩu sử dụng một hàm dẫn xuất. Nó nhận đầu vào là một mật khẩu, một giá trị muối mật mã, và lặp đi lặp lại áp dụng một hàm đã được xác định trước (thường là một hàm băm như `SHA256` hoặc một `HMAC`) lên những dữ liệu này. Quá trình này được lặp lại nhiều lần để tạo ra một khóa mật mã.

Trong bối cảnh của Bitcoin, `PBKDF2` được sử dụng kết hợp với hàm `HMAC-SHA512` để tạo ra hạt giống của một ví xác định và phân cấp (seed) từ một cụm từ khôi phục gồm 12 hoặc 24 từ. Giá trị muối mật mã được sử dụng trong trường hợp này là cụm từ mật khẩu BIP39, và số lần lặp là `2048`.