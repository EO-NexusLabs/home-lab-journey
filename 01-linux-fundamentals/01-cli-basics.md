# Lab 01: Linux Filesystem Hierarchy Standard (FHS) & CLI Basics

## 🎯 Objective
Understand and replicate the standard Linux directory structure (FHS) used in enterprise server environments, practicing core file and directory manipulation commands.

## 📐 Enterprise FHS Terminology
- `/etc`: Main directory for host-specific **system configuration files**.
  - `/etc/nginx/sites-available`: Directory holding Nginx virtual host configurations.
  - `/etc/sysctl.d`: Directory containing kernel parameter runtime configurations.
- `/var`: Contains **variable data files** generated during system operations.
  - `/var/log`: Centralized directory for system and application log files.

## 🛠️ Key Commands & Flags Executed
- `pwd`: Print absolute path of current working directory.
- `ls -lah`: List all entries with detailed metadata, hidden files (`.`), and human-readable file sizes.
- `mkdir -p`: Create parent directories recursively without throwing errors if they exist.
- `touch`: Instantiate empty files or update file timestamps.
- `rm -rf`: Forcefully remove directories and their contents recursively.

## 🧪 Hands-on Lab Operations
1. Created an authentic Linux FHS layout under `fhs-simulation/`.
2. Provisioned system configuration placeholders in `etc/`.
3. Created application log targets in `var/log/nginx/`.
4. Cleaned up non-standard legacy directories (`server-config/`, `logs/`).

## 📝 Key Takeaways
- Always adhere to FHS naming conventions (`/etc`, `/var`, `/usr`, `/opt`) to maintain industry standards and cross-platform consistency.
- Separation of configuration (`/etc`) and runtime state/logs (`/var`) is mandatory for security, backups, and storage partition management.
