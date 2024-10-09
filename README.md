# Hardened Ubuntu Autoinstall Configuration

This repository contains a configuration file for automated installation of a hardened Ubuntu system using the `autoinstall.yaml` file. This setup is designed for security and privacy, integrating essential packages and configurations to enhance the default Ubuntu experience.

## Project Overview

The `autoinstall.yaml` file enables the automated deployment of a secure and privacy-focused Ubuntu environment. It includes configurations for user creation, package installation, firewall setup, and more, making it easier to set up a secure system quickly.

### Key Features

- Automated installation of essential security packages:
  - OpenSSH Server
  - UFW (Uncomplicated Firewall)
  - Fail2Ban (Brute force attack protection)
  - Auditd (Auditing system)
  - Tor and OpenVPN for enhanced privacy
  - Firefox with a hardened `user.js` configuration for privacy
- Custom user creation with specific privileges
- Automatic updates for system security
- Configurations to disable unnecessary features that may compromise privacy

## Prerequisites

- A bootable Ubuntu installation medium (USB/DVD).
- Familiarity with Linux command-line and system administration.

## Installation Instructions

To install Ubuntu using the provided `autoinstall.yaml`, follow these steps:

1. **Prepare the Installation Medium**:
   - Create a bootable USB or DVD with the Ubuntu installation image. You can use tools like Rufus, Balena Etcher, or the `dd` command in Linux.

2. **Copy the Configuration File**:
   - Place the `autoinstall.yaml` file in the root of the bootable installation medium. The file should be accessible at:
     ```
     /autoinstall.yaml
     ```

3. **Boot from the Installation Medium**:
   - Insert the bootable USB or DVD into your target machine and boot from it. You may need to change the boot order in your BIOS/UEFI settings.

4. **Start the Installation**:
   - When the Ubuntu installer starts, it will automatically detect the `autoinstall.yaml` file and begin the installation process based on the specified configuration.

5. **Post-Installation**:
   - Once the installation is complete, log in with the username and password specified in the `autoinstall.yaml`. You can further customize your installation as needed.

## Additional Information

- For detailed explanations of the configurations in the `autoinstall.yaml` file, refer to the comments within the file.
- This project is maintained under the [MIT License](./License).

## Contribution

Contributions are welcome! Please submit a pull request or open an issue for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the [License](./License) file for more details.

