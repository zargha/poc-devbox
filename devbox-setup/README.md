# DevBox Setup Documentation

This project provides a configuration for setting up a Microsoft DevBox with essential development tools. The DevBox includes Rancher Desktop, WSL2, Visual Studio Code, SQL Server Management Studio, NVM (Node Version Manager), and .NET SDK version 6.0.201.

## Project Structure

```
devbox-setup
├── imagedefinition.yaml      # Configuration for the DevBox image
├── scripts                   # Contains installation scripts
│   ├── install-nvm.ps1      # Script to install NVM
│   ├── install-dotnet.ps1    # Script to install .NET SDK 6.0.201
│   └── install-ssms.ps1      # Script to install SQL Server Management Studio
└── README.md                 # Project documentation
```

## Setup Instructions

1. **Create the DevBox**: Use the `imagedefinition.yaml` file to create a Microsoft DevBox in Azure. This file defines the necessary tasks to install the required software.

2. **Run Installation Scripts**: After the DevBox is created, you can run the following PowerShell scripts to install additional tools:

   - To install NVM, run:
     ```
     .\scripts\install-nvm.ps1
     ```

   - To install .NET SDK 6.0.201, run:
     ```
     .\scripts\install-dotnet.ps1
     ```

   - To install SQL Server Management Studio, run:
     ```
     .\scripts\install-ssms.ps1
     ```

## Additional Information

- Ensure that you have the necessary permissions to create and configure resources in Azure.
- Follow the instructions in each script for any additional configuration that may be required after installation.

This README provides a high-level overview of the project and instructions for setting up the DevBox environment. For detailed usage of each tool, please refer to their respective documentation.