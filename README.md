# 🚀 Laravel API Authentication (Passport)
A simple REST API built with Laravel 12 using **Laravel Passport** for authentication (login, logout, and user management).  

## 📌 Features
- ✅ User Registration  
- ✅ User Login with API Token  
- ✅ Secure Logout  
- ✅ Authentication using Laravel Passport  
- ✅ RESTful API structure  

## 📂 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### 2️⃣ Install Dependencies
```bash
composer install
```

### 3️⃣ Configure Environment
Copy the `.env` file and update database credentials:
```bash
cp .env.example .env
```
Then generate the application key:
```bash
php artisan key:generate
```

### 4️⃣ Set Up Database
Run migrations to create tables:
```bash
php artisan migrate
```

### 5️⃣ Install & Set Up Passport
```bash
php artisan passport:install
```

### 6️⃣ Run the Application
```bash
php artisan serve
```
API will be available at:  
🔗 `http://127.0.0.1:8000/api/`

## 📌 API Endpoints

| Method | Endpoint        | Description               | Auth Required  |
|--------|-----------------|---------------------------|----------------|
| POST   | `/api/register` | Register a new user       |     No         |
| POST   | `/api/login`    | Login & get token         |     No         |
| POST   | `/api/logout`   | Logout (invalidate token) |     Yes        |


🔹 **Headers for Authenticated Requests:**  
```
Authorization: Bearer YOUR_ACCESS_TOKEN
```

## 📜 License
This project is open-source and free to use.  

---

