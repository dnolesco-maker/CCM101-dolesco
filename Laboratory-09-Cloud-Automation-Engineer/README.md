# Mission 9: The Cloud Automation Engineer

## 1. Mission Overview

This laboratory activity focuses on automating cloud operations using Bash scripting and Cron in a Linux environment. I created a backup script that compresses a sample data directory into a `.tar.gz` archive and configured a scheduled task to run the script automatically every day at 2:00 AM.

## 2. Objectives

- Understand Bash scripts and variables.
- Create a backup script using Nano.
- Learn how to grant execute permission using `chmod +x`.
- Generate compressed backups using `tar`.
- Schedule automated tasks using Cron.
- Document the process and upload the required files to GitHub.

## 3. Commands Executed

| Command | Purpose |
|---|---|
| `mkdir app-data` | Creates the sample data directory. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a sample data file. |
| `nano backup.sh` | Creates or edits the Bash script. |
| `chmod +x backup.sh` | Makes the script executable. |
| `./backup.sh` | Runs the backup script. |
| `ls -l backups/` | Lists the generated backup archives. |
| `env EDITOR=nano crontab -e` | Opens the Cron configuration for editing. |
| `crontab -l` | Displays the installed Cron schedule. |

## 4. Skills Learned

Through this activity, I learned how to automate a backup task using Bash scripting, create compressed archives, manage file permissions, and schedule recurring tasks with Cron. I also practiced documenting technical procedures and organizing project files in a GitHub portfolio.

## 5. Screenshots

- `screenshots/script-execution.png`: Shows the permission error, successful script execution, and generated backup archives.
- `screenshots/cron-schedule.png`: Shows the installed Cron schedule for the backup script.
