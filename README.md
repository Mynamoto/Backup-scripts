# Backup-scripts
Backup routines

# 🧩 Backup Scripts for Sysadmins

A collection of simple and effective bash scripts designed to help system administrators automate and manage their backup routines on Linux systems.

---

## 📁 Scripts Included

### 1. `daily_backup.sh`
Creates a daily compressed backup of a specified directory with a timestamp in the filename.

**Usage:**
```bash
bash daily_backup.sh /source/directory /backup/destination
```

### 2. `check_backup_status.sh`
Checks if the most recent backup file exists and was created within the last 24 hours. Useful for cron monitoring.

**Usage:**
```bash
bash check_backup_status.sh /backup/destination
```

### 3. `delete_old_backups.sh`
Deletes backup files older than X days (default: 7 days).

**Usage:**
```bash
bash delete_old_backups.sh /backup/destination 7
```

### 4. `remote_backup_rsync.sh`
Performs an incremental backup to a remote server using `rsync` over SSH.

**Usage:**
```bash
bash remote_backup_rsync.sh /local/folder user@remote:/path/to/backup
```

### 5. `backup_log_report.sh`
Generates a log summary of backup activities for the last 7 days.

**Usage:**
```bash
bash backup_log_report.sh /var/log/backup/
```

---

## ✅ Features
- Compatible with most Linux distros
- Easy to customize and expand
- Suitable for cron jobs and daily automation
- Clear logging (extendable with email/webhook alerts)

---

## 💡 Getting Started
To use the scripts:
1. Clone the repository:
```bash
git clone https://github.com/seuusuario/backup-scripts.git
cd backup-scripts
```
2. Make the scripts executable:
```bash
chmod +x *.sh
```
3. Customize paths and settings inside each script as needed.

---

## 📬 Contact
Created by [Fábio] - For educational and professional use. Contributions are welcome!

---

## 🧾 License
MIT License

