# Test Templates only
These are test templates meant to try out new configurations



### vm-ai-windows

Creates a Windows VM, and AI resource and XML WAD config that transfers data to the AI resource created.

| Name   | Description    |
|:--- |:---|
| newStorageAccountName  | Unique DNS Name for the Storage Account where the Virtual Machine's disks will be placed. |
| adminUsername  | Username for the Virtual Machines  |
| adminPassword  | Password for the Virtual Machine  |
| dnsNameForPublicIP  | Unique DNS Name for the Public IP used to access the Virtual Machine. |
| WindowsOSVersion  | Version of Windows to use. |



<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsbtron%2FAzureResourceManagerTemplates%2Fmaster%2FTest%2Fvm-ai-windows%2Fvm-ai-windows%2FTemplates%2FWindowsVirtualMachine.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
