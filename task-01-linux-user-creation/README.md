# Task 1 - Linux User Setup

## Task Statement:
Create a custom Linux user for Apache/web hosting purposes.
 - User name: mariyam
 - Host: app server 2
 - unique UID: 1319
 - home dir: /var/www/mariyam

## Solution

Step 1: Connect to App Server 2

```bash
ssh user@hostname
password:
```
Step 2: Create the custom Apache User

```bash
sudo useradd -u 1319 -d /var/www/mariyam -m mariyam
```

Step 3: Verify the Configuration

```bash
id mariyam
grep mariyam /etc/passwd
```
Expectd Output:
```
mariyam:x:1319:1319::/var/www/mariyam:/bin/bash
```

# 🚀 Task completed successfully 🔥

## Skills Learned:
- Linux User management
- Custom UID assignment
- Home directory creation
- Basic server Administration