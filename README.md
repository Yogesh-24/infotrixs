
# Infotrixs - AWS Cloud Intern

## 🔗 Links
[![Github](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://yogeshn.netlify.app)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)]([https://www.linkedin.com/](https://www.linkedin.com/in/yogeshn2403/))

 
# Task 1

## Installation

1. Install apache server 

```bash
  sudo apt install apache2

```

2. Install php runtime and php mysql connector
```bash
sudo apt install php libapache2-mod-php php-mysql

```
3. Install MySQL server
```bash
sudo apt install mysql-server 

```
4. Login to MySQL server
```bash
sudo mysql -u root

```
5. Change authentication plugin to mysql_native_password (change the password to something strong)
```bash
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password by 'yogesh@123';

```
6. Create a new database user for wordpress (change the password to something strong)
```bash
CREATE USER 'wp_user'@localhost IDENTIFIED BY 'yogesh@123';

```
7. Create a database for wordpress
```bash
CREATE DATABASE wordpress;

```
8. Grant all privilges on the database 'wordpress' to the newly created user
```bash
GRANT ALL PRIVILEGES ON wp.* TO 'wordpress_user'@localhost;

```
9. Download wordpress
```bash
cd /tmp
wget https://wordpress.org/latest.tar.gz

```
10. Unzip
```bash
tar -xvf latest.tar.gz

```
11. Move wordpress folder to apache document root
```bash
sudo mv wordpress/ /var/www/html

```
12. Command to restart/reload apache server
```bash
sudo systemctl restart apache2

```
    
