# Bug Reports — Báo cáo lỗi

> **Hướng dẫn**: Tạo 1 mục bug cho mỗi TC có kết quả **Fail**.
> Xem [examples/sample-bug-report.md](../examples/sample-bug-report.md) để hiểu cách viết bug report tốt.
> Mỗi bug cần: tiêu đề mô tả hành vi lỗi, bước tái hiện, expected vs actual, severity + giải thích.

| Thông tin | |
|---|---|
| **Nhóm** | Group 28 |
| **Ngày báo cáo** | 13-06-2026 |

---

## BUG-01

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-01 |
| **TC liên quan** | TC06 |
| **REQ liên quan** | REQ-02 |
| **Mức độ** | High |
| **Người phát hiện** | Trần Nam Long |
| **Ngày phát hiện** | 02-06-2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Tài khoản bị tạm ngưng có thể đăng nhập được

**Môi trường:**
- Trình duyệt: Chrome 149
- Hệ điều hành: Microsoft
- Ngôn ngữ giao diện: Tiếng Việt

**Điều kiện tiên quyết:**
Đăng nhập vào tài khoản admin

**Bước tái hiện:**
1. Vào phần "Thêm thành viên"
2. Điền họ tên, email, SĐT cho thành viên mới

**Kết quả mong đợi:**
Tài khoản được thêm vào trong database, hiện lên thông báo 'Tài khoản đã được thiết lập thành công'

**Kết quả thực tế:**
Email không hợp lệ

**Tác động:**
Admin không thể thêm tài khoản của các học sinh mới

**Minh chứng:**
bug02.png

**Đề xuất xử lý:**
Sửa lại tính năng thêm email cho thành viên mới của tài khoản admin

---

## BUG-02

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-02 |
| **TC liên quan** | TC05, TC14, TC15 |
| **REQ liên quan** | REQ-04, REQ-05 |
| **Mức độ** | High |
| **Người phát hiện** | Trần Nam Long |
| **Ngày phát hiện** | 02-06-2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Thành viên hết hạn vẫn có thể mượn sách

**Điều kiện tiên quyết:**


**Bước tái hiện:**


**Kết quả mong đợi:**


**Kết quả thực tế:**


**Tác động:**
Ảnh hưởng trực tiếp đến logic việc mượn/trả sách đối với các tài khoản.

**Minh chứng:**
bug02.png

**Đề xuất xử lý:**


---

## BUG-03

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-03 |
| **TC liên quan** | TC07 |
| **REQ liên quan** | REQ-02 |
| **Mức độ** | Low |
| **Người phát hiện** | Lương Xuân Phúc |
| **Ngày phát hiện** | 02-06-2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Thêm tài khoản có thông tin tương tự admin

**Điều kiện tiên quyết:**
Email đã tồn tại từ trước đó

**Bước tái hiện:**
1. Vào phần "Thêm thành viên"
2. Ghi lại thông tin của thành viên Lê Cần Cù

**Kết quả mong đợi:**
Email hoặc thông tin bị trùng lặp

**Kết quả thực tế:**
Hiện sai thông báo

**Tác động:**
Có thể gây hiểu lầm

**Minh chứng:**
bug03.png

**Đề xuất xử lý:**
Thay đổi thông báo khi có tín hiệu trùng thông tin đăng nhập

---

## BUG-04

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-04 |
| **TC liên quan** | TC16 |
| **REQ liên quan** | REQ-04 |
| **Mức độ** | High |
| **Người phát hiện** | Trần Nam Long |
| **Ngày phát hiện** | 03-06-2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Thành viên có thể mượn số lượng sách vượt quá giới hạn

**Điều kiện tiên quyết:**
Đăng nhập vào email của tài khoản Nguyễn Học Bá

**Bước tái hiện:**
1. Mượn dần 5 quyển sách theo thứ tự: BOOK001, BOOK002, BOOK003, BOOK004, BOOK005

**Kết quả mong đợi:**
Thông báo "Đã đạt giới hạn số lượng sách có thể mượn, không thể mượn quyển BOOK004."

**Kết quả thực tế:**
Mượn thành công BOOK004, lỗi thông báo sai khi mượn BOOK005.

**Tác động:**
Thành viên có thể lợi dụng lỗ hổng để mượn quá số lượng sách theo giới hạn

**Minh chứng:**
bug04.png

**Đề xuất xử lý:**
Sửa lại khả năng đếm số lượng sách thành viên đã mượn

---

## BUG-05

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-05 |
| **TC liên quan** | TC18 |
| **REQ liên quan** | REQ-05 |
| **Mức độ** | High |
| **Người phát hiện** | Lương Xuân Phúc |
| **Ngày phát hiện** | 04-06-2026 |
| **Trạng thái** | Open |

**Tiêu đề:**
Lỗi hiển thị sách quá hạn trong tài khoản thành viên

**Điều kiện tiên quyết:**
Đăng nhập vào tài khoản của thành viên Phạm Trung Bình

**Bước tái hiện:**
1. Vào trực tiếp phần Mượn-Trả


**Kết quả mong đợi:**
Hiển thị sách quá hạn, chưa trả

**Kết quả thực tế:**
Không hiển thị

**Tác động:**
Thành viên không thể mượn hay trả sách

**Minh chứng:**
bug05.png

**Đề xuất xử lý:**
Sửa lại phần hiển thị trong UI của web đối với các tài khoản quá hạn

---

## BUG-06

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-06 |
| **TC liên quan** | TC17 |
| **REQ liên quan** | REQ-02 |
| **Mức độ** | High |
| **Người phát hiện** | Trần Nam Long |
| **Ngày phát hiện** | 08-06-2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Lỗi trả hộ sách cho thành viên khác

**Điều kiện tiên quyết:**
Đăng nhập vào tài khoản của thành viên Nguyễn Học Bá

**Bước tái hiện:**
1. Vào mục Mượn/Trả
2. Tìm thông tin MEM006
3. Trả hộ sách cho thành viên Hoàng Cá Biệt

**Kết quả mong đợi:**
hiển thị thông báo bạn không có quyền truy cập

**Kết quả thực tế:**
trả thành công

**Tác động:**
thành viên có thể lợi dụng kẽ hở để hại thành viên khác thông qua việc trả sách trong thời hạn mượn

**Minh chứng:**
bug07.png

**Đề xuất xử lý:**
giới hạn lại khả năng truy cập và tương tác của từng thành viên trong mục Mượn/Trả

---

## BUG-07

| Thuộc tính | Chi tiết |
|-----------|---------|
| **Mã lỗi** | BUG-07 |
| **TC liên quan** | TC22 |
| **REQ liên quan** | REQ-08 |
| **Mức độ** | Medium |
| **Người phát hiện** | Trần Nam Long |
| **Ngày phát hiện** | 09/06/2026 |
| **Trạng thái** | Closed |

**Tiêu đề:**
Giao diện không đồng bộ ngôn ngữ

**Điều kiện tiên quyết:**
Đăng nhập tài khoản Nguyễn Học Bá

**Bước tái hiện:**
1. Vào trang của Admin
2. `<!-- -->`
3. `<!-- -->`

**Kết quả mong đợi:**
Bị từ chối, hiển thị không có quyền truy cập

**Kết quả thực tế:**
Một số trạng thái hiển thị sai ngôn ngữ và đăng nhập được vào trang admin

**Tác động:**
Một số thành viên có thể lạm dụng lỗi

**Minh chứng:**
bug09.png

**Đề xuất xử lý:**
Sủa lại khả năng truy cập của thành viên với trang Admin và hiển thị ngôn ngữ

