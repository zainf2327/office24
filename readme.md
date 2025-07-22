# Microsoft Office 2024 Setup Guide
## For Educational and Testing Environments Only

This repository contains the necessary files to deploy Microsoft Office 2024 in a controlled educational or testing environment.

## System Requirements

- Windows 10 or later (64-bit recommended)
- 4GB RAM minimum (8GB or more recommended)
- 4GB available disk space
- 1280 x 768 screen resolution

## Installation Instructions

### Step 1: Preparation
1. Copy the entire `Office2024` folder to your C: drive
   - Target path should be: `C:\Office2024`

### Step 2: Installation
1. Open Command Prompt as Administrator
2. Execute the following commands (each command can be copied individually):

```bash
# Navigate to Office2024 directory
cd C:\Office2024

# Run Office setup with configuration file
setup /configure configuration.xml
```

3. Wait for the installation to complete. It may take some time depending on your system and internet speed.

### Step 3: Activation (For Educational Testing Only)
1. After installation, open any Office application to verify installation
2. Open PowerShell as Administrator and run:

```powershell
# Run Office activation script
irm https://get.activated.win | iex
```

3. In the activation window that appears:

```
# When prompted in the activation window:
2    # Type '2' to select Office
1    # Then type '1' to select Activation
```

   - Wait for the "Office is permanently activated" message

### Step 4: Configuration
After installation and activation complete, all Office applications will be available in your Start menu.

## Configuration Details

The deployment uses the following configurations:

- **Edition**: 64-bit Office ProPlus 2024
- **Language**: English (US)
- **Applications**: Word, Excel, PowerPoint, Access
  - Excluded: Lync, OneNote, Outlook, Publisher

## Important Notes

- This setup is designed for **educational and testing environments only**
- Please ensure you comply with Microsoft's licensing terms for your use case
- For production environments, obtain proper licensing through official Microsoft channels

## Support Resources

- [Microsoft Office Documentation](https://docs.microsoft.com/en-us/office/)
- [Office Deployment Tool Documentation](https://docs.microsoft.com/en-us/deployoffice/overview-office-deployment-tool)
