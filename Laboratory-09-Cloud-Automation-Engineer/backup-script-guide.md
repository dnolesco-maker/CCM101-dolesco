# Backup Script Guide

## 1. Purpose of the Script

The `backup.sh` script automates the process of backing up the `app-data` directory. It creates a compressed `.tar.gz` archive inside the `backups` directory and adds a timestamp to the filename so each backup can be identified.

## 2. Bash Script

```bash
#!/bin/bash

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p $BACKUP_DIR

tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. Making the Script Executable

The command `chmod +x backup.sh` grants execute permission to the script, allowing it to run using `./backup.sh`. Without execute permission, attempting to run the script directly results in a `Permission denied` error.

## 4. Scheduling with Cron

The following cron expression schedules the backup script to run every day at 2:00 AM.

```bash
0 2 * * * /root/backup.sh
```

The five fields represent the following:

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

## 5. Commands Used

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -e
crontab -l
```

These commands create sample data, edit the script, grant execution permission, run the backup, inspect the generated archives, and verify the scheduled task.
