# Kiểm chứng phân quyền Triage trên GitHub

**Mục đích:** tạo Pull Request thử nghiệm để kiểm tra rằng Sinh viên C (`@ttbqb1st`) có quyền Triage nhưng không được phép merge vào nhánh `main`.

## Phân quyền dự kiến

| Tài khoản | Vai trò | Quyền trên repository |
|---|---|---|
| `@shun2195` | Sinh viên A – Project Lead | Admin |
| `@ttoannp` | Sinh viên B – Core Maintainer | Write |
| `@ttbqb1st` | Sinh viên C – Triager | Triage |

## Các bước kiểm thử thủ công bằng tài khoản C

1. Đăng nhập GitHub bằng tài khoản `ttbqb1st` (không phải `shun2195` hoặc `ttoannp`).
2. Mở Pull Request kiểm thử này và xem các tab **Conversation** và **Files changed**.
3. Cuộn xuống cuối trang **Conversation** để kiểm tra vùng gộp PR.
4. Xác nhận tài khoản C **không có nút Merge pull request khả dụng** (nút có thể bị vô hiệu hóa hoặc không hiển thị tùy giao diện).
5. Chụp ảnh màn hình có thể nhìn thấy tài khoản đang đăng nhập, địa chỉ PR, trạng thái Open và vùng Merge.
6. Không bấm merge bằng tài khoản Admin/Write trong lúc kiểm tra.

**Kết quả mong đợi:** C có thể đọc và tham gia sàng lọc thảo luận, nhưng không thể gộp PR do thiếu quyền Write.

**Trạng thái:** Chưa kiểm chứng bằng phiên đăng nhập của tài khoản C. PR này là minh chứng phân quyền, không thay đổi logic ứng dụng và được giữ **Open** cho đến khi chụp ảnh xong.
