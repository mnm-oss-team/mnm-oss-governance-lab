# HƯỚNG DẪN ĐÓNG GÓP

## Báo lỗi (Issue)

- Tìm Issue tương tự trước khi tạo mới.
- Cung cấp phiên bản, hệ điều hành, bước tái hiện, kết quả mong đợi và kết quả thực tế.
- Gỡ bỏ token, mật khẩu và dữ liệu cá nhân khỏi log trước khi đăng.

## Đề xuất tính năng hoặc thay đổi kiến trúc

- Thay đổi nhỏ có thể mở Issue/PR để thảo luận.
- Thay đổi kiến trúc, API hoặc hành vi phá vỡ tương thích phải có RFC trong `docs/rfc/`.
- RFC phải nêu động lực, thiết kế, phương án thay thế, rủi ro, kế hoạch kiểm thử và rollback.

## Pull Request

1. Tạo nhánh mô tả ngắn gọn, ví dụ `feat/json-logging`.
2. Viết test và cập nhật tài liệu liên quan.
3. Mô tả rõ thay đổi, liên kết Issue/RFC và ghi nhận breaking changes.
4. Chờ review; không tự merge PR của chính mình.
5. Chỉ merge khi CI đạt và các phản đối kỹ thuật đã được giải quyết.

## Quy tắc cộng đồng

Mọi người tham gia phải tuân thủ CODE_OF_CONDUCT.md. Maintainer có thể yêu cầu chỉnh sửa hoặc từ chối đóng góp không đáp ứng tiêu chuẩn chất lượng/an toàn.
