# Project SAP-ERP

A modular Laravel-based ERP (Enterprise Resource Planning) system designed to support the management of business processes and data. This project is built step-by-step to support scalability and maintainability.

## ⚙️ Technologies Used

-   [Laravel](https://laravel.com/) 11.x
-   [Laravel Breeze](https://github.com/laravel/breeze) for auth scaffolding
-   MySQL (via Laragon)
-   Blade (Laravel templating engine)
-   Docker (optional, for containerized development)
-   Vite & Tailwind CSS (optional frontend stack)

## 🖥️ Requirements

-   PHP >= 8.2
-   Composer
-   Node.js & NPM
-   MySQL (recommended: Laragon or Docker) and i'm with Laragon

## 🚀 Installation with Laragon

Follow these steps to run the SAP-ERP project using [Laragon](https://laragon.org/), a lightweight and portable Laravel development environment for Windows.

### 1. Install Laragon

If you haven't already:

-   Download Laragon from [https://laragon.org/download/](https://laragon.org/download/)
-   Install Laragon (you can choose to install it in `D:\laragon` if you prefer to keep it off the C: drive)
-   Start Laragon and ensure **Apache** and **MySQL** services are running

---

### 2. Create a New Laravel Project via Laragon (Optional)

You can create a fresh Laravel project directly in Laragon:

-   Open Laragon
-   Click **Menu > Quick App > Laravel**
-   Laragon will generate the Laravel project in `D:\laragon\www\your-project-name`

---

### 3. Open Project Directory

Open `D:\laragon\www\sap-erp` in your code editor (e.g., VS Code).

---

### 4. Install Dependencies

Open Terminal (from VS Code or Laragon context menu) and run:

```bash
composer install
npm install && npm run dev
```

### 5. Configure Environment File .env

```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel-sap-erp
DB_USERNAME=root
DB_PASSWORD=

```

### 6. Run migrations

```
php artisan migrate
```

### 7. Start the App

```
php artisan serve
```

### 8. Acces app in localhost

```
http://127.0.0.1:8000/
```
