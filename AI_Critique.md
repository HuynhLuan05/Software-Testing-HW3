# Đánh giá và Phản biện AI (AI Critique)

Qua quá trình cộng tác với AI trong bài tập HW03 về kiểm thử GUI & Usability cho hệ thống quản lý sự kiện EMS (Event Management System), em nhận thấy các thế mạnh và hạn chế rõ rệt của AI như sau:

### 1. Những sai sót và điểm chưa hoàn thiện của AI
AI thường đưa ra các đánh giá giao diện mang tính lý thuyết tĩnh và thiếu bối cảnh nghiệp vụ thực tế của SUT:
- **Giới hạn về Thị giác & Tương tác động:** AI chỉ có thể phân tích giao diện tĩnh dựa trên các ảnh chụp màn hình được cung cấp. Nó không thể phát hiện hoặc đánh giá các tương tác động theo thời gian thực, ví dụ như hiệu ứng chuyển đổi mượt mà khi kéo thả, hay hiển thị của các thông báo Toast.
- **Thiên lệch dữ liệu (Bias):** AI có xu hướng đề xuất các tiêu chuẩn UI chung chung (như khuyên thêm nút Home hoặc thanh cuộn) mà không hiểu rõ nghiệp vụ đặc thù của EMS.
- **Không bắt được lỗi chức năng động:** AI không thể tự nhận biết được một dropdown bị "liệt" (như dropdown chọn số dòng phân trang ở màn D3 bấm vào không phản hồi) nếu chỉ nhìn ảnh chụp tĩnh. Điều này đòi hỏi con người phải trực tiếp thao tác để phát hiện lỗi.

### 2. Nguyên nhân AI bỏ sót các vấn đề
Nguyên nhân chủ yếu do AI thiếu môi trường thực thi động (dynamic execution context) để chạy thử nghiệm thực tế ứng dụng và có xu hướng suy luận dựa trên các mẫu thiết kế phổ biến có sẵn trong dữ liệu huấn luyện. Nếu prompt đầu vào của người dùng chỉ ở dạng mô tả tính năng chung chung mà không đính kèm mã nguồn chi tiết, AI sẽ tạo ra các bộ test cases lý thuyết và bỏ lọt hầu hết các lỗi logic nội bộ cũng như lỗi bảo mật thực tế.

### 3. Bài học rút ra khi cộng tác với AI
Nguyên tắc cốt lõi là luôn duy trì vai trò "Human-in-the-loop" (con người kiểm duyệt). AI đóng vai trò xuất sắc trong việc sinh bộ khung ý tưởng ban đầu (như bộ khung checklist >40 mục) và tra cứu nhanh các nguyên tắc thiết kế UI. Tuy nhiên, việc thực thi kiểm thử trên thiết bị thật, tương tác trực tiếp với các nút bấm và trải nghiệm cảm xúc của người dùng thật (User Testing với 5 người) là không thể thay thế bởi bất kỳ mô hình AI nào ở thời điểm hiện tại.