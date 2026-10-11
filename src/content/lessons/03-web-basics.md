---
title: Web tĩnh và GitHub Pages
description: Đóng gói tài liệu thành website tĩnh có thể xuất bản miễn phí.
chapter: Xuất bản
order: 3
---

# Web tĩnh và GitHub Pages

## Mục tiêu

- Hiểu khác biệt giữa source code và thư mục build.
- Kiểm tra liên kết trước khi deploy dưới một project URL.
- Tự cập nhật nội dung Markdown.

## Từ source đến website

Vite đọc các file trong `src`, xử lý module và tạo thư mục `dist`. GitHub Actions sẽ chạy quy trình này rồi gửi `dist` đến GitHub Pages.

```bash
npm install
npm run build
npm run preview
```

Các đường dẫn nội bộ của website này dùng hash (`#/lessons/...`), vì vậy vẫn hoạt động khi site được đặt dưới `/repository-name/`.

## Bài tập

Thêm một bài Markdown mới trong `src/content/lessons/`, rồi kiểm tra nó xuất hiện trong trang Bài học.
