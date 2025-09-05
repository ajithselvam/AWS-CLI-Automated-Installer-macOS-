# AWS-CLI-Automated-Installer-macOS-
AWS CLI Automated Installer (macOS)

# AWS CLI Automated Installer (macOS)

This project provides a Bash script to **automate the installation of AWS CLI on macOS** using Homebrew.  
It supports both **Apple Silicon (M1/M2)** and **Intel-based Macs**, handling permissions and sudo access automatically.

---

## ✨ Features
- Detects system architecture (**arm64 / Intel**).  
- Grants necessary permissions for Homebrew installation directories.  
- Temporarily adds the user to `sudoers` for a seamless installation.  
- Installs **AWS CLI** using Homebrew.  
- Verifies installation after setup.  
- Cleans up sudoers entry for security.

---

## 📦 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/aws-cli-macos-installer.git
   cd aws-cli-macos-installer
2. Make the script executable:

chmod +x install-aws-cli.sh


3. Run the script:

./install-aws-cli.sh

✅ Verification

After installation, check AWS CLI version:

aws --version

⚙️ Script Workflow

Detects logged-in user.

Grants temporary sudo privileges.

Configures Homebrew installation path based on architecture.

Installs AWS CLI via Homebrew.

Verifies successful installation.

Cleans up temporary sudoers entry.


🛠️ Requirements

macOS (Intel or Apple Silicon).

Internet connection.

Homebrew installed.

📜 License

This project is licensed under the MIT License.
Feel free to modify and use it as per your requirements.
