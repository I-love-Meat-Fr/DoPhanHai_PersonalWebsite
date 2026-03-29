# 🎨 DoPhanHai Personal Portfolio & Blog

Dự án website cá nhân dành cho Designer 2D, được xây dựng trên nền tảng **Laravel 11** và **React (Vite)**. Website kết hợp giữa việc trưng bày tác phẩm nghệ thuật (Artworks) và chia sẻ kiến thức đồ họa (Blog).

---

## 🚀 Tính năng chính
- **Portfolio Gallery:** Trưng bày các tác phẩm 2D (Concept Art, UI/UX) hỗ trợ định dạng WebP tối ưu dung lượng.
- **Tech Blog:** Hệ thống bài viết chia sẻ kinh nghiệm, kỹ thuật vẽ và công cụ (Krita, Photoshop).
- **AI Integration:** Dự kiến tích hợp chatbot hỗ trợ tư vấn phong cách thiết kế (HealthCompass AI core).
- **Responsive Design:** Giao diện tối ưu cho cả Mobile và Desktop.

---

## 🛠 Công nghệ sử dụng
- **Backend:** Laravel 11 (PHP 8.2+)
- **Frontend:** React.js, Tailwind CSS, Framer Motion
- **Database:** - Development: Oracle Database 21c (WSL2 Connection)
  - Production: MySQL (Shared Hosting / phpMyAdmin)
- **Tools:** Cursor AI, DBeaver, WSL2 (Ubuntu)

---

## ⚙️ Cài đặt môi trường (Local Development)

### 1. Yêu cầu hệ thống
- PHP >= 8.2
- Composer
- Node.js & NPM
- WSL2 (Nếu chạy trên Windows)

### 2. Các bước cài đặt
```bash
# Clone dự án
git clone [https://github.com/I-love-Meat-Fr/DoPhanHai_PersonalWebsite.git](https://github.com/I-love-Meat-Fr/DoPhanHai_PersonalWebsite.git)
cd DoPhanHai_PersonalWebsite

# Cài đặt thư viện Backend
composer install

# Cài đặt thư viện Frontend
npm install

# Tạo file cấu hình môi trường
cp .env.example .env
php artisan key:generate

3. Cấu hình Database (WSL2 to Windows Host)
Trong file .env, cập nhật địa chỉ IP của Windows Host (vEthernet):

Đoạn mã
DB_CONNECTION=mysql
DB_HOST=172.20.32.1  # Thay đổi theo IP vEthernet thực tế
DB_PORT=3306
DB_DATABASE=portfolio_db
DB_USERNAME=root
DB_PASSWORD=your_password

4. Khởi chạy
Bash
# Tab 1: Chạy Backend
php artisan serve

# Tab 2: Chạy Frontend (Vite)
npm run dev

📂 Cấu trúc Database (Database First)
Dự án được thiết kế theo hướng Database First với 2 bảng chính:

artworks: Lưu trữ tiêu đề, mô tả, link ảnh WebP, danh mục và tags.

posts: Lưu trữ nội dung bài viết blog liên kết với tác phẩm.

👤 Author
Họ tên: Quoc Anh (Do Phan Hai)

Role: Full-stack Developer & Digital Artist

Contact: nguyenquocanh170205@gmail.com