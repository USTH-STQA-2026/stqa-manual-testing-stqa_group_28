#  Test Execution – STQA Group 28

## 1. Thông tin nhóm
- **Nhóm:** STQA Group 28   
- **Ngày thực thi:** 17/06/2026  
- **Trình duyệt:** Chrome 126  
- **Hệ điều hành:** Windows 11  

---

## 2. Kết quả chi tiết

| Mã TC | Nhóm chức năng | Kết quả mong đợi (tóm tắt) | Kết quả thực tế | Kết luận | Minh chứng | Bug |
|-------|----------------|----------------------------|-----------------|----------|------------|-----|
| TC01 | Đăng nhập | Vào dashboard | Vào dashboard | Pass | - | - |
| TC02 | Đăng nhập | Thông báo lỗi | Thông báo lỗi | Pass | - | - |
| TC03 | Đăng nhập | Thông báo lỗi | Thông báo lỗi | Pass | - | - |
| TC04 | Đăng nhập | Hiển thị “Tạm ngưng” | Một số màn hình hiển thị “Hoạt động” | Fail | - | BUG-04 |
| TC05 | Đăng nhập/Mượn sách | Hiển thị “Hết hạn” | Vẫn cho phép mượn sách | Fail | - | BUG-02, BUG-04 |
| TC06 | Quản lý user | Thêm thành viên hợp lệ | Cho phép email không hợp lệ | Fail | - | BUG-01 |
| TC07 | Quản lý user | Thông báo lỗi email trùng | Thông báo lỗi | Pass | - | - |
| TC08 | Quản lý user | Cập nhật vai trò + thông báo | Cập nhật nhưng không có thông báo | Fail | - | BUG-06 |
| TC09 | Quản lý user | Không cho xóa user đang mượn | Thông báo lỗi | Pass | - | - |
| TC10 | Quản lý sách | Thêm sách mới | Thêm thành công | Pass | - | - |
| TC11 | Quản lý sách | ISBN trùng → lỗi | Thông báo lỗi | Pass | - | - |
| TC12 | Quản lý sách | Sửa thông tin | Cập nhật thành công | Pass | - | - |
| TC13 | Quản lý sách | Không cho xóa sách đang mượn | Thông báo lỗi | Pass | - | - |
| TC14 | Mượn sách | Mượn thành công | Thành công | Pass | - | - |
| TC15 | Mượn sách | Hết số lượng → lỗi | Thông báo lỗi | Pass | - | - |
| TC16 | Mượn sách | Quá giới hạn → lỗi | Thông báo lỗi | Pass | - | - |
| TC17 | Trả sách | Trả đúng hạn → “Đã trả” | “Đã trả” | Pass | - | - |
| TC18 | Trả sách | Trả quá hạn → “Quá hạn” | “Quá hạn” | Pass | - | - |
| TC19 | Tìm kiếm | Hiển thị kết quả | Không hiển thị hoặc sai | Fail | - | BUG-03 |
| TC20 | Tìm kiếm | “Không có kết quả” | “Không có kết quả” | Pass | - | - |
| TC21 | Quản trị | Truy cập thủ thư | Thành công | Pass | - | - |
| TC22 | Quản trị | User hoạt động bị chặn | Một số trạng thái hiển thị sai ngôn ngữ | Fail | - | BUG-07 |
| TC23–TC28 | Bổ sung | Đúng như mong đợi | Đúng như mong đợi | Pass | - | - |

---

## 3. Tổng hợp kết quả

| Chỉ số | Giá trị |
|--------|----------|
| Tổng số test case | 28 |
| Pass | 21 |
| Fail | 7 |
| Blocked | 0 |
| Not Run | 0 |
| Tỷ lệ Pass | ~75% |

---

## 4. Kết quả theo nhóm chức năng

| Nhóm | Tổng TC | Pass | Fail | Tỷ lệ Pass |
|------|----------|------|------|------------|
| Đăng nhập | 5 | 3 | 2 | 60% |
| Quản lý user | 4 | 2 | 2 | 50% |
| Quản lý sách | 4 | 4 | 0 | 100% |
| Mượn/Trả sách | 5 | 5 | 0 | 100% |
| Tìm kiếm | 2 | 1 | 1 | 50% |
| Quản trị | 2 | 1 | 1 | 50% |
| Bổ sung | 6 | 6 | 0 | 100% |
