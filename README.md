Windows Subsystem for Linux (WSL) allows you to run a Linux distribution alongside your Windows installation without the need for a virtual machine. Here’s how you can install and set up WSL on your Windows machine using PowerShell:

### Step-by-Step Guide to Installing WSL

1. **Open PowerShell as Administrator**
   - Press `Windows + X` and select `Windows PowerShell (Admin)`.

2. **Enable the WSL Feature**
   - Run the following command to enable the WSL feature:
     ```powershell
     dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
     ```
   - Next, enable the Virtual Machine Platform feature (required for WSL 2):
     ```powershell
     dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
     ```

3. **Restart Your Computer**
   - A restart is necessary for the changes to take effect.

4. **Set WSL 2 as the Default Version**
   - After restarting, open PowerShell as Administrator again and run:
     ```powershell
     wsl --set-default-version 2
     ```

5. **Install a Linux Distribution**
   - You can install a Linux distribution from the Microsoft Store. For example, to install Ubuntu:
     ```powershell
     wsl --install -d Ubuntu
     ```
   - Alternatively, you can open the Microsoft Store, search for a distribution (e.g., Ubuntu, Debian, Kali Linux), and install it from there.

6. **Launch Your Linux Distribution**
   - Once installed, you can launch your Linux distribution from the Start menu or by running:
     ```powershell
     wsl
     ```
   - The first time you launch your Linux distribution, you will be prompted to create a new user account and password.

### Example Commands

- **Check WSL Version**
  ```powershell
  wsl --list --verbose
  ```
  This will list all installed distributions and their WSL versions.

- **Update WSL Kernel**
  ```powershell
  wsl --update
  ```

- **Set a Specific Distribution to Use WSL 2**
  ```powershell
  wsl --set-version <distribution-name> 2
  ```
  Replace `<distribution-name>` with the name of your distribution, such as `Ubuntu`.

- **List All Installed Distributions**
  ```powershell
  wsl --list --all
  ```

- **Unregister (Uninstall) a Distribution**
  ```powershell
  wsl --unregister <distribution-name>
  ```

### Example Usage in WSL

Once inside your WSL distribution, you can use common Linux commands. Here are a few examples:

- **Update Package Lists (Ubuntu)**
  ```bash
  sudo apt update
  ```

- **Install a Package (e.g., Git)**
  ```bash
  sudo apt install git
  ```

- **Navigate File System**
  ```bash
  cd /mnt/c
  ls
  ```

- **Edit Files with nano or vim**
  ```bash
  nano filename
  vim filename
  ```

By following these steps, you will have WSL installed and configured on your Windows machine, allowing you to run Linux applications and tools seamlessly. 
