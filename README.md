🎨 DoPhanHai Personal Portfolio & Blog
A personal website project for a 2D Designer, built on Laravel 11 & React (Vite). The website is a combination of an art showcase and a blog for sharing digital art techniques.

🚀 Key Features
Portfolio Gallery: Showcases artworks (Concept Art, UI/UX) with WebP format support.

Tech Blog: In-depth article system covering Krita and Photoshop.

AI Integration: Design style consultant chatbot (inherited from the HealthCompass AI core).

Responsive Design: Smooth experience across all devices.

🛠 Tech Stack
Backend: Laravel 11 (PHP 8.2+)

Frontend: React.js, Tailwind CSS, Framer Motion

Database: - Development: Oracle Database 21c (Connection via WSL2)

Production: MySQL (Shared Hosting / phpMyAdmin)

Tools: Cursor AI, DBeaver, WSL2 (Ubuntu 22.04)

⚙️ Local Development Setup
1. System Requirements
PHP >= 8.2 & Composer

Node.js & NPM

WSL2 (Ubuntu)

2. Installation Steps
```Bash
# Clone the project
git clone https://github.com/I-love-Meat-Fr/DoPhanHai_PersonalWebsite.git
cd DoPhanHai_PersonalWebsite

# Install Backend & Frontend dependencies
composer install
npm install

# Initialize environment
cp .env.example .env
php artisan key:generate
```
3. Database Configuration (WSL2 to Windows Host)
In the .env file, update the Windows Host IP (vEthernet):

```Bash
DB_CONNECTION=mysql
DB_HOST=172.20.32.1  # Your machine's WSL vEthernet IP
DB_PORT=3306
DB_DATABASE=portfolio_db
DB_USERNAME=root
DB_PASSWORD=your_password
```
4. Running the Application
Open 2 terminals simultaneously:

```Bash
# Tab 1: Backend
php artisan serve

# Tab 2: Frontend
npm run dev
```
#📂 Database Schema (Database First)
artworks: Manages artworks (Title, Slug, Image WebP, Category, Tags).

posts: Manages blog content (linked to Artworks via artwork_id).

#👤 Author
Full Name: Quoc Anh (Do Phan Hai)

Role: Full-stack Developer & Digital Artist

Contact: nguyenquocanh170205@gmail.com