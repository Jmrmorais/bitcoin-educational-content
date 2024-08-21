---
term: RICOCHET
---

Một kỹ thuật bao gồm việc thực hiện nhiều giao dịch giả mạo cho chính mình để mô phỏng việc chuyển quyền sở hữu của bitcoin. Ricochet được sử dụng để làm mờ các chi tiết có thể làm ảnh hưởng đến tính chất thay thế của một đồng Bitcoin. Ví dụ, nếu bạn thực hiện một coinjoin, đầu ra của bạn sẽ được nhận diện như vậy. Nhãn này của một "_đồng tiền từ coinjoin_" có thể ảnh hưởng đến tính chất thay thế của một UTXO. Các thực thể được quản lý, như các nền tảng giao dịch, có thể từ chối chấp nhận một UTXO đã trải qua coinjoin, hoặc thậm chí yêu cầu giải thích từ chủ sở hữu, với rủi ro bị chặn tài khoản hoặc đóng băng tài sản. Trong một số trường hợp, nền tảng có thể thậm chí báo cáo hành vi của bạn cho các cơ quan nhà nước. Đây là nơi phương pháp Ricochet được áp dụng. Để che giấu dấu vết để lại bởi coinjoin, Ricochet thực hiện bốn giao dịch liên tiếp nơi người dùng chuyển tiền của họ cho chính họ tại các địa chỉ khác nhau. Sau chuỗi giao dịch này, công cụ Ricochet cuối cùng chuyển bitcoin đến điểm đến cuối cùng của chúng, như một nền tảng giao dịch. Mục tiêu là tạo khoảng cách giữa giao dịch coinjoin ban đầu và hành động chi tiêu cuối cùng. Theo cách này, các công cụ phân tích chuỗi sẽ có khả năng giả định rằng đã có sự chuyển giao quyền sở hữu sau coinjoin, và do đó không cần thiết phải khởi xướng các hành động chống lại người phát hành. Trường hợp sử dụng phổ biến nhất cho Ricochet xảy ra khi cần thiết phải che giấu sự tham gia trước đó trong một coinjoin trên một UTXO, đặc biệt là để tránh bị nhắm mục tiêu bởi các chính sách AML/CTF của các nền tảng được quản lý hoặc danh sách đen. Công cụ Ricochet có sẵn trên Samourai Wallet.