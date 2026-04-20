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
<img width="1840" height="312" alt="Screenshot 2026-04-20 093733" src="https://github.com/user-attachments/assets/fda2d8f1-ce04-4bce-a5e4-a9c89686df11" />

#### 2. Terminal Configuration
<img width="1402" height="857" alt="Screenshot 2026-04-20 093717" src="https://github.com/user-attachments/assets/012bfed0-fc41-4214-959d-1ed569685430" />

## 📝 How to Update the Site
Whenever you want to change the text or code, run these three commands:
1. `nano index.php` (Edit your code)
2. `git commit -am "Your update message"`
3. `git push origin main`
