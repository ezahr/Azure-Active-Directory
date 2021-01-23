# Azure-Active-Directory


![airwatch](..//pictures/47474A80-D815-49B5-A7F1-F2C2B7B31133.png)



## Inschrijving voor Azure AD-integratie
Door integratie met Microsoft Azure Active Directory worden Windows-apparaten automatisch aangemeld bij Workspace ONE UEM met minimale interactie met de eindgebruiker. Inschrijving voor Azure AD-integratie vereenvoudigt de inschrijving voor zowel eindgebruikers als beheerders. Inschrijving voor Azure AD-integratie ondersteunt drie verschillende inschrijvingsstromen: deelnemen aan Azure AD, Out of Box Experience-inschrijving en Office 365-inschrijving. Voor alle methoden is configuratie van Azure AD-integratie met Workspace ONE UEM vereist.[Voordat u uw apparaten kunt inschrijven met behulp van Azure AD-integratie, moet u Workspace ONE UEM en Azure AD configureren](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/services/Windows_Desktop_Device_Management/GUID-AWT-ENROLL-OVERVIEWWD.html)


[Uw universele platform om identiteiten te beheren en te beveiligen](https://azure.microsoft.com/nl-nl/services/active-directory/)

De Azure Active Directory-bedrijfsidentiteitsservice (Azure AD) biedt eenmalige aanmelding en meervoudige verificatie om uw gebruikers te beschermen tegen 99,9 procent van de cyberbeveiligingsaanvallen.  U wordt geverifieerd op basis van uw Azure AD-tenant. De web-app vraagt ook om enkele toestemmingen, en u wordt om uw toestemming gevraagd.  Selecteer Accepteren. De webapp verschijnt dan. De titelbalk bevat uw geverifieerde gebruikersnaam, wat aangeeft dat u met succes bent aangemeld met de identiteit in de Learn Module AAD Tenant-directory.

## De soeverein is niet thuisSelf-Sovereign Identity (SSI) en Attribute Based Credentials (ABC)Mireille Hildebrand

Directory (Azure AD) is de cloudgebaseerde service voor identiteits- en toegangsbeheer van Microsoft. Het vereenvoudigt authenticatie voor ontwikkelaars door identiteit als een service te bieden. Het ondersteunt standaardprotocollen zoals OAuth 2.0 en OpenID Connect. Met Azure AD kunnen gebruikers zich aanmelden en bronnen bekijken. En het heeft functies om uw identiteiten te beveiligen, zoals identiteitsbescherming en meervoudige authenticatie. Microsoft-services zoals Azure en Microsoft 365 gebruiken Azure AD om gebruikers op te slaan en te beheren. Wanneer Microsoft 365 bijvoorbeeld een gebruiker moet verifiëren, voert Azure AD alle identiteits- en toegangsbeheer uit.
SSI zou het beheer van persoonsgegevens mogelijk moeten maken voor ‘gebruikers’, door die gegevens op te slaan op een blockchain en degene wiens gegevens het betreft de sleutel te geven waarmee anderen toegang kunnen verkrijg.  De I van SSI gaat niet over identiteit, maar over data die identificatie mogelijk maakt, dat wil zeggen data die het mogelijk maakt een persoon als uniek te onderscheiden van andere personen. Of data identificatie mogelijk maakt, verschilt per context
De beginselen van Allen zijn ontroerend in termen van goede bedoelingen maar geven weinig inzicht in wat SSI nu ei
ABC richt zich, anders dan SSI, niet alleen naar de wensen van de betrokkene. Naast de beperking van dataverwerking tot hetgeen noodzakelijk is gezien het verwerkingsdoel, richt ABC zich ook op de betrouwbaarheid van de verstrekte attributen. Een probleem dat noch SSI- noch ABC-systemen kunnen oplossen is de handel in gedragsgegevens. En laat dat nu juist één van de cruciale pijnpunten zijn van de huidige, gemankeerde informatieomgeving. Gedragsdata bestaat niet uit attributen die we zelfstandig ‘uploaden’ in de SSI- of ABC-applicatie. Integendeel, deze data wordt door anderen ‘gevangen’ op basis van spyware
ABC lijkt minder problemen te scheppen, maar de inzet van ABC-toepassingen hangt net als bij SSI af van de beschikbaarheid van een infrastructuur die ABC mogelijk maakt De verwarring rond consent hangt mogelijk samen met het feit dat voor gebruikers, dienstverleners en informatici het verrichten van een feitelijke handeling, zoals het klikken op een button, gelijk staat aan het geven van consent. Juridisch gezien ligt dat echter niet voor de hand
Bij ABC-systemen lijkt een evenwichtige afweging te zijn ingebouwd die de relationele aard van persoonsgegevens bevestigt en naïef soevereiniteitsdenken voorkomt

## Beveilig uw toepassingen door verificatie naar Azure AD te verplaatsen
Als uw organisatie momenteel Active Directory Federation Services (AD FS) gebruikt om aanmelding bij cloud-apps mogelijk te maken, kunt u upgraden naar Azure AD om het beheer te vereenvoudigen en uw on-premises footprint te verkleinen.
[Meer informatie over migratie naar Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/migration-resources)
https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Insights

Installeer AD FS Connect Health om aan de slag te gaan
Installeer eerst AD FS Connect Health op uw AD FS-servers om aan de slag te gaan. AD FS Connect Health helpt niet alleen bij het migreren van apps naar Azure AD, maar biedt ook:
AD FS-waarschuwingen
AD FS-analyse
Prestatie monitoring
Mislukte aanmeldingsgegevens


For those of you using Azure Active Directory (which includes everyone using Office 365), a number of capabilities enable remote work while helping you keep your organization secured.

 

|nr||Here are our top five recommendations for enabling remote work:|
|------------|-------------------------------------------------------------------------| 
| 1. | Use a common collaboration tool (like Microsoft Teams, Cisco Webex, Slack, Workplace by Facebook or Zoom) If your company hasn’t already broadly adopted a collaboration tool, standardizing on a common platform can reduce barriers across groups. If you’re not currently licensed to use Microsoft Teams, see here for details about free access.If you prefer tools like Cisco Webex, Slack, Workplace from Facebook, or Zoom, Azure AD integration provides federated single-sign-on (SSO) and automated user provisioning, allowing you to deploy to all your users quickly and give them frictionless access. Go here to learn about integrating apps with Azure AD.|
|2.| Enable your users to securely access cloud apps from outside your corporate network To protect your organization, it’s essential that when you enable access to cloud apps from personal devices and remote locations, it is done securely. If you’re already using Azure AD Conditional Access, you know it can be used to apply security policies to help ensure the right people have access to the apps they need, in line with your organizational requirements. You can extend your policies to protect all your apps, requiring controls like passing an MFA challenge or using a compliant device. For more information about Conditional Access, go here. If you’re not using Conditional Access, Security Defaults can help keep your users and apps secured (learn more here). If you already have Conditional Access rolled out in your organization, we recommend you examine your policies and ensure they’re not preventing remote access. Policies that block access when off the corporate network are common, and would cause problems. You may find that an alternative combination of Conditional Access controls will enable remote work, while still meeting your security requirements.|
|3.| Provide secure access to your on-premises apps from outside your corporate network Most organizations are running lots of business-critical apps on-premises, many of which may not be accessible from outside the corporate network. Azure AD Application Proxy is a lightweight agent that enables internet access to your on-premises apps, without opening up broad access to your network. You can combine this with your existing Azure AD authentication and Conditional Access policies to help keep your users and data secured. For more information about App Proxy, go here.  Alternatively, if you’re using Akamai Enterprise Application Access (EAA), Citrix Application Delivery Controller (ADC), F5 BIG-IP Access Policy Manager (APM) or Zscaler Private Access, Microsoft has partnerships to help you provide remote access securely. For more information about Secure Hybrid Access, .|
|4. |Collaborate with partners With many companies canceling non-essential business travel, working closely with business partners can become more difficult. Azure AD’s B2B collaboration capabilities can help you use your chosen collaboration app—including SharePoint, Teams, Box, Dropbox, and Google Drive—securely across company boundaries. For more information, go here.|
|5. |Support bring-your-own-device Not every organization can provide corporate devices for remote work, but you can enable access to company data on personally owned devices using Microsoft Intune app protection policies combined with Azure AD Conditional Access. |

 
The power of the cloud enables new ways to work, giving us flexibility in challenging times. We hope Azure AD can help keep your users productive — and your business moving. Stay safe and be well.


Attribute based credentials(ABC) is een systeem dat het mogelijk maakt om alleen die gegevens te delen die noodzakelijk zijn voor de te verlenen dienst
Het schermen met een term als SSI zal juristen gemakkelijk irriteren, want er is eenvoudigweg geen overeenstemming over de betekenis en er zijn ook geen operationele voorbeelden voorhanden
De metafoor van de soeverein, die vooropstaat bij de idee van SSI, is niet bijzonder productief. Deze metafoor suggereert namelijk een publiekrechtelijke relatie ten aanzien van persoonsgegevens die gebaseerd is op soevereine wil
Herhaaldelijk gaan stemmen op om de relatie tussen persoon en persoonsgegevens als een eigendomsrelatie te kwalificeren, vaak als goedbedoelde poging om meer bescherming te bieden. Dat zou meer problemen scheppen dan oplossen




##  Nu inschakelen Enable Azure Active Directory Premium trial (Engelstalige video)



|Bekijk in 5 eenvoudige stappen hoe u dit moet doen|
|----------------|
|Open Active Directory|
|Kies een map|
|Activeer de proefversie|
|Bevestig uw licenties|
|Wijs uw licenties toe|




