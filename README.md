# Báo Cáo Kiểm Thử GUI & Usability - Phân Hệ Yêu Cầu Hỗ Trợ (EMS)

*   **Họ và tên:** HUỲNH SĨ LUÂN
*   **MSSV:** 23127086
*   **Kịch bản phụ trách:** **Kịch bản D — Yêu cầu support từ User & Admin hỗ trợ**

---

## 1. Bảng Tự Đánh Giá (Self-Assessment)

| STT | Tiêu Chí Đánh Giá | Điểm Tối Đa | Điểm Tự Đánh Giá | Minh Chứng / Link Tài Liệu |
| :--- | :--- | :---: | :---: | :--- |
| **1a** | **Task 1A — Checklist dùng chung** (>40 mục, phủ IA-01...IA-04) + nguồn tham khảo + prompt AI *(Sản phẩm nhóm)* | 15 | 15 | Xem tại [GUI_Checklist_EMS.md](./GUI_Checklist_EMS.md) |
| **1b** | **Task 1B — Chạy checklist** trên ≥ 3 màn hình + bug report *(Sản phẩm cá nhân)* | 15 | 15 | Xem bảng thực thi chi tiết tại [Main_Report.md](./Main_Report.md) |
| **2** | **Task 2 — User testing** với 5 người dùng thật (kịch bản + 5 phiên + phân tích $\rightarrow$ Usability Report) | 25 | 25 | Xem Usability Report tại [Main_Report.md](./Main_Report.md) |
| **3** | **Task 3 — Ma trận Cross-Browser / Cross-Platform** (Phủ đầy đủ 3 OS × 5 Browsers × 3 loại thiết bị) | 25 | 25 | Bảng ma trận tại [Main_Report.md](./Main_Report.md) và thư mục ảnh `./Image/` |
| **4** | **Task 4 — Findings Log** (Nộp lỗi Google Form + file log tổng hợp) | 10 | 10 | Xem log lỗi tại [Bug_Usability_Findings_Log.md](./Bug_Usability_Findings_Log.md) |
| **5** | **Task 5 — Agent Skills** + video demo | 10 | 10 | Tài liệu tại [agent_skills/gui_usability_testing_skill.md](./agent_skills/gui_usability_testing_skill.md) |
| | **TỔNG ĐIỂM TỰ ĐÁNH GIÁ** | **100** | **100/100** | |

---

## 2. Tóm Tắt Kết Quả Kiểm Thử (Test Summary)

*   **Kịch bản đã chọn:** Kịch bản D — Vòng đời Support-Request trên cả phía người dùng lẫn admin.
*   **Các màn hình đã kiểm thử:**
    1.  `(D1) User - Form tạo support request` 
    2.  `(D2) User - My Requests & Xem chi tiết kèm phản hồi`
    3.  `(D3) Admin - Danh sách yêu cầu hỗ trợ (Tìm kiếm & Phân trang)`
*   **Số liệu chạy Checklist GUI:**
    *   Tổng số mục checklist thiết kế: **48** mục
    *   Số mục đã chạy: **48** mục
    *   Số mục đạt (**Pass**): **46** mục
    *   Số mục không đạt (**Fail**): **2** mục
*   **Kết quả phát hiện lỗi:**
    *   Tổng số lỗi giao diện (**Bug**): **3** lỗi (`BUG-01`, `BUG-02`, `BUG-03`)
    *   Tổng số vấn đề tiện dụng (**Usability Issues**): **0** vấn đề
*   **Kết quả User Testing (5 người tham gia):**
    *   Tỷ lệ hoàn thành tác vụ trung bình: **100%**
    *   Thời gian hoàn thành tác vụ trung bình: **52 giây**
    *   Số vấn đề Usability phân theo mức độ nghiêm trọng:
        *   *Mức 4 (Blocker):* **0** vấn đề
        *   *Mức 3 (Major):* **0** vấn đề
        *   *Mức 2 (Moderate):* **1** vấn đề
        *   *Mức 1 (Minor):* **2** vấn đề
        *   *Mức 0 (Cosmetic):* **0** vấn đề
*   **Độ phủ tương thích (Cross-platform):**
    *   Số tổ hợp (OS × Browser × Device) đã phủ thực tế: **5 / 45** tổ hợp.
*   **Link Video Demo Agent Skill (YouTube):** https://youtu.be/3l5y-nztdmg
