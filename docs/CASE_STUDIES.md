# CASE STUDIES – PHƯƠNG ÁN XỬ LÝ TÌNH HUỐNG THỰC CHIẾN

## 1. Tranh cãi độc hại và vi phạm Code of Conduct

### 1.1 Quy trình xử lý theo bốn cấp độ

Tình huống: một lập trình viên kỳ cựu có PR tối ưu thuật toán giúp giảm 45% thời gian xử lý, nhưng lại công kích cá nhân một sinh viên mới khi trả lời câu hỏi kỹ thuật.

**Bước 1 – Correction (nhắc nhở/chỉnh sửa):** Steering Council lưu lại bằng chứng, yêu cầu dừng ngay lời lẽ công kích và nhắc người vi phạm rằng review phải tập trung vào mã nguồn. Nếu là lần đầu, mức xử lý ban đầu có thể là Correction; đồng thời ẩn hoặc xóa nội dung xúc phạm nếu cần để bảo vệ người bị nhắm tới.

**Bước 2 – Warning (cảnh cáo):** Nếu hành vi nghiêm trọng hoặc tái diễn, gửi cảnh cáo chính thức, trích dẫn quy định bị vi phạm, yêu cầu cam kết không tái phạm và thông báo rõ chế tài tiếp theo.

**Bước 3 – Temporary Ban (tạm đình chỉ):** Nếu tiếp tục quấy rối hoặc có hành vi trả đũa, tạm khóa quyền bình luận/đóng góp trong thời hạn xác định. Nhóm chỉ định người khác xử lý PR để không làm đình trệ dự án.

**Bước 4 – Permanent Ban (cấm vĩnh viễn):** Áp dụng với hành vi đe dọa, quấy rối nghiêm trọng, tiết lộ thông tin riêng tư hoặc tái phạm sau các cảnh cáo. Thu hồi quyền truy cập và lưu hồ sơ quyết định.

Không nhất thiết phải đi tuần tự cả bốn bước nếu mức độ vi phạm đặc biệt nghiêm trọng. Người xử lý cần khách quan, bảo mật danh tính người báo cáo và cho phép yêu cầu xem xét lại bởi người không tham gia quyết định ban đầu.

### 1.2 Có merge PR tối ưu ngay lập tức không?

**Không merge ngay lập tức chỉ vì chất lượng thuật toán tốt.** Chất lượng mã nguồn và an toàn cộng đồng là hai tiêu chí độc lập. Merge ngay khi chưa xử lý vi phạm có thể tạo thông điệp rằng người đóng góp giỏi được miễn trừ quy tắc, khiến Contributor mới rời bỏ dự án và làm suy giảm niềm tin.

Nhóm nên tạm dừng merge để review độc lập phần kỹ thuật, yêu cầu tác giả chỉnh sửa hành vi và đánh giá rủi ro. Nếu mã nguồn đáp ứng test, bảo mật, giấy phép và review, PR có thể được merge sau khi có biện pháp xử lý CoC phù hợp. Nếu tác giả không hợp tác hoặc tiếp tục công kích, nhóm có thể đóng PR hoặc chuyển quyền xử lý cho Maintainer khác. Không dùng chất lượng code để đổi lấy việc dung thứ hành vi độc hại.

## 2. Xung đột thương mại hóa và nguy cơ Hard Fork

### 2.1 Bài học từ Redis → Valkey và Terraform → OpenTofu

- **Redis → Valkey:** việc thay đổi điều khoản cấp phép của phần mềm phổ biến có thể khiến cộng đồng và nhà cung cấp phân phối tách ra để duy trì hướng phát triển theo giấy phép mở. Một fork có cơ hội tồn tại khi có nhóm Maintainer, nhà tài trợ, quy trình phát hành và hệ sinh thái hỗ trợ đủ mạnh.
- **Terraform → OpenTofu:** khi định hướng cấp phép thay đổi, cộng đồng có thể phối hợp tạo fork do một tổ chức trung lập hỗ trợ, duy trì khả năng tương thích và xây dựng lộ trình phát triển riêng.

Bài học: niềm tin cộng đồng, tính dự đoán được của giấy phép và quyền sử dụng lâu dài có giá trị không kém nguồn tài trợ. Hard Fork không chỉ là sao chép mã nguồn; nó cần quản trị độc lập, người bảo trì, hạ tầng CI/CD, bảo mật, thương hiệu và kế hoạch chuyển đổi.

MIT là giấy phép mã nguồn mở được OSI phê duyệt. BSL/SSPL có điều khoản hạn chế khác và không được xem là giấy phép Open Source theo định nghĩa OSI. Không thể mặc nhiên áp dụng giấy phép mới hồi tố lên các bản phát hành MIT đã tồn tại; việc đổi giấy phép cho phiên bản tương lai cần kiểm tra quyền tác giả, CLA/copyright assignment và sự đồng ý cần thiết của các chủ sở hữu bản quyền.

### 2.2 Kế hoạch họp giải quyết xung đột lợi ích

1. **Công bố minh bạch:** đăng RFC nêu rõ đề nghị tài trợ 300.000 USD, điều kiện BSL/SSPL, chi phí cơ hội, ảnh hưởng đến người dùng và các lựa chọn khác.
2. **Đánh giá pháp lý:** nhờ tư vấn pháp lý kiểm tra quyền đổi giấy phép, đóng góp của bên thứ ba, CLA và nghĩa vụ với phiên bản MIT hiện tại.
3. **Thu thập ý kiến:** mở ít nhất 14 ngày thảo luận; mời Maintainer, Contributor, nhà cung cấp và người dùng doanh nghiệp tham gia. Không chỉ lấy ý kiến nhóm có lợi ích tài chính trực tiếp.
4. **So sánh phương án:** giữ MIT và nhận tài trợ không kèm độc quyền; tài trợ qua quỹ trung lập; Open Collective/sponsorship; dual licensing cho phần mã đủ điều kiện; dịch vụ hỗ trợ/hosted service; hoặc nhận vốn nhưng tách sản phẩm thương mại khỏi lõi OSS.
5. **Bỏ phiếu có kiểm soát xung đột lợi ích:** thành viên có lợi ích tài chính phải công khai và không quyết định thay cộng đồng. Steering Council công bố biên bản, tiêu chí và kết quả.
6. **Quyết định:** ưu tiên duy trì giấy phép MIT cho dòng mã hiện tại và quyền lợi người dùng. Chỉ xem xét đổi giấy phép cho phiên bản tương lai nếu có cơ sở pháp lý, đồng thuận đủ rộng và kế hoạch chuyển đổi rõ ràng.
7. **Phương án Fork:** nếu cộng đồng không đồng thuận, hỗ trợ quá trình fork có trật tự: xác định người duy trì, tên/nhãn hiệu riêng, CI/CD, quy trình bảo mật, roadmap, tài liệu migration và thông báo cho người dùng.

### 2.3 Đề xuất cuối cùng

Không chấp nhận điều kiện đổi giấy phép toàn bộ dự án từ MIT sang BSL/SSPL chỉ để nhận 300.000 USD khi chưa có đánh giá pháp lý và đồng thuận của cộng đồng. Nhóm nên thương lượng tài trợ không độc quyền, nhận tài trợ qua quỹ hoặc phát triển dịch vụ thương mại tách biệt. Nếu nhà đầu tư không chấp nhận, từ chối khoản tài trợ và tiếp tục phát triển theo giấy phép MIT; nếu xảy ra fork, tôn trọng quyền fork hợp pháp và cạnh tranh bằng chất lượng, minh bạch và tốc độ hỗ trợ cộng đồng.
