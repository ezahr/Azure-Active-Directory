
## the AD creation process

[2-create-aad](https://docs.microsoft.com/en-us/learn/modules/manage-users-and-groups-in-aad/2-create-aad)


An organization (tenant) always has one default Azure AD directory it's associated with, however owners can create additional directories to support development or testing purposes, or because they want to have separate directories to synchronize with their local Windows Server AD forests.


The steps to create a new directory are shown below, however unless you are an owner of your Azure account, this option won't be available to you. The Azure Sandbox doesn't allow you to create new Azure AD directories.

##    Sign into the Azure portal .  https://portal.azure.com/#home

![tt](../../pictures/Sign-into-the-Azure-portal-https-porta-azure-com-home.png)

##    Select Create a resource from the left sidebar, Identity from the Azure Marketplace, and then Azure Active Directory from the list.


![tt](../../pictures/AZ_resource_Azure_Active_Directory_from_the_list.png)


````
Azure Active Directory is an Identity and Access Management as a service (IDaaS) solution that extends your on-premises directories into the cloud and provides single sign-on to Azure, Office 365 and thousands of cloud (SaaS) apps and access to web apps you run on-premises.
Built for ease of use, Azure Active Directory enables enterprise mobility and collaboration and delivers advanced identity protection through multi-factor authentication (MFA), security reports, audits, alerts and adaptive conditional access policies based on device health, user location and risk level.
````

![tt](../../pictures/Identity-and-Access-Management-as-a-service-IDaaS.png)

    
##    Choose a name for the directory that will help distinguish it from your other directories. If the directory you're creating is to be used in production, choose a name for the directory that your users will recognize as the name of your organization. You can change the name later if you want.





## Enter the domain name associated with it. The domain must not be known to Azure or you will get a validation error. The default domain name will always have the suffix .onmicrosoft.com. While this default domain cannot be changed, later you can add a custom domain owned by your organization so defined users can use a traditional company email such as john@contoso.com.


## Select the country the directory should reside in. This will identify the region and data center where the Azure AD instance will live and it cannot be changed later.
    Screenshot showing the AD creation process


## Select Create to create the new directory. This will create a free tier directory where you can add users, create roles, register apps and devices, and control licenses.

