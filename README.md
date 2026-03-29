# 🎨 DoPhanHai Personal Portfolio & Blog

Dự án website cá nhân dành cho **Designer 2D**, xây dựng trên nền tảng **Laravel 11** & **React (Vite)**. Website là sự kết hợp giữa trưng bày tác phẩm nghệ thuật và blog chia sẻ kỹ thuật đồ họa.

---

## 🚀 Tính năng chính
- **Portfolio Gallery:** Trưng bày tác phẩm (Concept Art, UI/UX) hỗ trợ định dạng **WebP**.
- **Tech Blog:** Hệ thống bài viết chuyên sâu về Krita, Photoshop.
- **AI Integration:** Chatbot tư vấn phong cách thiết kế (kế thừa từ core HealthCompass AI).
- **Responsive Design:** Trải nghiệm mượt mà trên mọi thiết bị.

---

## 🛠 Công nghệ sử dụng
- **Backend:** Laravel 11 (PHP 8.2+)
- **Frontend:** React.js, Tailwind CSS, Framer Motion
- **Database:** - *Development:* Oracle Database 21c (Connection qua WSL2)
  - *Production:* MySQL (Shared Hosting / phpMyAdmin)
- **Tools:** Cursor AI, DBeaver, WSL2 (Ubuntu 22.04)

---

## ⚙️ Cài đặt môi trường (Local Development)

### 1. Yêu cầu hệ thống
- PHP >= 8.2 & Composer
- Node.js & NPM
- WSL2 (Ubuntu)

### 2. Các bước cài đặt
```bash
# Clone dự án
git clone https://github.com/I-love-Meat-Fr/DoPhanHai_PersonalWebsite.git
cd DoPhanHai_PersonalWebsite

# Cài đặt Backend & Frontend
composer install
npm install

# Khởi tạo môi trường
cp .env.example .env
php artisan key:generate

```
### 3. Cấu hình Database (WSL2 to Windows Host)
Trong file .env, cập nhật IP của Windows Host (vEthernet):
```bash
DB_CONNECTION=mysql
DB_HOST=172.20.32.1  # IP vEthernet (WSL) của máy bạn
DB_PORT=3306
DB_DATABASE=portfolio_db
DB_USERNAME=root
DB_PASSWORD=your_password
```

### 4. Khởi chạy
Mở 2 terminal song song:
```bash
# Tab 1: Backend
php artisan serve

# Tab 2: Frontend
npm run dev
```
#📂 Cấu trúc Database (Database First)
artworks: Quản lý tác phẩm (Title, Slug, Image WebP, Category, Tags).

posts: Quản lý nội dung Blog (liên kết với Artworks qua artwork_id).

#👤 Author
Họ tên: Quoc Anh (Do Phan Hai)

Role: Full-stack Developer & Digital Artist

Contact: nguyenquocanh170205@gmail.com
