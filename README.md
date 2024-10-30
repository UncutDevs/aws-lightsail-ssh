# SSH-Auth-Manager

**SSH-Auth-Manager** is a simple and interactive Bash script that allows you to enable or disable password-based authentication on your SSH server. This tool is especially useful for quickly configuring SSH access security on cloud instances, such as AWS Lightsail or Google Cloud.

## Features

- Enables password-based authentication for SSH with a single command
- Disables password-based authentication to enforce SSH key usage
- Automatically restarts the SSH service to apply changes
- Easy-to-use interactive prompts

## Requirements
- A Linux server with `bash` and `systemctl` (default for most modern Linux distributions)
- `sudo` privileges to modify SSH configuration

## Usage
1. Login to your VPS using AWS Lightsail SSH Connect 
2. Set password for your linux user using this command ```passwd``` and update the password for your user : ubuntu, debian etc...
3. Run this command directly
   ```bash
   wget -O ssh-auth.sh https://raw.githubusercontent.com/UncutDevs/aws-lightsail-ssh/refs/heads/main/ssh-auth && sh ssh-auth.sh
   ```
4. Now you can login using password or you can also disable it as well for security.

## For Enabling Root User Direct Login
**NOTE**
This script does not allow direct root login if you want to login diectly as root then you can run this followin code:

1. Set a new root password first by loggin in as root user and running this command
**passwd**
2. Run this command
```bash
   wget -O root-ssh-auth.sh https://raw.githubusercontent.com/UncutDevs/aws-lightsail-ssh/refs/heads/main/root-ssh-auth && sh root-ssh-auth.sh
```
3. Now you can login as direct root user.


