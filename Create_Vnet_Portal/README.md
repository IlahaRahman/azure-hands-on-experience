# Create Virtual Networks using Azure Portal

This task is part of a hands-on Azure networking lab, where I created a virtual network (`CoreServicesVnet`) and configured subnets using the Azure Portal. 

## Task Overview

- Sign into the Azure Portal
- Create a new resource group named az104-rg4
- Create a Virtual Network named `CoreServicesVnet` in the East US region
	![Create VNets](./Screenshots/Screenshot(294).png)
	![Create VNets](./Screenshots/Screenshot(295).png)
- Define a custom IPv4 address space (`10.20.0.0/16`)
- Add two subnets:
  - `SharedServicesSubnet`: `10.20.10.0/24`
	![Create VNets](./Screenshots/Screenshot(296).png)
  - `DatabaseSubnet`: `10.20.20.0/24`
	![Create VNets](./Screenshots/Screenshot(297).png)
- Remove the default subnet
	![Create VNets](./Screenshots/Screenshot(298).png)

- Validate and deploy the network
- Export and download the ARM template for future use
	![Create VNets](./Screenshots/Screenshot(299).png)


## 🛠 Steps Performed

1. **Logged into the Azure Portal**
2. **Created a new virtual network** named `CoreServicesVnet`
3. **Defined a custom address space** `10.20.0.0/16`
4. **Added two subnets**:
   - `SharedServicesSubnet` at `10.20.10.0/24`
   - `DatabaseSubnet` at `10.20.20.0/24`
5. **Deleted the default subnet**
6. **Reviewed and created** the VNet after validation
7. **Exported and downloaded** the deployment template (`template.json`) for use in future tasks.

## ✅ Outcome

Successfully deployed a virtual network and its associated subnets via the portal. The exported template will be used in the next task to deploy a similar network using Infrastructure as Code.
 
