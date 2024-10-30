# SSH-Auth-Manager

**SSH-Auth-Manager** is a simple and interactive Bash script that allows you to enable or disable password-based authentication on your SSH server. This tool is especially useful for quickly configuring SSH access security on cloud instances, such as AWS Lightsail or EC2.

## Features

- Enables password-based authentication for SSH with a single command
- Disables password-based authentication to enforce SSH key usage
- Automatically restarts the SSH service to apply changes
- Easy-to-use interactive prompts

## Requirements

- A Linux server with `bash` and `systemctl` (default for most modern Linux distributions)
- `sudo` privileges to modify SSH configuration

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/SSH-Auth-Manager.git
   cd SSH-Auth-Manager
