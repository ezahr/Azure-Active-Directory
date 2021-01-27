[get-list-of-registered-azure-ad-apps-powershel](https://morgantechspace.com/2018/04/get-list-of-registered-azure-ad-apps-powershell.html)

Een powershell-script delen om de lijst met Azure AD-toepassingen te vinden en op te halen die door uw bedrijf 
in de huidige tenant zijn geregistreerd. We kunnen de cmdlet Get-AzureADApplication gebruiken om alle geregistreerde apps op te halen.

````
$Result=@()
$Users = Get-AzureADUser -All $true | Select UserPrincipalName,ObjectId
$Users | ForEach-Object {
$user = $_
Get-AzureADUserRegisteredDevice -ObjectId $user.ObjectId | ForEach-Object {
$Result += New-Object PSObject -property @{ 
DeviceOwner = $user.UserPrincipalName
DeviceName = $_.DisplayName
DeviceOSType = $_.DeviceOSType
ApproximateLastLogonTimeStamp = $_.ApproximateLastLogonTimeStamp
}
}
}
$Result | Select DeviceOwner,DeviceName,DeviceOSType,ApproximateLastLogonTimeStamp
````

![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_12.png)

## Install-Module -Name AzureAD



## PS C:\WINDOWS\system32> connect-AzureAD

````
PS C:\WINDOWS\system32> connect-AzureAD

Account                 Environment TenantId                             TenantDomain AccountType
-------                 ----------- --------                             ------------ -----------
bosch.peter@outlook.com AzureCloud  f8cdef31-a31e-4b4a-93e4-5f571e91255a              User


PS C:\WINDOWS\system32>
````

## PS C:\Users\boscp08> get-module -listavailable
## Get-AzureADUser -Filter "userPrincipalName eq 'twarner@boschpeteroutlook.onmicrosoft.com'"

## get-azure-ad-users-with-registered-devices-powershell.
[get-azure-ad-users-with-registered-devices-powershell](https://morgantechspace.com/2019/06/get-azure-ad-users-with-registered-devices-powershell.html)


````
n this post, I am going to share Powershell script to find and list devices that are registered by Azure AD users. We can use the Get-AzureADUserRegisteredDevice cmdlet to get the registered devices.

Before proceed run the below command to connect Azure AD Powershell module.

Connect-AzureAD

The below command gets the devices that are registered to the specified user.

$user = Get-AzureADUser -SearchString "UserName"
Get-AzureADUserRegisteredDevice -ObjectId  $user.ObjectId -All $true
List registered devices of all Azure AD users:

To get a report of the device list for all Azure AD users, first, 
we need to get users by Get-AzureADUser cmdlet 
and pipe the user list to Get-AzureADUserRegisteredDevice cmdlet.

$Result=@()
$Users = Get-AzureADUser -All $true | Select UserPrincipalName,ObjectId
$Users | ForEach-Object {
$user = $_
Get-AzureADUserRegisteredDevice -ObjectId $user.ObjectId | ForEach-Object {
$Result += New-Object PSObject -property @{ 
DeviceOwner = $user.UserPrincipalName
DeviceName = $_.DisplayName
DeviceOSType = $_.DeviceOSType
ApproximateLastLogonTimeStamp = $_.ApproximateLastLogonTimeStamp
}
}
}
$Result | Select DeviceOwner,DeviceName,DeviceOSType,ApproximateLastLogonTimeStamp


Export Report to CSV file:

You can export the result to CSV file using the command Export-CSV.
1
	
$Result | Export-CSV "C:\AzureADJoinedDevices.csv" -NoTypeInformation -Encoding UTF8
 

````


![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_00.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_01.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_02.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_03.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_04.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_05.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_06.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_07.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_08.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_09.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_10.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_11.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_12.png)
![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_13.png)
[![cloud powershell](./../pictures/Azure_Active_Directory_gateway_on_powershell_14.png)](https://devblogs.microsoft.com/dotnet/azure-active-directorys-gateway-service-is-on-net-core-3-1/)

