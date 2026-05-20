# Cấu hình SEO & Metadata cho BrickDocs

File này định nghĩa toàn bộ cấu hình thẻ `<meta>` bắt buộc áp dụng cho toàn bộ trang của dự án BrickDocs. 

## 🤖 Hướng dẫn dành cho Cursor (AI Instructions)
Khi thực hiện chèn thẻ meta vào các trang web:
1. Giữ nguyên các **Thẻ Cố Định** cho tất cả các trang.
2. Tự động thay đổi các **Biến Linh Hoạt** `{{...}}` dựa trên nội dung cụ thể của từng trang (ví dụ: Trang chủ, Trang đọc sách, Trang danh mục).
3. Tuyệt đối không để trống các thẻ có chứa biến linh hoạt.

---

## 📄 Template Metadata Chuẩn

```html
<!-- ========================================================== -->
<!-- 1. NHÓM THẺ CỐ ĐỊNH (Áp dụng giống nhau 100% cho mọi trang) -->
<!-- ========================================================== -->
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="author" content="Dat">
<meta name="robots" content="index, follow">

<!-- Open Graph Chung -->
<meta property="og:site_name" content="BrickDocs">
<meta property="og:locale" content="vi_VN">

<!-- Twitter Card Chung -->
<meta name="twitter:card" content="summary_large_image">

<!-- UI/UX Mobile -->
<meta name="theme-color" content="#ffffff"> <!-- Thay bằng mã màu chủ đạo của BrickDocs nếu cần -->
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
<meta name="apple-mobile-web-app-title" content="BrickDocs">


<!-- ========================================================== -->
<!-- 2. NHÓM BIẾN LINH HOẠT (Phải thay đổi nội dung theo từng trang) -->
<!-- ========================================================== -->
<!-- Tiêu đề trang web -->
<title>{{PAGE_TITLE}} - BrickDocs</title>

<!-- SEO Tiêu chuẩn -->
<meta name="description" content="{{PAGE_DESCRIPTION}}">

<!-- Đường dẫn chuẩn của trang để tránh trùng lặp nội dung -->
<link rel="canonical" href="{{PAGE_URL}}">

<!-- Facebook / Zalo Open Graph -->
<meta property="og:type" content="{{OG_TYPE}}"> <!-- 'website' cho trang chủ/danh mục, 'article' cho trang đọc tài liệu -->
<meta property="og:title" content="{{PAGE_TITLE}} - BrickDocs">
<meta property="og:description" content="{{PAGE_DESCRIPTION}}">
<meta property="og:image" content="{{PAGE_IMAGE_URL}}">
<meta property="og:url" content="{{PAGE_URL}}">

<!-- Twitter / Discord / Slack Card -->
<meta name="twitter:title" content="{{PAGE_TITLE}} - BrickDocs">
<meta name="twitter:description" content="{{PAGE_DESCRIPTION}}">
<meta name="twitter:image" content="{{PAGE_IMAGE_URL}}">