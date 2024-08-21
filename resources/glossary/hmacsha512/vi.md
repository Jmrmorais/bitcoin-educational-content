`HMAC-SHA512` là viết tắt của "Hash-based Message Authentication Code - Secure Hash Algorithm 512". Đây là một thuật toán mật mã được sử dụng để xác minh tính toàn vẹn và tính xác thực của các thông điệp được trao đổi giữa hai bên. Nó kết hợp hàm băm mật mã `SHA512` với một khóa bí mật chung để tạo ra một Mã Xác Thực Thông Điệp (MAC) duy nhất cho mỗi thông điệp.

Trong bối cảnh của Bitcoin, việc sử dụng `HMAC-SHA512` có một chút khác biệt. Thuật toán này được sử dụng trong quá trình phái sinh xác định và phân cấp của cây khóa mật mã của một ví. `HMAC-SHA512` đặc biệt được sử dụng để chuyển từ hạt giống đến khóa chính, và sau đó cho mỗi quá trình phái sinh từ một cặp cha mẹ sang các cặp con. Thuật toán này cũng được tìm thấy trong một thuật toán phái sinh khác có tên là `PBKDF2`, được sử dụng để chuyển từ cụm từ khôi phục và cụm từ mật khẩu sang hạt giống.