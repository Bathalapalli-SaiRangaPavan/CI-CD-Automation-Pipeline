# Visual Studio Code, Git, Terraform, AWS CLI Installation, Configuring AWS CLI, and Mobaxterm Installation Guide for Windows
This guide provides step-by-step instructions for installing Visual Studio Code, Git, Terraform, and AWS CLI on a Windows system, along with configuring AWS CLI and installing Mobaxterm.
## Prerequisites

- Windows operating system
- Internet connection

---

## Installing Visual Studio Code on Windows

### 1. Download the Installer

- Visit the official Visual Studio Code website at [https://code.visualstudio.com/download](https://code.visualstudio.com/download).

### 2. Download for Windows

- Click the "Download for Windows" button on the VSCode website to download the installer package appropriate for your Windows version.

### 3. Run the Installer

- Locate the downloaded installer file (usually in your Downloads folder) and double-click it to run it.

### 4. Installation Wizard

- Follow the on-screen instructions in the installation wizard:
  - Select "I accept the agreement".
  - Choose the installation location (optional).
  - Select additional tasks like adding VSCode to the system PATH or creating a desktop shortcut (optional).
  - Click "Install" to begin the installation process.

### 5. Completing the Installation

- Once the installation is complete, ensure the "Launch Visual Studio Code" option is checked, and then click "Finish".

### 6. VSCode First Launch

- Visual Studio Code will open for the first time. You're now ready to start using the editor.

---
# Installing Git Bash on Windows

## Downloading Git Bash

1. Open your web browser.
2. Search for "Git Bash download".
3. Visit the official Git website [here](https://git-scm.com/).
4. Download the Git for Windows installer (typically a .exe file).
5. Choose the appropriate version for your system (32-bit or 64-bit).

## Installing Git Bash

1. Once the download is complete, locate the downloaded .exe file.
2. Double-click on the installer file to start the installation process.
3. Follow the installation wizard instructions:
    - Click "Next" to proceed.
    - Read and accept the license agreement.
    - Choose the installation directory (default is recommended).
    - Select components to install (default options are recommended).
    - Choose the start menu folder (default is recommended).
    - Select the desired additional tasks (e.g., creating desktop icon).
    - Click "Next" to begin the installation.
    - Wait for the installation process to complete.
    - Click "Finish" to exit the installer.

## Verifying Git Bash Installation

1. Once installation is complete, you can verify that Git Bash has been installed successfully:
    - Go to the Start menu.
    - Search for "Git Bash" or look for it in the installed programs list.
    - Open Git Bash to launch the terminal.
2. Alternatively, you can open a command prompt and type `git --version` to check if Git is installed and to see the installed version.

---
## Installing Terraform on Windows

### 1. Download Terraform Binary

- Go to the [Terraform Downloads](https://www.terraform.io/downloads.html) page on the official Terraform website.
- Download the Terraform binary for Windows.

### 2. Extract Terraform Binary

- Once downloaded, extract the contents of the zip file to a directory of your choice on your Windows system.

### 3. Add Terraform to PATH

- Open "System (Control Panel)" > "Advanced system settings" > "Environment Variables...".
- Under "System variables", select the `Path` variable and click "Edit...".
- Add the full path to the directory where Terraform binary (`terraform.exe`) is located.
- Click "OK" on all windows to apply the changes.

### 4. Verify Installation

- Open a new command prompt window.
- Type `terraform --version` and press Enter to verify that Terraform is installed correctly.

---

## Installing Terraform Extension for Visual Studio Code

### 1. Access Extensions View

- Open Visual Studio Code.
- Click on the square icon at the bottom of the sidebar to access the Extensions view.

### 2. Search for Terraform Extension

- Type "Terraform" into the search bar and press Enter.

### 3. Install Terraform Extension

- Look for the official HashiCorp Terraform extension and click "Install".

### 4. Verify Installation

- Reload Visual Studio Code if prompted.
- After reloading, you should see the Terraform extension listed in the Extensions view under "Installed".

---
## Installing AWS CLI on Windows

### Downloading and Installing AWS CLI

1. Visit the official AWS CLI installation guide [here](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).
2. Select the Windows operating system.
3. Open PowerShell in Windows as an administrator.
4. Execute the following command:
    ```
    msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
    ```
5. Follow the installation wizard instructions:
    - Click "Next" to proceed.
    - Accept the license agreement.
    - Click "Next" to accept the default installation directory.
    - Click "Install" to begin the installation process.
    - Wait for the installation to complete.
    - Click "Finish" to exit the installer.

### Verifying AWS CLI Installation

1. Close the PowerShell window.
2. Reopen PowerShell or open Git Bash.
3. Execute the command `aws --version` to verify the installation.
4. If AWS CLI is installed correctly, it will display the installed version.
---
## Creating IAM User and Configuring AWS CLI

This guide provides step-by-step instructions for creating an IAM user and configuring AWS CLI credentials.

### Creating IAM User:

1. Login to the AWS Management Console.
2. Navigate to the IAM service.
3. Click on "Users" from the left-hand menu.
4. Click on the "Add user" button.
5. Enter a username, e.g., "terraform".
6. Click "Next".
7. Uncheck the option for providing user access to the AWS Management Console.
8. Select "Attach policies directly".
9. Search for and select "AdministratorAccess" policy.
10. Click "Next".
11. Review the settings and click "Create user".
12. Click on the newly created "terraform" user.
13. Navigate to the "Security credentials" tab.
14. Click "Create access key".
15. Select "Programmatic access".
16. Click "Next: Permissions".
17. Enter a description tag value, e.g., "terraform credentials".
18. Click "Create access key".
19. Download the CSV file containing the access key ID and secret access key.
20. Store the CSV file securely.
21. Click "Done".

### Configuring AWS CLI:

1. Open Git Bash or your terminal of choice.
2. Execute the command `aws configure`.
3. Enter the access key ID from the downloaded CSV file.
4. Enter the secret access key from the downloaded CSV file.
5. Enter the default region, e.g., `us-east-1`.
6. Choose the default output format, e.g., `json`.

#### Ensure that you keep the access key and secret key securely and do not expose them publicly.
---
## MobaXterm Installation Guide for Windows

This guide provides step-by-step instructions for installing MobaXterm on a Windows system.

### Downloading MobaXterm:

1. Open your web browser.
2. Search for "MobaXterm download".
3. Visit the MobaXterm website [here](https://mobaxterm.mobatek.net/).
4. Choose the Home Edition for download.
5. Select the Installer Edition for a direct .exe file installation.

### Installing MobaXterm:

1. Once the download is complete, locate the downloaded .exe file.
2. Double-click on the installer file to start the installation process.
3. Follow the installation wizard instructions:
    - Click "Next" to proceed.
    - If prompted, remove any existing installations.
    - Accept the terms and conditions.
    - Choose the installation directory (default is recommended).
    - Click "Install" to begin the installation process.
    - Wait for the installation to complete.
    - Click "Finish" to exit the installer.

### Using MobaXterm:

- Search for "MobaXterm" in the Start menu or use the desktop shortcut (if created) to open the application.
- MobaXterm provides a terminal emulator with various features, including support for SSH, RDP, X11, and more.
- To connect to a remote system, click on the "Session" button and enter the IP address and load the required key pair.
- Further usage instructions will be provided in subsequent documents.

