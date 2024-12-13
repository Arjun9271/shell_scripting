
# AWS CLI Installation Guide for Ubuntu

This guide provides step-by-step instructions to install AWS CLI on an Ubuntu system.

---

## Prerequisites

Ensure you have `curl` and `unzip` installed on your system. These tools will be used to download and extract the installer.

---

## Installation Steps

1. **Update Package List**  
   Run the following command to update your system's package list:
   ```bash
   sudo apt update
   ```

2. **Install Required Tools**  
   Install `curl` and `unzip` (if not already installed):
   ```bash
   sudo apt install curl unzip -y
   ```

3. **Download AWS CLI Installer**  
   Download the AWS CLI version 2 installer using `curl`:
   ```bash
   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   ```

4. **Extract the ZIP File**  
   Unzip the downloaded installer:
   ```bash
   unzip awscliv2.zip
   ```

5. **Run the Installer**  
   Install AWS CLI by executing the installation script:
   ```bash
   sudo ./aws/install
   ```

6. **Verify Installation**  
   Confirm the installation by checking the AWS CLI version:
   ```bash
   aws --version
   ```

---

## Additional Notes

- If any command fails, ensure you have administrative permissions (run commands with `sudo` as needed).
- For more details and troubleshooting, visit the [official AWS CLI documentation](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).

---

## Cleanup

After successful installation, you can remove the downloaded files to free up space:
```bash
rm -rf awscliv2.zip aws
```
