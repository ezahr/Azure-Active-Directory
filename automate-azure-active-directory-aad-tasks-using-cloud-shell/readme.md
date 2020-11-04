## Automate-azure-active-directory-aad-tasks-using-cloud-shell


[automate-azure-active-directory-aad-tasks-using-cloud-shell](https://www.sqlshack.com/automate-azure-active-directory-aad-tasks-using-cloud-shell/)


Introduction
In the article How to create an Azure SQL Database using the Cloud Shell, we learned how to work with the Cloud Shell. In this new article, we will show how to automate Azure Active Directory tasks (AAD) using the Cloud Shell. We will work with loops, files and variables to automate tasks.

The following tasks will be included:

Show the list of Azure Active Directory Users
Show a specific Azure Active Directory user with a specific User principal name or Object ID
Create an Azure Active Directory User
Create an Azure Active Directory User using variables
Create multiple Azure Active Directory users from a list
Create an Azure Active Directory Group
Show Active Directory Groups in different formats
Filter results
Add Azure Active Directory Users to an Azure Active Directory Group
Check the Azure Active Directory User/Group Administrator in Azure SQL
Remove the Azure Active Directory User/Group Administrator in Azure SQL


## az login 

![tt](./../pictures/az_login_01.png)
![tt](./../pictures/az_login_00.png)
![tt](./../pictures/az_login_02.png)
![tt](./../pictures/az_login_03.png)
![tt](./../pictures/az_login_04.png)
![tt](./../pictures/az_login_05.png)
![tt](./../pictures/az_login_06.png)
![tt](./../pictures/az_login_07.png)
![tt](./../pictures/az_login_08.png)

## az ad user list 

Show the list of Azure Active Directory Users
We will first list all the Azure AD Users using the following command:

````
boscp08@kubernetes-worker2:~$ az ad user list
[
  {
    "accountEnabled": true,
    "ageGroup": null,
    "assignedLicenses": [
      {
        "disabledPlans": [],
        "skuId": "16ddbbfc-09ea-4de2-b1d7-312db6112d70"
      }
    ],
    "assignedPlans": [
      {
        "assignedTimestamp": "2020-09-29T08:55:10Z",
        "capabilityStatus": "Enabled",
        "service": "TeamspaceAPI",
        "servicePlanId": "4fa4026d-ce74-4962-a151-8e96d57ea8e4"
      },
      {
        "assignedTimestamp": "2020-09-29T08:55:10Z",
        "capabilityStatus": "Enabled",
        "service": "WhiteboardServices",
        "servicePlanId": "36b29273-c6d0-477a-aca6-6fbe24f538e3"
      },
      {
        "assignedTimestamp": "2020-09-29T08:55:10Z",
        "capabilityStatus": "Enabled",
        "service": "SharePoint",
        "servicePlanId": "902b47e5-dcb2-4fdc-858b-c63a90a2bdb9"
      },
      {
        "assignedTimestamp": "2020-09-29T08:55:10Z",
        "capabilityStatus": "Enabled",
        "service": "MicrosoftCommunicationsOnline",
        "servicePlanId": "617d9209-3b90-4879-96e6-838c42b2701d"
      }
    ],
    "city": null,
    "companyName": null,
    "consentProvidedForMinor": null,
    "country": null,
    "createdDateTime": "2019-10-17T15:06:09Z",
    "creationType": null,
    "deletionTimestamp": null,
    "department": null,
    "dirSyncEnabled": null,
    "displayName": "Peter Bosch",
    "employeeId": null,
    "facsimileTelephoneNumber": null,
    "givenName": "Peter",
    "immutableId": null,
    "isCompromised": null,
    "jobTitle": null,
    "lastDirSyncTime": null,
    "legalAgeGroupClassification": null,
    "mail": "bosch.peter@outlook.com",
    "mailNickname": "bosch.peter_outlook.com#EXT#",
    "mobile": null,
    "objectId": "a4dd55d4-80ba-430f-9ebb-ce1d227d2111",
    "objectType": "User",
    "odata.type": "Microsoft.DirectoryServices.User",
    "onPremisesDistinguishedName": null,
    "onPremisesSecurityIdentifier": null,
    "otherMails": [
      "bosch.peter@outlook.com"
    ],
    "passwordPolicies": null,
    "passwordProfile": null,
    "physicalDeliveryOfficeName": null,
    "postalCode": null,
    "preferredLanguage": "en",
    "provisionedPlans": [
      {
        "capabilityStatus": "Enabled",
        "provisioningStatus": "Success",
        "service": "SharePoint"
      }
    ],
    "provisioningErrors": [],
    "proxyAddresses": [
      "SMTP:bosch.peter@outlook.com"
    ],
    "refreshTokensValidFromDateTime": "2019-10-17T15:06:09Z",
    "showInAddressList": null,
    "signInNames": [],
    "sipProxyAddress": null,
    "state": null,
    "streetAddress": null,
    "surname": "Bosch",
    "telephoneNumber": null,
    "thumbnailPhoto@odata.mediaEditLink": "directoryObjects/a4dd55d4-80ba-430f-9ebb-ce1d227d2111/Microsoft.DirectoryServices.User/thumbnailPhoto",
    "usageLocation": "NL",
    "userIdentities": [],
    "userPrincipalName": "bosch.peter_outlook.com#EXT#@boschpeteroutlook.onmicrosoft.com",
    "userState": null,
    "userStateChangedOn": null,
    "userType": "Member"
  }
]
bo
````

## Show a specific Azure Active Directory user with a specific User principal name or Object ID

## Create an Azure Active Directory User

## Create an Azure Active Directory User using variables


## Create multiple Azure Active Directory users from a list

## Create an Azure Active Directory Group

## Show Active Directory Groups in different formats

## Filter results

## Add Azure Active Directory Users to an Azure Active Directory Group

## Check the Azure Active Directory User/Group Administrator in Azure SQL

##Remove the Azure Active Directory User/Group Administrator in Azure SQL

