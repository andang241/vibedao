# vibedao

Blog cá nhân dùng [Jekyll](https://jekyllrb.com/) + [GitHub Pages](https://pages.github.com/), giao diện theme `minima`.

Trang web: **https://andang241.github.io/vibedao/**

---

## 1. Cấu trúc thư mục

```
vibedao/
├── _config.yml      # Cấu hình chính của site (tiêu đề, url, baseurl, plugin...)
├── _posts/          # Mỗi bài viết là 1 file Markdown ở đây
├── index.md         # Trang chủ (tự liệt kê bài viết)
├── about.md         # Trang giới thiệu
├── Gemfile          # Khai báo thư viện Ruby (github-pages)
└── .gitignore
```

> Repo tên `vibedao` nên đây là **project site**, chạy tại
> `https://andang241.github.io/vibedao/`. Vì vậy trong `_config.yml`,
> `baseurl` phải để là `/vibedao`.

## 2. Viết bài mới

Tạo file trong `_posts/` theo đúng định dạng tên:

```
_posts/NĂM-THÁNG-NGÀY-tieu-de.md
```

Nội dung mở đầu bằng front matter:

```yaml
---
layout: post
title: "Tiêu đề"
date: 2026-07-09 10:00:00 +0700
categories: [ghi-chú]
tags: [vd]
---
```

## 3. Xem thử trên máy (tùy chọn)

```bash
# Cài công cụ (chỉ làm 1 lần)
gem install bundler --user-install
bundle install

# Chạy server xem trước tại http://localhost:4000
bundle exec jekyll serve
```

## 4. Đưa lên GitHub

```bash
git add .
git commit -m "Cập nhật blog"
git push
```

Sau khoảng 1–2 phút, GitHub sẽ tự build và cập nhật trang web.

## 5. Bật GitHub Pages (chỉ làm 1 lần)

Trên GitHub: **Settings → Pages → Build and deployment**
→ Source: **Deploy from a branch** → Branch: **main** / **/(root)** → Save.
