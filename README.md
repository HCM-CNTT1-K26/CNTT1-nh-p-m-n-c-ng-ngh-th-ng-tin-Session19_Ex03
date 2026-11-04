# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session19_Ex03
## 1. Báo cáo

* **Input:** Facebook/Gmail văng phiên liên tục, có vị trí đăng nhập lạ, nguy cơ lộ cookie/token.
* **Process:** Ngắt mạng Đổi pass từ thiết bị sạch, Thu hồi Token GitHub và Cài lại Windows / Quét virus.
* **Output:** Máy sạch, tài khoản an toàn với mật khẩu mới và 2FA.

---

## 2. Triển khai

### Bước 1: Đổi mật khẩu & Đăng xuất thiết bị khác

Lấy **điện thoại** (đã ngắt Wi-Fi, dùng 4G) để thực hiện:

* Vào phần bảo mật Facebook / Google Chọn **Đổi mật khẩu**.
* Bấm chọn dòng **Đăng xuất khỏi tất cả các thiết bị khác** (Log out of all other sessions).
* *Kiểm tra:* Vào lại mục danh sách thiết bị đang hoạt động, thấy duy nhất điện thoại hiện tại là thành công.

---

### Bước 2: Thu hồi Token trên GitHub (Revoke Token)

1. **Vào Developer Settings:** Thực hiện trên thiết bị sạch.
Đăng nhập GitHub trên điện thoại hoặc máy sạch, click vào ảnh avatar, **Settings**, Kéo xuống chọn **Developer settings**.
*Kiểm tra:* Màn hình hiện menu quản lý Personal access tokens và OAuth apps.


2. **Revoke Personal Access Tokens:** Hủy các token nghi ngờ.
Vào **Personal access tokens** (kiểm tra cả *Tokens (classic)* lẫn *Fine-grained tokens*). Nhấp vào token lạ hoặc cũ rồi nhấn nút **Revoke** màu đỏ.
*Kiểm tra:* Token biến mất khỏi bảng danh sách, các ứng dụng hay script cũ dùng token này bị cắt truy cập ngay lập tức.


3. **Revoke OAuth Apps:** Xóa ứng dụng bên thứ ba.
Vào mục **OAuth Apps** ở danh mục bên trái. Duyệt qua các ứng dụng đã cấp quyền, cái nào thấy lạ hoặc không dùng nữa thì bấm **Revoke access**.
*Kiểm tra:* Danh sách ứng dụng liên kết được dọn sạch, không còn app lạ lọt vào.
