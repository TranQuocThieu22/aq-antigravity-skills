---
name: git-commit-convention
description: Quy định bắt buộc khi viết commit message cho dự án backend
---

# Quy Định Viết Git Commit Message (Backend)

Khi thực hiện tạo commit cho các dự án backend, bạn **bắt buộc** phải tuân thủ các quy tắc sau:

1. **Ngôn ngữ**: Commit message phải được viết bằng **Tiếng Việt**.
2. **Thành phần/API bị ảnh hưởng**: Bắt buộc phải lưu/ghi chú rõ **tên API, Service hoặc chức năng bị ảnh hưởng** bởi thay đổi trong nội dung commit (ví dụ: `=> Thành phần bị ảnh hưởng: API lấy danh sách hoạt động cộng đồng / Service gửi email`).
3. **Cấu trúc**:
   - Tiêu đề commit (dòng 1): Theo chuẩn `<type>(<scope>): <short summary>`.
     + `<type>` có thể là `feat`, `fix`, `refactor`, `update`, `chore`,... Bắt buộc KHÔNG DÙNG chữ "Cập nhật".
     + `<scope>` (trong ngoặc đơn) **BẮT BUỘC** là tên service/module/package bị ảnh hưởng (ví dụ: `sae-api`, `aq-core-framework`, `auth-service`). Nếu thay đổi từ 2 module trở lên, phân tách bằng dấu phẩy (ví dụ: `refactor(sae-api,auth-service): ...`). Tuyệt đối không dùng tên folder tính năng nhỏ làm scope.
     + `<short summary>` **BẮT BUỘC** phải viết bằng **Tiếng Việt** (ví dụ: `tối ưu hoá query database và xoá file utils cũ`).
   - Body commit: Giải thích chi tiết hơn về thay đổi (nếu cần thiết) và dòng ghi chú thành phần/API bị ảnh hưởng.
4. **Quy trình thực hiện**: Tuyệt đối **KHÔNG** tự ý thực thi các lệnh `git commit`. Bạn chỉ được phép sinh ra nội dung commit message và in ra trong phần chat để người dùng tự xem xét (review) và tự commit.
