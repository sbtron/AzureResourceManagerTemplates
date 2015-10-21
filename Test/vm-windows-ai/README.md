# Test Templates only
These are test templates meant to try out new configurations

### application-insights

Creates an application insights resource

| Name   | Description    |
|:--- |:---|
| newStorageAccountName  | Unique Name for the Application Insights Resource that will be created. |

Outputs the Instrumentation Key for the resource created.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsbtron%2FAzureResourceManagerTemplates%2Fmaster%2FTest%2Fvm-windows-ai%2Fvm-windows-ai%2FTemplates%2FApplicationInsightsResource.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>


### vm-windows-ai

Creates a Windows VM, and XML WAD config that accepts storage account and AI Ikey

| Name   | Description    |
|:--- |:---|
| newStorageAccountName  | Unique DNS Name for the Storage Account where the Virtual Machine's disks will be placed. |
| adminUsername  | Username for the Virtual Machines  |
| adminPassword  | Password for the Virtual Machine  |
| dnsNameForPublicIP  | Unique DNS Name for the Public IP used to access the Virtual Machine. |
| WindowsOSVersion  | Version of Windows to use. |
| DiagnosticsStorageAccountName  | Specify the storage account where diagnostics data will be transfered. The Diagnostics Account must exist and must be deployed separately from this template. You can default to specifying the same storage account as newStorageAccountName |
| DiagnosticsStorageResourceGroup  | Specify the resource group for the diagnostics storage account. If you use the same storage account as newStorageAccountName then specify the same resource group name here |
| ApplicationInsightsInstrumentationKey  | Specify the Instrumentation Key for Application Insights resource where the diagnostics data will be piped. The Application Insights resource must exist and must be deployed separately from this template (for e.g. using the application-insights template above which outputs the instrumentation key for the application insights resource created). |


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsbtron%2FAzureResourceManagerTemplates%2Fmaster%2FTest%2Fvm-windows-ai%2Fvm-windows-ai%2FTemplates%2FWindowsVirtualMachine.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>



