# Network Monitoring Deployment

## Overview
This project involves deploying and configuring a network monitoring tool (Zabbix or PRTG Network Monitor) to monitor network traffic, CPU usage, and disk health. The project also includes simulating network issues and observing alerts for troubleshooting.

## Tools Used
- **Zabbix**: Open-source network monitoring solution.
- **PRTG Network Monitor**: Commercial network monitoring solution.

## Key Activities

### 1. Install and Configure Zabbix

#### Install Zabbix Server
1. **Virtual Machine Setup**:
   - Create a new virtual machine using VirtualBox or VMware.
   - Install a Linux distribution (e.g., Ubuntu Server) on the VM.
2. **Install Zabbix**:
   - Open a terminal and add the Zabbix repository:
     ```bash
     wget https://repo.zabbix.com/zabbix/6.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_6.0-4+ubuntu20.04_all.deb
     sudo dpkg -i zabbix-release_6.0-4+ubuntu20.04_all.deb
     sudo apt update
     ```
   - Install Zabbix server, frontend, and agent:
     ```bash
     sudo apt install zabbix-server-mysql zabbix-frontend-php zabbix-apache-conf zabbix-sqlite3-database zabbix-agent
     ```
   - Follow the prompts to set up the database and configure the server.

#### Configure Zabbix
1. **Access the Web Interface**:
   - Open a web browser and navigate to `http://<VM-IP>/zabbix`.
   - Follow the setup wizard to complete the initial configuration.
2. **Add Devices for Monitoring**:
   - Go to "Configuration" > "Hosts" > "Create host".
   - Add the IP addresses of the devices you want to monitor (e.g., laptops, phones).
   - Select appropriate templates for monitoring (e.g., "Template OS Linux" for Linux devices).

### 2. Install and Configure PRTG Network Monitor

#### Install PRTG
1. **Virtual Machine Setup**:
   - Create a new virtual machine using VirtualBox or VMware.
   - Install a Windows Server or Windows 10 on the VM.
2. **Install PRTG**:
   - Download the PRTG Network Monitor installer from the official website.
   - Run the installer and follow the prompts to complete the installation.

#### Configure PRTG
1. **Access the Web Interface**:
   - Open a web browser and navigate to `http://<VM-IP>:8080`.
   - Log in using the default credentials (admin/PRTGadmin).
2. **Add Devices for Monitoring**:
   - Go to "Setup" > "Devices" > "Add Device".
   - Add the IP addresses of the devices you want to monitor (e.g., laptops, phones).
   - Add sensors for monitoring network traffic, CPU usage, and disk health.

### 3. Simulate Network Issues

#### Disconnect Devices
- Unplug a network cable or turn off Wi-Fi on a device.
- Observe the alerts in Zabbix or PRTG.

#### Create High Bandwidth Usage
- Use tools like `iperf` to generate network traffic.
- Observe the network traffic graphs and alerts in Zabbix or PRTG.

### 4. Documentation and Reports

- **Network Issues Detected**:
  - Document the network issues detected during the simulation.
  - Include screenshots of the alerts and the devices involved.

- **Resolution Steps**:
  - Document the steps taken to resolve the network issues.
  - Include screenshots of the resolution process.

- **Bandwidth Usage Graphs**:
  - Generate and include bandwidth usage graphs from Zabbix or PRTG.
  - Analyze the graphs to understand the impact of high bandwidth usage.

## Screenshots

### Zabbix Installation
![Zabbix Installation](../assets/screenshots/zabbix_install.png)

### Zabbix Add Device
![Zabbix Add Device](../assets/screenshots/zabbix_add_device.png)

### PRTG Installation
![PRTG Installation](../assets/screenshots/prtg_install.png)

### PRTG Add Device
![PRTG Add Device](../assets/screenshots/prtg_add_device.png)

### Network Issues and Alerts
![Network Issues](../assets/screenshots/network_issues.png)

### Bandwidth Usage Graphs
![Bandwidth Usage](../assets/screenshots/bandwidth_usage.png)

