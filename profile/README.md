<p align="center"><img src="https://raw.githubusercontent.com/Codepro-OJ/Codepro-Web/main/docs/branding/codepro-logo.png" alt="Codepro-OJ" width="220"></p>

# Codepro-OJ

Nền tảng luyện lập trình thi đấu và chấm bài, gồm website trực tuyến, ứng dụng Windows và hệ thống thi offline qua mạng LAN.

## Các kho mã

| Kho mã | Vai trò |
| --- | --- |
| [Codepro-Web](https://github.com/Codepro-OJ/Codepro-Web) | Website chính, Django API, quản trị, worker và hệ thống chấm bài trực tuyến |
| [Codepro-Client](https://github.com/Codepro-OJ/Codepro-Client) | Ứng dụng desktop Windows để đọc đề, viết mã và tham gia cuộc thi trên Codepro-Web |
| [Submit-Offline](https://github.com/Codepro-OJ/Submit-Offline) | OJ độc lập cho nhiều phòng thi qua LAN: web nộp bài, quản trị, cơ sở dữ liệu và Judge riêng |

## Dữ liệu và triển khai

- **Codepro-Web:** đề, testcase và gói kỳ thi được lưu ngoài repository. Máy chủ tải snapshot riêng tư từ S3/MinIO bằng lệnh `python manage.py sync_problem_data download`. Xem [hướng dẫn kho đề](https://github.com/Codepro-OJ/Codepro-Web/blob/main/docs/deployment/problem-data.md) và [hướng dẫn triển khai](https://github.com/Codepro-OJ/Codepro-Web/blob/main/docs/deployment/README.md).
- **Submit-Offline:** chuẩn bị đề, tài khoản và image chấm trước kỳ thi; khi thi, hệ thống hoạt động trên LAN mà không cần Internet. Mỗi tài khoản thí sinh chỉ có một phiên trên một máy; giám thị theo dõi phiên và nhận bản sao lưu thư mục bài làm. Xem [hướng dẫn vận hành](https://github.com/Codepro-OJ/Submit-Offline#readme).
- **Codepro-Client:** xem [hướng dẫn cài đặt và chạy](https://github.com/Codepro-OJ/Codepro-Client#readme).

Dữ liệu cuộc thi thật, testcase riêng tư, mật khẩu, khóa và bản sao lưu không được đưa vào Git.

## Đóng góp và báo lỗi

Đọc [hướng dẫn đóng góp](https://github.com/Codepro-OJ/.github/blob/main/CONTRIBUTING.md) trước khi mở pull request. Báo lỗi ở repository tương ứng: [Web](https://github.com/Codepro-OJ/Codepro-Web/issues), [Client](https://github.com/Codepro-OJ/Codepro-Client/issues), [Offline](https://github.com/Codepro-OJ/Submit-Offline/issues).
