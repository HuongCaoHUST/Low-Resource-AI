---
title: Git và GitHub
description: Lưu lịch sử thay đổi và cộng tác với repository từ xa.
chapter: Công cụ làm việc
order: 2
---

# Git và GitHub

## Mục tiêu

- Phân biệt working tree, staging area và commit.
- Tạo nhánh cho một thay đổi nhỏ.
- Đẩy source code lên GitHub an toàn.

## Vòng đời của một thay đổi

Mỗi thay đổi nên có phạm vi nhỏ và một thông điệp commit dễ đọc. Sau khi kiểm tra bằng `git diff`, bạn có thể đưa file vào staging rồi tạo commit.

```bash
git status
git add .
git commit -m "docs: add first lesson"
git push origin main
```

Không đưa token, mật khẩu hoặc file chứa thông tin cá nhân vào repository. Có thể tham khảo [tài liệu Git chính thức](https://git-scm.com/doc) để xem đầy đủ lệnh.

## Bài tập

Tạo một branch tên `exercise/git-basics`, cập nhật README và mở pull request cho branch chính.
