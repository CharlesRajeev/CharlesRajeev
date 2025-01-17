# Active Directory Lab

## Overview
This project involves setting up an Active Directory (AD) lab environment using Windows Server and VirtualBox. The lab includes configuring Group Policies, creating user accounts, and simulating user login issues to practice troubleshooting.

## Tools Used
- **Windows Server**: Operating system for the domain controller.
- **Group Policy Management**: Tool for managing and configuring Group Policies.
- **VirtualBox**: Hypervisor for running the Windows Server virtual machine.

## Key Activities

### 1. Install Windows Server on VirtualBox
- **Download and Install VirtualBox**:
  - Visit the VirtualBox website and download the installer.
  - Follow the installation wizard to install VirtualBox on your host machine.
- **Create a New Virtual Machine (VM)**:
  - Open VirtualBox and click on "New."
  - Name your VM (e.g., "ADLab"), select "Microsoft Windows" as the type, and "Windows Server 2019" or "Windows Server 2022" as the version.
  - Allocate at least 2GB of RAM and create a new virtual hard disk with at least 40GB of space.
- **Install Windows Server**:
  - Download the Windows Server ISO from the Microsoft Evaluation Center.
  - Start your VM and mount the ISO file to the VM's virtual optical drive.
  - Follow the installation prompts to install Windows Server. Choose "Server with a GUI" for an easier setup experience.

### 2. Set Up Active Directory
- **Promote the Server to a Domain Controller**:
  - Open Server Manager and click on "Add roles and features."
  - Follow the wizard to add the "Active Directory Domain Services" role.
  - After the role is installed, open the "Active Directory Domain Services Configuration Wizard" and promote the server to a domain controller.
  - Create a new forest and domain name (e.g., `adlab.local`).
- **Verify AD Installation**:
  - Use the `dcdiag` command in PowerShell to verify that the domain controller is functioning correctly.

### 3. Configure Group Policies
- **Open Group Policy Management Console (GPMC)**:
  - In Server Manager, click on "Tools" and select "Group Policy Management."
- **Create a New GPO**:
  - Right-click on your domain (e.g., `adlab.local`) or a specific Organizational Unit (OU).
  - Select "Create a GPO in this domain, and Link it here."
  - Name the GPO (e.g., "Security Policies").
- **Configure Security Settings**:
  - **Restrict USB Access**:
    - Navigate to `User Configuration > Policies > Administrative Templates > System > Removable Storage Access`.
    - Enable the policy "Deny all access to all removable storage."
  - **Enforce Strong Password Policies**:
    - Navigate to `Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy`.
    - Set policies like "Minimum password length," "Password must meet complexity requirements," and "Maximum password age."

### 4. Create User Accounts and Manage Permissions
- **Create User Accounts**:
  - Open Active Directory Users and Computers (ADUC) from Server Manager.
  - Right-click on the domain and select "New > User."
  - Fill in the required details (e.g., first name, last name, username).
- **Manage Permissions**:
  - Right-click on a user or group and select "Properties."
  - Go to the "Security" tab to set permissions for resources like folders, files, or shared drives.

### 5. Simulate and Troubleshoot User Login Issues
- **Simulate a Login Issue**:
  - Try logging in with a user account and intentionally make a mistake (e.g., wrong password, account locked out).
- **Troubleshoot the Issue**:
  - **Check Event Viewer**:
    - Open Event Viewer and navigate to `Windows Logs > Security` to find error messages related to the login attempt.
  - **Unlock the Account**:
    - In ADUC, find the user account, right-click, and select "Unlock Account."
  - **Reset the Password**:
    - In ADUC, right-click the user account and select "Reset Password."

## Screenshots

### Installing Windows Server
![Installing Windows Server](../assets/screenshots/installing_windows_server.png)

### Promoting to Domain Controller
![Promoting to Domain Controller](../assets/screenshots/promote_to_dc.png)

### Creating a GPO
![Creating a GPO](../assets/screenshots/create_gpo.png)

### Configuring Group Policies
![Configuring Group Policies](../assets/screenshots/configure_gpo.png)

### Creating User Accounts
![Creating User Accounts](../assets/screenshots/create_user.png)

### Troubleshooting Login Issues
![Troubleshooting Login Issues](../assets/screenshots/troubleshoot_login.png)


