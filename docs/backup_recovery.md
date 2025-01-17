# Backup and Recovery Strategies

## Overview
This project involves setting up and managing full system image backups using Macrium Reflect Free and Acronis True Image. The project also includes simulating data loss, restoring from backups, and automating backup routines.

## Tools Used
- **Macrium Reflect Free**: Free backup software for creating system image backups.
- **Acronis True Image**: Comprehensive backup software with advanced features.

## Key Activities

### 1. Create Full System Image Backups

#### Using Macrium Reflect Free
1. **Install Macrium Reflect Free**:
   - Download and install from the official website.

2. **Create a Full System Image Backup**:
   - Open Macrium Reflect Free.
   - Click on the "Backup" tab.
   - Select the disk (e.g., C: drive).
   - Choose a save location (e.g., external drive).
   - Click "Create Backup Now."

3. **Schedule Daily and Weekly Backups**:
   - Click on the "Schedule" tab.
   - Set up a new schedule for daily incremental backups (e.g., 2:00 AM).
   - Set up a new schedule for weekly full backups (e.g., 1:00 AM on Sundays).
   - Enable email notifications.

#### Using Acronis True Image
1. **Install Acronis True Image**:
   - Download and install from the official website.

2. **Create a Full System Image Backup**:
   - Open Acronis True Image.
   - Click on "Backup" and select "Backup my disk."
   - Choose the disk (e.g., C: drive).
   - Select a save location (e.g., external drive or cloud storage).
   - Click "Backup Now."

3. **Schedule Daily and Weekly Backups**:
   - Click on "Schedule" and select "Create new schedule."
   - Set up a new schedule for daily incremental backups (e.g., 2:00 AM).
   - Set up a new schedule for weekly full backups (e.g., 1:00 AM on Sundays).
   - Enable notifications.

### 2. Simulate Data Loss and Restore from Backups

#### Simulate Data Loss
1. **Delete Files**:
   - Identify and delete non-critical files or folders to simulate data loss.

#### Restore from Backup
1. **Using Macrium Reflect Free**:
   - Open Macrium Reflect Free.
   - Click on the "Restore" tab.
   - Select the backup image.
   - Choose the files or folders to restore.
   - Click "Restore."

2. **Using Acronis True Image**:
   - Open Acronis True Image.
   - Click on "Restore" and select "Restore from backup."
   - Choose the backup image and the files or folders to restore.
   - Click "Restore."

### 3. Verify Backup Integrity
1. **Check Backup Logs**:
   - Review the backup logs in both Macrium Reflect Free and Acronis True Image to ensure backups completed successfully.
   - Verify the size and integrity of the backup files.

2. **Test Restored Files**:
   - Open and test the restored files to ensure they are intact and functional.

## Screenshots

### Creating a Full System Image Backup with Macrium Reflect Free
![Macrium Reflect Full Backup](../assets/screenshots/macrium_full_backup.png)

### Scheduling Backups with Macrium Reflect Free
![Macrium Reflect Schedule](../assets/screenshots/macrium_schedule.png)

### Creating a Full System Image Backup with Acronis True Image
![Acronis True Image Full Backup](../assets/screenshots/acronis_full_backup.png)

### Scheduling Backups with Acronis True Image
![Acronis True Image Schedule](../assets/screenshots/acronis_schedule.png)

### Restoring Files with Macrium Reflect Free
![Macrium Reflect Restore](../assets/screenshots/macrium_restore.png)

### Restoring Files with Acronis True Image
![Acronis True Image Restore](../assets/screenshots/acronis_restore.png)

