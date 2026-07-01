# 1. Chọn ngành
- **Ngành chọn để phân tích**: Y tế / Symptom Checker / Health Assistant

# 2. Chấm Risk Profile / Điền Industry Risk Snapshot

- **Phạm vi giả định:** chatbot/app hỏi triệu chứng, gợi ý khả năng bệnh, hướng dẫn tự chăm sóc, hoặc khuyến nghị đi khám/cấp cứu.

| Câu hỏi | Low / Medium / High / Critical | Vì sao? |
|---|---|---|
| Nếu AI sai, có thể gây hại thể chất không? | Critical | Có. Nếu AI phân loại sai triệu chứng, trấn an sai, hoặc khuyên người bệnh không đi cấp cứu, **người dùng có thể trì hoãn điều trị hoặc xử trí sai**. Các nghiên cứu về symptom checker cho thấy độ chính xác chẩn đoán và triage còn biến thiên, có thể tạo rủi ro an toàn cho bệnh nhân. |
| AI có ảnh hưởng đến quyết định hệ trọng không? | Critical | Có. Dù chỉ là “assistant”, kết quả AI có thể **ảnh hưởng trực tiếp đến quyết định: ở nhà theo dõi, đi khám thường, đi cấp cứu, dùng thuốc không kê đơn, hoặc tin rằng tình trạng không nghiêm trọng**. WHO nhấn mạnh AI y tế cần bảo vệ tự chủ con người, an toàn, trách nhiệm và tính minh bạch. |
| Hệ thống có động tới dữ liệu nhạy cảm không? | Critical | Có. Người dùng có thể nhập **triệu chứng, bệnh nền, thuốc đang dùng, tiền sử bệnh, tuổi, giới tính, ảnh y tế, vị trí hoặc thông tin định danh**. Đây là nhóm dữ liệu sức khỏe rất nhạy cảm; HHS mô tả HIPAA Privacy Rule là chuẩn bảo vệ hồ sơ y tế và thông tin sức khỏe có thể định danh cá nhân. |
| Nếu sai, hậu quả có khó đảo ngược không? | High | Có. Nếu AI **bỏ sót dấu hiệu cấp cứu** như đau ngực, đột quỵ, nhiễm trùng nặng, thai kỳ nguy cơ cao hoặc phản ứng thuốc, **việc chậm can thiệp có thể để lại hậu quả lâu dài**. |
| Nếu triển khai rộng, blast radius có lớn không? | High | Lớn. Symptom checker hoặc health assistant thường là sản phẩm số, có thể phục vụ nhiều người dùng cùng lúc. **Một lỗi trong model, prompt, triage rule hoặc dữ liệu y khoa có thể lặp lại trên nhiều người dùng.** WHO cũng ghi nhận các mô hình AI đa phương thức có khả năng được ứng dụng rộng trong chăm sóc sức khỏe, nghiên cứu y tế và y tế công cộng. |
| Có cần human review hoặc escalation không? | Critical | Có, bắt buộc cần cơ chế chuyển tuyến/escalation. **Các trường hợp có “red flags”, triệu chứng nặng, trẻ em, người già, phụ nữ mang thai, bệnh nền phức tạp, nguy cơ tự hại hoặc model low-confidence** cần được chuyển đến bác sĩ, cấp cứu, hoặc kênh hỗ trợ chuyên môn. WHO đưa ra nhiều khuyến nghị để bảo đảm việc dùng AI trong y tế là phù hợp và bảo vệ sức khỏe cộng đồng. |
| **Risk profile tổng thể của ngành** | Critical | Ngành này có rủi ro tổng thể **Critical** vì hội tụ cả 5 yếu tố: có thể gây hại thể chất, ảnh hưởng quyết định y tế hệ trọng, xử lý dữ liệu sức khỏe nhạy cảm, hậu quả sai có thể khó đảo ngược, và có khả năng lan rộng nếu triển khai đại trà. FDA cũng xem nhiều phần mềm AI/ML trong y tế là nhóm cần quản lý để hỗ trợ nhà cung cấp dịch vụ và cải thiện chăm sóc bệnh nhân một cách an toàn. |