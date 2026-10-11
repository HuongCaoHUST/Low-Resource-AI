# Dev Course · HUST

Website tài liệu lập trình tĩnh, xây bằng Vite và JavaScript thuần. Nội dung bài học nằm trong Markdown để dễ chỉnh sửa và deploy miễn phí bằng GitHub Pages.

## Chạy local

```bash
npm install
npm run dev
```

Kiểm tra bản production:

```bash
npm run build
npm run preview
```

## Thêm bài học

Tạo file `.md` mới trong `src/content/lessons/` với frontmatter:

```md
---
title: Tên bài học
description: Mô tả ngắn.
chapter: Tên chương
order: 4
---
```

Sau đó viết nội dung Markdown bên dưới. Trang Bài học sẽ tự đọc các file này khi build.

## Cấu hình repository

Sửa `repositoryUrl` trong `src/config.js` thành URL GitHub thật trước khi publish. Đây là nơi duy nhất cần cập nhật URL repository.

## Deploy GitHub Pages

1. Đẩy repository lên GitHub, dùng branch `main`.
2. Vào **Settings → Pages → Build and deployment**, chọn **GitHub Actions**.
3. Mỗi lần push lên `main`, workflow `.github/workflows/deploy.yml` sẽ build và deploy thư mục `dist`.

`base: './'` và hash routing giúp asset, điều hướng hoạt động khi website nằm dưới URL dạng `https://username.github.io/repository-name/`.
