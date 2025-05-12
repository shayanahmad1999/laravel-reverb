# 🧠 Laravel Reverb Realtime Task App

This project demonstrates how to build a **real-time task management app** using **Laravel Reverb** and **Vue.js**. Tasks are added, updated, and deleted with live updates via Laravel's broadcasting features.

---

## 🚀 Quick Start

```bash
# 1. Create Laravel project
composer create-project laravel/laravel todo
cd todo

# 2. Setup broadcasting
php artisan install:broadcasting

# 3. Install Laravel Reverb
php artisan reverb:install

# 4. Create model and migration
php artisan make:model Task -m
php artisan migrate

# 5. Create events
php artisan make:event TaskAdded
php artisan make:event TaskUpdated
php artisan make:event TaskDeleted

# 6. Create controller
php artisan make:controller TaskController

# 7. Install frontend dependencies
npm install
npm install --save-dev @vitejs/plugin-vue

# 8. Build frontend
npm run build

# 9. Start servers
php artisan reverb:start --debug
php artisan serve

OR 
click the below links and read document carefully

https://www.twilio.com/en-us/blog/laravel-reverb-comprehensive-guide-real-time-broadcasting