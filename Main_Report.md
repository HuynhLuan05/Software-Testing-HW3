# Báo Cáo Chính: GUI & Usability Testing - Phân Hệ Yêu Cầu Hỗ Trợ (EMS)

## 1. Giới Thiệu
*   **Hệ thống kiểm thử (SUT):** EMS (Event Management System) - [Link Web SUT](https://prod-dev.ems-fitus.cloud/dashboard).
*   **Kịch bản được chọn:** **Kịch bản D — Vòng đời Support-Request** (Người dùng tạo yêu cầu hỗ trợ, xem trạng thái phản hồi và Admin quản trị duyệt, note nội bộ, gửi phản hồi chính thức).
*   **Danh sách các màn hình kiểm thử:**
    1.  `Màn hình D1 (User Side):` Form tạo yêu cầu hỗ trợ (Support Request Form).
    2.  `Màn hình D2 (User Side):` Danh sách My Requests & Trang chi tiết yêu cầu kèm phản hồi.
    3.  `Màn hình D3 (Admin Side):` Trang quản lý danh sách yêu cầu hỗ trợ của Admin (có bộ lọc tìm kiếm và phân trang).

---

## 2. Task 1B — Thực Thi GUI Checklist trên 3 Màn Hình

Dưới đây là bảng chạy checklist GUI dùng chung của nhóm (48 mục) được áp dụng trực tiếp trên 3 màn hình của Kịch bản D:

| Mã CL | Khía Cạnh | Tiêu Chí Kiểm Tra | Heuristic / Nguyên Tắc | Màn D1 | Màn D2 | Màn D3 | Ghi Chú Lỗi (Notes nếu Fail) |
|---|---|---|---|:---:|:---:|:---:|---|
| **GUI-01** | IA-01 | Bố cục tổng thể (Layout) nhất quán giữa các trang | Nielsen #4, Shneiderman #1, Norman #5 | Pass | Pass | Pass | |
| **GUI-02** | IA-01 | Typography nhất quán (font-family, font-size, line-height) | Nielsen #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-03** | IA-01 | Bảng màu (Color palette) nhất quán và có đủ tương phản | Nielsen #4, Shneiderman #2, Norman #1 | Pass | Pass | Pass | |
| **GUI-04** | IA-01 | Canh lề (Alignment) và khoảng cách (Spacing) đồng nhất | Nielsen #8, Shneiderman #1 | Pass | Fail | Fail | **D2**: Lệch vị trí icon thời gian gửi; **D3**: Các ô nhập ngày bị lệch hàng dọc. |
| **GUI-05** | IA-01 | Responsive design — hiển thị trên các kích thước màn hình | Shneiderman #2, Norman #1 | Pass | Pass | Pass | |
| **GUI-06** | IA-01 | Trạng thái Empty state hiển thị thông báo rõ ràng | Nielsen #1, Norman #2, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-07** | IA-01 | Trạng thái Loading hiển thị rõ ràng | Nielsen #1, Norman #2, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-08** | IA-01 | Hỗ trợ đa ngôn ngữ (i18n EN/VI) chuyển đổi chính xác | Shneiderman #2, Nielsen #4 | Pass | Pass | Pass | |
| **GUI-09** | IA-01 | Icon có ý nghĩa rõ ràng và nhất quán | Nielsen #6, Norman #6, Shneiderman #8 | Pass | Pass | Pass | |
| **GUI-10** | IA-01 | Hình ảnh (thumbnail, avatar, banner) hiển thị đúng tỷ lệ | Nielsen #8, Norman #1 | Pass | Pass | Pass | |
| **GUI-11** | IA-01 | Nút bấm (Button) có trạng thái rõ ràng: default, hover, active, disabled | Nielsen #1, Norman #2, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-12** | IA-01 | Accessibility — Điều hướng bằng bàn phím (Keyboard navigation) | Shneiderman #2, Nielsen #7 | Pass | Pass | Pass | |
| **GUI-13** | IA-01 | Accessibility — Thuộc tính ARIA và cấu trúc heading | Shneiderman #2, Nielsen #4 | Pass | Pass | Pass | |
| **GUI-14** | IA-02 | Label của form field rõ ràng và đặt đúng vị trí | Nielsen #6, Norman #1, Shneiderman #8 | Pass | Pass | Pass | |
| **GUI-15** | IA-02 | Trường bắt buộc được đánh dấu rõ ràng (dấu * hoặc "(Required)") | Nielsen #5, Shneiderman #5, Norman #3 | Pass | Pass | Pass | |
| **GUI-16** | IA-02 | Validation inline — hiển thị lỗi ngay tại trường lỗi | Nielsen #9, Shneiderman #5, Norman #2 | Pass | Pass | Pass | |
| **GUI-17** | IA-02 | Thông báo lỗi mang tính hướng dẫn (constructive error message) | Nielsen #9, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-18** | IA-02 | Validation ngày/giờ — ngày kết thúc phải sau ngày bắt đầu | Nielsen #5, Shneiderman #5, Norman #3 | Pass | Pass | Pass | |
| **GUI-19** | IA-02 | Upload hình ảnh — hiển thị preview, kiểm tra kích thước và định dạng | Nielsen #5, Norman #3, Shneiderman #5 | Pass | Pass | Pass | |
| **GUI-20** | IA-02 | Rich-Text Editor hoạt động đúng | Nielsen #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-21** | IA-02 | Form giữ lại dữ liệu đã nhập khi validation fail | Shneiderman #6, Nielsen #5 | Pass | Pass | Pass | |
| **GUI-22** | IA-02 | Dropdown / Select có thể tìm kiếm khi danh sách dài | Nielsen #7, Shneiderman #7, Norman #6 | Pass | Pass | Pass | |
| **GUI-23** | IA-02 | Giới hạn ký tự (character limit) được hiển thị cho các trường có giới hạn | Nielsen #1, Shneiderman #5, Norman #3 | Pass | Pass | Pass | |
| **GUI-24** | IA-02 | Placeholder text không thay thế label và biến mất khi focus | Nielsen #6, Shneiderman #8 | Pass | Pass | Pass | |
| **GUI-25** | IA-02 | Tab order trong form đúng logic (trên→dưới, trái→phải) | Shneiderman #2, Nielsen #7 | Pass | Pass | Pass | |
| **GUI-26** | IA-02 | Xác nhận trước khi mất dữ liệu form chưa lưu | Nielsen #5, Shneiderman #5, Norman #3 | Pass | Pass | Pass | |
| **GUI-27** | IA-03 | Menu sidebar hiển thị mục đang active | Nielsen #1, Norman #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-28** | IA-03 | Breadcrumb hiển thị đúng đường dẫn phân cấp | Nielsen #1, Nielsen #6, Shneiderman #8 | Pass | Pass | Pass | |
| **GUI-29** | IA-03 | Nút Back / Return hoạt động đúng và không mất dữ liệu | Nielsen #3, Shneiderman #6, Norman #4 | Pass | Pass | Pass | |
| **GUI-30** | IA-03 | Deep link / URL trực tiếp dẫn đến đúng trang | Nielsen #7, Shneiderman #7 | Pass | Pass | Pass | |
| **GUI-31** | IA-03 | Tabs chuyển đổi đúng nội dung và có indicator | Nielsen #1, Norman #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-32** | IA-03 | Pagination hoạt động đúng và hiển thị thông tin trang | Nielsen #1, Shneiderman #3, Norman #1 | Pass | Pass | Fail | **D3**: Dropdown "Số dòng mỗi trang" bị đơ, không thay đổi số lượng dòng hiển thị. |
| **GUI-33** | IA-03 | Menu sidebar collapse/expand trên màn hình nhỏ | Shneiderman #2, Nielsen #7 | Pass | Pass | Pass | |
| **GUI-34** | IA-03 | Link/nút điều hướng dẫn đến đúng đích | Nielsen #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-35** | IA-03 | Nút quay lại trang người dùng từ admin (và ngược lại) | Nielsen #3, Shneiderman #6, Norman #4 | Pass | Pass | Pass | |
| **GUI-36** | IA-03 | Scroll-to-top khi chuyển trang hoặc tải nội dung mới | Shneiderman #2, Nielsen #7 | Pass | Pass | Pass | |
| **GUI-37** | IA-04 | Toast notification hiển thị sau hành động thành công | Nielsen #1, Norman #2, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-38** | IA-04 | Dialog xác nhận trước hành động hủy hoại (destructive action) | Nielsen #5, Shneiderman #5, Norman #3 | Pass | Pass | Pass | |
| **GUI-39** | IA-04 | Màu trạng thái (status color) nhất quán và có ý nghĩa | Nielsen #4, Norman #4, Shneiderman #1 | Pass | Pass | Pass | |
| **GUI-40** | IA-04 | Progress bar / indicator cho hành động mất thời gian | Nielsen #1, Norman #2, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-41** | IA-04 | Badge/counter hiển thị số lượng chưa xử lý | Nielsen #1, Norman #1, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-42** | IA-04 | Thông báo lỗi hệ thống (server error) hiển thị thân thiện | Nielsen #9, Shneiderman #3, Norman #2 | Pass | Pass | Pass | |
| **GUI-43** | IA-04 | Double-click / Double-submit bị chặn | Nielsen #5, Shneiderman #5 | Pass | Pass | Pass | |
| **GUI-44** | IA-04 | Cập nhật real-time (nếu có) — dữ liệu tự refresh | Nielsen #1, Norman #2 | Pass | Pass | Pass | |
| **GUI-45** | IA-04 | Trạng thái phiên đăng nhập (Session) — timeout và thông báo | Nielsen #9, Shneiderman #3 | Pass | Pass | Pass | |
| **GUI-46** | IA-04 | Export file (Excel) — phản hồi tải xuống rõ ràng | Nielsen #1, Shneiderman #3, Norman #2 | Pass | Pass | Pass | |
| **GUI-47** | IA-04 | Lightbox / Modal ảnh hoạt động đúng | Nielsen #3, Norman #6, Shneiderman #6 | Pass | Pass | Pass | |
| **GUI-48** | IA-04 | Undo / Hoàn tác hành động vừa thực hiện | Nielsen #3, Shneiderman #6 | Pass | Pass | Pass | |

