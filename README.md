# Dev Course · HUST

Website tài liệu lập trình tĩnh, chỉ dùng HTML, CSS và một JavaScript nhỏ cho menu mobile. Không cần Node.js, npm, backend hoặc bước build.

## Chạy local

Mở `index.html` trực tiếp bằng trình duyệt, hoặc dùng một static server bất kỳ:

```bash
python3 -m http.server 8000
```

Sau đó truy cập `http://localhost:8000`.

## Thêm bài học

Tạo một file HTML mới, ví dụ `lesson-04.html`, sao chép cấu trúc từ một bài học hiện có, thay nội dung, rồi thêm liên kết tới bài mới trong `lessons.html`.

## Cấu hình repository

Thay `https://github.com/your-username/your-course-repository` trong các file HTML bằng URL GitHub thật trước khi publish.

## Deploy GitHub Pages

1. Đẩy repository lên GitHub, dùng branch `main`.
2. Vào **Settings → Pages → Build and deployment**, chọn **GitHub Actions**.
3. Workflow `.github/workflows/deploy.yml` sẽ upload trực tiếp thư mục gốc, không build.

Các liên kết dùng tên file tương đối, nên hoạt động tại URL dạng `https://username.github.io/repository-name/`.
