# Đóng góp cho Codepro

Chọn đúng kho: Codepro-Web cho website/API/máy chấm; Codepro-Client cho ứng dụng desktop.

## Báo lỗi

Cung cấp các bước tái hiện, kết quả mong đợi, kết quả thực tế và phiên bản đang dùng. Có thể đính kèm ảnh đã che thông tin riêng tư. Không đưa mật khẩu, token, cookie, dữ liệu người dùng hoặc testcase bí mật vào issue.

## Gửi thay đổi

1. Tạo nhánh cho một thay đổi cụ thể.
2. Làm theo quy ước của kho và cập nhật tài liệu liên quan.
3. Chạy kiểm tra phù hợp, ghi rõ kết quả trong pull request.
4. Mô tả vấn đề, cách khắc phục và đính kèm ảnh nếu thay đổi giao diện.

Web: `npm run lint`, `npm test` và các bài kiểm tra Python liên quan.
Client: `npm ci`, `npm test`; dùng `npm run dist:win` để đóng gói Windows.