Лабораторная работа: Установка LAMP + phpMyAdmin (Debian / Ubuntu / WSL)

## 1. Установка Apache

sudo apt update
sudo apt install apache2 -y


Проверка:
Открыть в браузере http://localhost — должен быть стартовый экран Apache.

## 2. Установка MariaDB

sudo apt install mariadb-server -y
sudo systemctl start mariadb
sudo systemctl enable mariadb


## 3. Настройка безопасности MariaDB

sudo mariadb-secure-installation

## 4. Установка PHP и модулей

sudo apt install php libapache2-mod-php php-mysql -y

## 5. Установка phpMyAdmin

sudo apt install phpmyadmin -y

После установки phpMyAdmin доступен по адресу:
http://localhost/phpmyadmin

## 6. Создание базы данных
1. Открыть phpMyAdmin  
2. Логин: root  
3. Пароль: тот, который вводился в mariadb-secure-installation  
4. Создать новую БД (например `lab1`)

Готово.
