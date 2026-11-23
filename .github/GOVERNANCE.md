# QUY CHẾ QUẢN TRỊ DỰ ÁN (PROJECT GOVERNANCE)

## 1. Mô hình quản trị

Dự án vận hành theo mô hình **Consensus-Seeking kết hợp Meritocracy**:

- Consensus-Seeking: quyết định quan trọng được công khai thảo luận, tiếp nhận phản biện có căn cứ và ghi lại kết quả.
- Meritocracy: quyền hạn tăng theo đóng góp có chất lượng, năng lực review và mức độ tin cậy; không tự động phát sinh từ thâm niên hoặc quan hệ cá nhân.
- Least privilege: mỗi thành viên chỉ nhận quyền GitHub tối thiểu cần cho nhiệm vụ.
- Transparency: RFC, quyết định, lộ trình và tiêu chí thăng tiến được lưu công khai trong repository.

## 2. Vai trò hiện tại của nhóm thực hành

| Thành viên | Vai trò | Quyền GitHub mục tiêu | Trách nhiệm |
|---|---|---|---|
| @shun2195 | Project Lead / Steering Council – Sinh viên A | Admin | Quản trị repository, ban hành quy chế, xử lý tranh chấp CoC và quyết định phê duyệt cuối cùng |
| @ttoannp | Core Maintainer – Sinh viên B | Write | Code review, duy trì nhánh phát triển, kiểm tra chất lượng và theo dõi Roadmap |
| @ttbqb1st | Triager / Reviewer – Sinh viên C | Triage | Sàng lọc Issue, gắn nhãn, kiểm tra khả năng tái hiện và hỗ trợ Contributor mới |

**Trạng thái cấu hình thực tế:** Repository đã được chuyển vào Organization `mnm-oss-team`. @shun2195 là Organization Owner/Admin; @ttoannp đã có quyền Write; lời mời quyền Triage cho @ttbqb1st đang chờ chấp nhận. Quyền Triage có hiệu lực sau khi người nhận chấp nhận lời mời. Không tự ý cấp Write thay thế.

## 3. Bậc thang thăng tiến (Contributor Ladder)

### Cấp 1 – Community Contributor

- Điều kiện: có ít nhất 01 Pull Request được review và merge; đóng góp có thể là mã nguồn, tài liệu hoặc kiểm thử.
- Quyền: đọc repository, mở Issue/PR, tham gia thảo luận RFC.
- Trách nhiệm: tuân thủ CONTRIBUTING.md và CODE_OF_CONDUCT.md.

### Cấp 2 – Reviewer / Triager

- Điều kiện: tối thiểu 05 PR chất lượng; hỗ trợ giải đáp và tái hiện Issue thường xuyên trong ít nhất 30 ngày.
- Quyền: Triage – quản lý nhãn, phân loại, đóng/mở Issue và hỗ trợ điều phối.
- Không có quyền merge thay Maintainer.

### Cấp 3 – Core Maintainer

- Điều kiện: đóng góp bền bỉ ít nhất 03 tháng; hiểu kiến trúc; có đề cử từ một Maintainer và được Steering Council đồng thuận.
- Quyền: Write – push nhánh được phép, review/merge PR theo branch protection, quản lý release theo quy trình.
- Trách nhiệm: bảo đảm chất lượng, tương thích ngược và bảo mật.

### Cấp 4 – Steering Council

- Cơ cấu: 03 thành viên, nhiệm kỳ 01 năm; thành viên được bầu hoặc tái xác nhận công khai.
- Quyền: Admin – quản lý cấu hình repository, Secrets, quyền truy cập và quyết định quản trị đặc biệt.
- Admin không được dùng quyền kỹ thuật để bỏ qua quy trình review hoặc Code of Conduct.

## 4. Cơ chế ra quyết định – Lazy Consensus

1. Đề xuất phải được đăng dưới dạng RFC hoặc Issue có phạm vi, phương án, tác động và kế hoạch rollback.
2. Thời gian lấy ý kiến mặc định là **72 giờ** kể từ khi thông báo RFC đã sẵn sàng review.
3. Im lặng không đồng nghĩa với đồng ý tuyệt đối; nếu không có phản đối có căn cứ trong thời hạn, Maintainer có thể ghi nhận Lazy Consensus và tiến hành bước tiếp theo.
4. Phản đối `-1 (Veto)` phải nêu rủi ro kỹ thuật cụ thể, bằng chứng và điều kiện để giải quyết; không dùng veto chỉ vì sở thích cá nhân.
5. Tác giả phải phản hồi từng phản đối. Khi vấn đề được giải quyết, người phản đối cập nhật trạng thái; quyết định và lý do được ghi trong RFC/PR.
6. Thay đổi bảo mật, dữ liệu hoặc thay đổi phá vỡ tương thích có thể cần thời gian review dài hơn 72 giờ và phải được Steering Council xác nhận.

## 5. Code of Conduct và chế tài

Báo cáo vi phạm được tiếp nhận riêng tư bởi Project Lead hoặc người được ủy quyền. Nhóm bảo vệ người báo cáo, không công khai thông tin cá nhân, lưu bằng chứng cần thiết và đánh giá dựa trên hành vi.

Các mức xử lý tăng dần:

1. **Correction:** nhắc nhở riêng, yêu cầu dừng hành vi và giải thích tác động.
2. **Warning:** cảnh cáo chính thức, nêu rõ hành vi vi phạm và hậu quả nếu tái phạm.
3. **Temporary Ban:** tạm đình chỉ quyền tham gia trong thời hạn xác định.
4. **Permanent Ban:** chấm dứt quyền tham gia với vi phạm nghiêm trọng hoặc tái phạm.

Mức xử lý phụ thuộc mức độ, tần suất, tác động và thái độ khắc phục; có thể bỏ qua cấp trung gian nếu hành vi đặc biệt nghiêm trọng. Người bị xử lý có thể gửi yêu cầu xem xét lại tới thành viên Steering Council không tham gia quyết định ban đầu.

## 6. Emeritus Status và rà soát quyền

- Maintainer không hoạt động liên tục 06 tháng được đề nghị chuyển sang trạng thái Emeritus.
- Quyền Write/Admin được rà soát và có thể thu hồi; tên vẫn được ghi nhận trong lịch sử đóng góp.
- Quyền truy cập được rà soát ít nhất mỗi quý và ngay khi có dấu hiệu tài khoản bị xâm nhập.
- Khi rời dự án, quyền truy cập được thu hồi kịp thời; Secrets và token liên quan được xoay vòng nếu cần.

## 7. Bảo mật và thay đổi khẩn cấp

- Báo cáo lỗ hổng qua kênh bảo mật do repository công bố; không đăng chi tiết khai thác chưa vá lên Issue công khai.
- Sự cố P0 có thể được xử lý khẩn cấp bởi Maintainer/Steering Council; sau đó phải có post-incident review và ghi lại lý do.
- Không commit token, mật khẩu, khóa riêng hoặc dữ liệu cá nhân vào repository.
