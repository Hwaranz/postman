# postman
# Báo cáo Thực hành Kiểm thử API với Postman

**Người kiểm thử:** Nguyễn Xuân Thanh  

## 1. Mục tiêu thực hành
- Sử dụng Postman để gửi các HTTP Request (GET, POST) tới hệ thống API (reqres.in).
- Áp dụng các Snippet JavaScript trong Postman để tự động hóa việc kiểm tra HTTP Status Code.
- Sử dụng Collection Runner để chạy kiểm thử hàng loạt.

## 2. Chi tiết các Test Case

### 2.1. Lấy danh sách người dùng (GET Request)
- **API Endpoint:** `GET https://reqres.in/api/users?page=2`
- **Mục tiêu:** Kiểm tra API có trả về mã trạng thái 200 OK hay không.
- **Kết quả:** Request thành công, test case báo `PASS`.
*<img width="962" height="597" alt="Screenshot 2026-10-07 100206" src="https://github.com/user-attachments/assets/b6748ea7-9716-43d6-bdfe-0de996dc17b2" />
*

### 2.2. Tạo người dùng mới (POST Request)
- **API Endpoint:** `POST https://reqres.in/api/users`
- **Body Data:** Gửi lên dữ liệu JSON gồm tên và nghề nghiệp.
- **Mục tiêu:** Kiểm tra mã trạng thái trả về là `201 Created` (tạo mới thành công).
- **Kết quả:** Request thành công, test case báo `PASS`.
*<img width="962" height="595" alt="Screenshot 2026-10-07 100522" src="https://github.com/user-attachments/assets/f78c263c-0873-49f1-8ff0-aa5c40fc0880" />
*

### 2.3. Chạy kiểm thử tự động với Collection Runner
- Đã nhóm các request vào chung một Collection `Thuc-hanh-API` và chạy tự động.
- **Kết quả:** 100% test case (2/2) đều vượt qua.
*<img width="964" height="596" alt="Screenshot 2026-10-07 101055" src="https://github.com/user-attachments/assets/03fd30cc-3d15-484c-aea8-264057f9f3e1" />
*
