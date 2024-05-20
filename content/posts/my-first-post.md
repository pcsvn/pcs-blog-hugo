+++
title = 'My First Post'
date = 2024-05-09T15:50:29+07:00
draft = false
+++
## Introduction

**Cài đặt Kho - Repository**
Đối với các trang blog xây dựng bằng Jekyll thì có lẽ bạn chỉ cần duy nhất một repository như bước 2 là đủ ( tùy một số theme yêu cầu cài plugin mà github không hỗ trợ thì phải làm hơi khác). Nhưng với trang blog xây dựng bằng Hugo thì bạn cần thêm một repository nữa (cái này tên gì cũng được vì không được public ra ngoài). Như vậy chúng ta sẽ tạo 2 repository với mục đích như sau:


1. <blog-name>-hugo (tạm gọi là Kho lớn) : mục tiêu cao cả là lưu trữ toàn bộ source code của bạn. 
2. <github username>.github.io (tạm gọi là kho nhỏ) : nhiệm vụ lưu trữ những thứ được generate ra và host trang blog của bạn. Tạo xong hai repository thì bạn clone chúng về máy tính, tuy nhiên bạn cần chú ý là đặt repo github.io làm submodule của repo lớn, để khi chúng ta update repo nhỏ thì repo lớn tự động update:
``` Markdown
git clone git@github.com:<username>/<blog-name>-hugo.git
git submodule add git@github.com:<username>/<username>.github.io.git
```
### Kho - Repository

Myconfig

| Option | Description | Note |
| ------ | ----------- | ---- |
| [pcs-blog-hugo](https://github.com/pcsvn/pcs-blog-hugo) | Kho chủ |Private |
| [pcsvn.github.io](https://github.com/pcsvn/pcsvn.github.io) | Kho con | Public |

```
git clone git@github.com:pcsvn/pcs-blog-hugo.git
git submodule add git@github.com:pcsvn/pcsvn.github.io.git
```
Lab Mình làm tại thư mục D:\GitHubDeskTop\quickstart thông qua VS Code
Laptop ở nhà dùng VS CODE và thay bằng lệnh 
```
'git submodule add https://github.com/pcsvn/pcsvn.github.io.git'
```
## Tài liệu tham khảo
* https://tw-docs.com/docs/static-site-generators/hugo-install/
* https://www.itnota.com/setup-visual-studio-code-hugo-static-site-generator/
* https://www.youtube.com/watch?v=7SHqBNRP9bQ&ab_channel=GetIntoGameDev
* https://codecungtui.github.io/tao-blog-don-gian-voi-hugo-va-github
## Themes 
https://github.com/dillonzq/LoveIt

Update Big Repo from Private to Public
sau khi thay đổi có thể chỉnh bài viết từ trình duyệt web!