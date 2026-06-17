#  Summary – STQA Group 28

## 1. Thông tin nhóm
- **Nhóm:** STQA Group 28  
- **Lớp:** SE001.P11  
- **Ngày báo cáo:** 17/06/2026  
- **Hệ thống kiểm thử:** [Library App](https://stqa.rbc.vn) – v1.0  

---

## 2. Tổng quan kết quả
- **Tổng số Test Case:** 28  
- **Pass:** 21  
- **Fail:** 7 (tương ứng với BUG-01 → BUG-07)  
- **Blocked:** 0  
- **Not Run:** 0  
- **Tỷ lệ Pass:** ~75%  

### Phân bổ bug theo mức độ
| Mức độ | Số lượng | Bug IDs |
|--------|----------|---------|
| High   | 1        | BUG-02 |
| Medium | 4        | BUG-01, BUG-03, BUG-05, BUG-07 |
| Low    | 2        | BUG-04, BUG-06 |

---

## 3. Kỹ thuật thiết kế đã sử dụng
- **Equivalence Partitioning (EP):** cho hầu hết các chức năng (REQ-01 → REQ-07).  
- **Boundary Value Analysis (BVA):** cho đăng nhập sai mật khẩu, mượn quá giới hạn, mượn sách hết số lượng.  
- **Decision Table (DT):** cho xóa user đang mượn sách, xóa sách đang mượn.  

---

## 4. Phân tích chất lượng phần mềm
### Điểm mạnh
- Chức năng thêm/xóa sách hoạt động đúng.  
- Đăng nhập với tài khoản hợp lệ vào dashboard thành công.  
- Tìm kiếm sách không tồn tại trả về thông báo chính xác.  

### Điểm yếu
- Cho phép thành viên hết hạn mượn sách (BUG-02).  
- Validation email chưa chặt chẽ (BUG-01).  
- Hiển thị số sách mượn không chính xác (BUG-05).  
- Giao diện ngôn ngữ không đồng bộ (BUG-07).  

---

## 5. Đề xuất ưu tiên sửa lỗi
| Thứ tự | Bug | Mức độ | Lý do ưu tiên |
|--------|-----|--------|---------------|
| 1 | BUG-02 | High | Ảnh hưởng trực tiếp đến logic nghiệp vụ mượn sách |
| 2 | BUG-05 | Medium | Sai dữ liệu số lượng sách mượn |
| 3 | BUG-01 | Medium | Vi phạm quy tắc nhập liệu |
| 4 | BUG-03 | Medium | Tìm kiếm không chính xác |
| 5 | BUG-07 | Medium | Giao diện ngôn ngữ không đồng bộ |
| 6 | BUG-04 | Low | Hiển thị trạng thái không đồng bộ |
| 7 | BUG-06 | Low | Thiếu thông báo khi đổi trạng thái |

---

## 6. Kết luận
Hệ thống cơ bản đáp ứng được các yêu cầu chính, nhưng chưa sẵn sàng phát hành vì tồn tại bug nghiêm trọng (BUG-02). Cần khắc phục bug High và Medium trước khi triển khai chính thức.

---

## 7. Bài học rút ra
- Thiết kế test case đa dạng (EP, BVA, DT) giúp phát hiện nhiều lỗi logic.  
- Minh chứng hình ảnh giúp báo cáo thuyết phục và dễ kiểm tra.  
- Việc đối chiếu Bug ↔ TC ↔ REQ giúp quản lý chất lượng chặt chẽ.  

---

## 8. Khai báo sử dụng AI
- **Công cụ AI:** 
- **Dùng cho phần:**   
- **Kiểm tra/chỉnh sửa:**   
