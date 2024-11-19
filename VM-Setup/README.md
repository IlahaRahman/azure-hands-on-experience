## Virtual Machine Setup

This guide explains how to create and configure a Virtual Machine (VM) in Azure.

## Steps

### 1. Login to Azure Portal
- Go to [Azure Portal](https://portal.azure.com/) and log in.

### 2. Create a Resource Group
- Navigate to **Resource Groups** and click **+ Create**.
- Name the resource group `MyAzureVM-RG`.

### 3. Create a Virtual Machine
- Go to **Virtual Machines** and click **+ Add**.
- Fill in the following:
  - **VM Name:** `MyFirstVM`
  - **Region:** East US
  - **Image:** Ubuntu 20.04
  - **Size:** B1s (basic tier)
  - **Username:** `adminuser`
  - **Authentication:** Password-based login

### 4. Configure Networking
- Use default settings for the virtual network.
- Ensure ports are open for RDP/SSH.

### 5. Connect to the VM
- Use the public IP and credentials to connect via SSH or RDP.

### 6. Stop or Delete the VM
- Stop or delete the VM when no longer needed to avoid charges.
