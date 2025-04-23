# Tech-Environment-Setup
## DevOps Mini-Project - 3MTT

This project sets up a DevOps environment for the 3MTT DevOps course. It includes development tools, a virtualized Ubuntu environment, and cloud accounts.

## Prerequisites
- **Operating System**: Windows 11
- **Hardware**: 16GB RAM, 4-core CPU, 20GB free disk space
- **Software**:
  - Visual Studio Code
  - Git
  - VirtualBox
  - Ubuntu 22.04 LTS (in VirtualBox)
- **Accounts**:
  - GitHub
  - AWS
- **Internet**: Stable connection

## Setup Instructions

All steps were performed on Windows 11.

### 1. Install Visual Studio Code
**Purpose**: Code editor for scripting and documentation.

1. Download from [code.visualstudio.com](https://code.visualstudio.com).
2. Run the installer and accept default settings.
3. Install extensions: GitLens, Markdown Preview Enhanced.

**Verification**:
- Open VS Code.
- Check version in terminal:
**Output**: `1.99.3`


![vscode](./img/1.%20VScode.png)

---

### 2. Install Git
**Purpose**: Version control for project files.

1. Download from [git-scm.com](https://git-scm.com).
2. Run the installer, keeping default settings.
3. Configure Git

**Verification**:
- Open Git Bash or Command Prompt.
- Run:
![Git bash](./img/2.%20Git%20Bash.png)


**Output**: `git version 2.45.2` (or similar)

---

### 3. Install VirtualBox
**Purpose**: Virtualization software to run Ubuntu.

1. Download VirtualBox 7.1.4 from [virtualbox.org](https://www.virtualbox.org).
2. Run the installer as Administrator.
3. **Issue Encountered**: Installer required Microsoft Visual C++ 2019 Redistributable.
 - **Screenshot**: [VirtualBox Error](img/virtualbox-error.png)
 - **Fix**: Downloaded Visual C++ 2019 Redistributable (x64) from [Microsoft](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist).
 - Installed `vc_redist.x64.exe` and restarted VirtualBox installation.
4. Complete the installation.

**Verification**:
- Open VirtualBox.
- Check version via Help > About.
**Output**: `7.1.8` (or similar)

---

### 4. Set Up Ubuntu in VirtualBox
**Purpose**: Linux environment for DevOps tasks.

1. Download Ubuntu 22.04 ISO from [Ubuntu.com](https://ubuntu.com/download/desktop).
2. In VirtualBox, create a new VM:
 - Name: Ubuntu-3MTT
 - Type: Linux, Ubuntu (64-bit)
 - RAM: 4GB
 - CPU: 2 cores
 - Disk: 20GB (dynamic)
3. Mount the Ubuntu ISO and start the VM.
4. Follow Ubuntu installer prompts (default settings).

**Verification**:
- Boot the VM and log into Ubuntu.
- Open a terminal and run: