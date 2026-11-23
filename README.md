# MNM OSS Governance Lab

Repository thực hành môn Mạng máy tính nâng cao – chủ đề **Quản trị dự án và vận hành cộng đồng OSS**.

## Mục tiêu

- Thiết kế Contributor Ladder và quy chế quản trị minh bạch.
- Thực hành phân quyền theo nguyên tắc least privilege.
- Soạn thảo RFC và vận hành Lazy Consensus.
- Chuẩn hóa Issue Labels và tự động hóa Issue Triage bằng GitHub Actions.
- Xây dựng Roadmap, danh sách Maintainers và phương án kế thừa.
- Phân tích tình huống Code of Conduct và nguy cơ Hard Fork.

## Thành viên và vai trò

| GitHub | Vai trò trong bài lab | Quyền GitHub mục tiêu |
|---|---|---|
| [@shun2195](https://github.com/shun2195) | Sinh viên A – Project Lead / Steering Council | Admin |
| [@ttoannp](https://github.com/ttoannp) | Sinh viên B – Core Maintainer | Write |
| [@ttbqb1st](https://github.com/ttbqb1st) | Sinh viên C – Triager / Reviewer | Triage |

**Trạng thái cấu hình thực tế:** Repository đã được chuyển vào GitHub Organization `mnm-oss-team`. `@shun2195` là Organization Owner và có quyền Admin trên repository; `@ttoannp` đã có quyền Write; lời mời quyền Triage cho `@ttbqb1st` đã được gửi và đang chờ người nhận chấp nhận. Sau khi chấp nhận, quyền Triage sẽ có hiệu lực. Không cấp Write thay thế vì sẽ vượt quá quyền cần thiết.

## Cấu trúc

- `.github/GOVERNANCE.md`: mô hình quản trị và Contributor Ladder.
- `.github/workflows/issue-triage.yml`: tự động chào mừng và gắn nhãn Issue mới.
- `docs/rfc/RFC-0001.md`: đề xuất chuẩn hóa Structured JSON Logging.
- `ROADMAP.md`: lộ trình Now – Next – Later.
- `MAINTAINERS.md`: danh sách người bảo trì và chính sách kế thừa.
- `CODE_OF_CONDUCT.md`: chuẩn mực ứng xử cộng đồng.
- `CONTRIBUTING.md`: hướng dẫn đóng góp.
- `docs/CASE_STUDIES.md`: phương án xử lý hai tình huống thực chiến.

## Nguyên tắc làm việc

Mọi thay đổi kiến trúc lớn phải có RFC; mọi Pull Request cần review; mọi thành viên phải tuân thủ Code of Conduct. Quyền quản trị được cấp theo đóng góp và được rà soát định kỳ.
