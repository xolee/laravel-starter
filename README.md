<p align="center">
    <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
</p>
<p align="center">
    <img src="https://user-images.githubusercontent.com/41773797/131910226-676cb28a-332d-4162-a6a8-136a93d5a70f.png" alt="Filament Banner" width="800" />
</p>
<p align="center">基于 Laravel 和 Filament 构建的后台管理系统</p>

## 环境需求

- PHP 8.2+
- Laravel 12+
- Filament 4.0+
- ext-curl
- ext-fileinfo
- ext-libxml
- ext-openssl
- ext-simplexml
- ext-sodium

## 安装 Install

```bash
git clone https://github.com/xolee/laravel-starter.git laravel-starter
cd laravel-starter

# 本地开发安装
composer install

# 生产线上安装
# composer install --no-dev

# 环境配置
cp .env.example .env
php artisan key:generate
php artisan migrate

# 使用 Filament 面板开发
php artisan filament:install --panels
php artisan make:filament-user
```

## Branch 分支说明

使用 Git Flow 来进行版本分支管理，每个版本对应一个分支。

- `master` 该分支为稳定分支，用于发布稳定版本
- `develop` 该分支为开发分支，用于开发新功能
- `laravel-version` 该分支为 Laravel 版本分支，用于 Laravel 升级使用

## 改善 Filament 面板性能

```bash
# 缓存 icons
php artisan icons:cache
# 缓存 Filament components
php artisan filament:cache-components
# 缓存 Laravel Files
php artisan optimize
```

## 其他

```bash
# 清除 Filament components 缓存
php artisan filament:clear-cached-components
# 清除 Laravel 缓存
php artisan optimize:clear
```
## Package List

基于 Laravel 和 Filament 构建的后台管理系统。

- [Laravel](https://github.com/laravel/laravel)
- [Filament](https://github.com/filamentphp/filament)

### Require Package List

### Require-dev Package List
- [barryvdh/laravel-debugbar](https://packagist.org/packages/barryvdh/laravel-debugbar)
