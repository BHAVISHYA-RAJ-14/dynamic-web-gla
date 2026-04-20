# BH Dynamic Web Project
This project is a dynamic PHP website hosted on an **AWS EC2 (Amazon Linux 2023)** instance and synced with **GitHub**.

## 🚀 Project Overview
- **Server:** AWS EC2
- **OS:** Amazon Linux 2023
- **Web Server:** Apache (httpd)
- **Language:** PHP 8.x
- **Timezone:** Asia/Kolkata (IST)

---

## 🛠️ Installation & Setup Commands

### 1. Server Environment
| Command | Function |
| :--- | :--- |
| `sudo dnf install -y httpd php git` | Installs Web Server, PHP, and Git. |
| `sudo systemctl start httpd` | Starts the Apache server. |
| `sudo chown -R ec2-user:ec2-user /var/www/html` | Permissions to edit files without sudo. |

### 2. Git Configuration
| Command | Function |
| :--- | :--- |
| `git init` | Starts a new local repository. |
| `git remote add origin <URL>` | Connects EC2 to your GitHub repo. |
| `git config --global credential.helper store` | **Saves your Token so you don't have to login every time.** |

---

## 📸 Project Screenshots
> **Note:** To see these images, upload your screenshots to the GitHub repository and name them exactly as shown below.

#### 1. Live Website Status
![Website Screenshot](website_preview.png)

#### 2. Terminal Configuration
![Terminal Screenshot](terminal_setup.png)

---

## 📝 How to Update the Site
Whenever you want to change the text or code, run these three commands:
1. `nano index.php` (Edit your code)
2. `git commit -am "Your update message"`
3. `git push origin main`
