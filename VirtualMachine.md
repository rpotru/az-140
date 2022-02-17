Virtual Machines can be created in multiple ways using the GUI, command line or scripted/tools approach. Let us explore multiple ways of creation.

1) Using Azure Portal
   https://www.portal.azure.com


2) Scripted methodology 
   Using the Powershell/Bash/Azure CLI
```sh
New-AzVm `
    -ResourceGroupName 'labrg01' `
    -Name 'vmNew' `
    -Location 'East US' `
    -VirtualNetworkName 'vnet01' `
    -SubnetName 'default' `
    -SecurityGroupName 'nsg01' `
    -PublicIpAddressName 'publicip02' `
    -OpenPorts 3389
 ```
	
3) Azure ARM templates
  https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview

4) Terraform (IaC tool to deploy anything through code Azure/AWS/Google cloud)
```sh
terraform plan
terraform apply
```
