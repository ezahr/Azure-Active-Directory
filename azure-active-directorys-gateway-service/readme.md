https://devblogs.microsoft.com/dotnet/azure-active-directorys-gateway-service-is-on-net-core-3-1/

## De gatewayservice van Azure Active Directory is een omgekeerde proxy voor honderden services waaruit Azure Active Directory (Azure AD)
De gatewayservice van Azure Active Directory is een omgekeerde proxy voor honderden services waaruit Azure Active Directory (Azure AD) bestaat. 
Als u services zoals office.com, outlook.com, azure.com of xbox.live.com heeft gebruikt, heeft u de gateway van Azure AD gebruikt. 
De gateway biedt functies zoals TLS-beëindiging, automatische failovers / nieuwe pogingen, geo-nabijheidsroutering, 
beperking en tarpitting naar services in Azure AD. De gateway is aanwezig in meer dan 53 Azure-datacentra 
over de hele wereld en verwerkt dagelijks ~ 115 miljard verzoeken. Tot voor kort draaide de gateway van Azure AD op .NET Framework 4.6.2. 
Vanaf september 2020 draait het op .NET Core 3.1.  ;-)
Motivatie voor porten naar .NET Core
De schaal van uitvoering van de gateway resulteert in een aanzienlijk verbruik van rekenbronnen, 
wat op zijn beurt weer geld kost. Het vinden van manieren om de kosten van het uitvoeren van de service te verlagen, 
was een belangrijk doel voor het team erachter. Het geroezemoes rond .NET Core's focus op prestaties trok onze aandacht, 
vooral omdat TechEmpower ASP.NET Core noemde als een van de snelste webframeworks ter wereld. 
We hebben onze eigen benchmarks uitgevoerd op gateway-prototypes op .NET Core en de resultaten maakten de beslissing 
erg gemakkelijk: we moeten onze service overzetten naar .NET Core

U kunt de gateway van Azure AD niet als een resource maken in Azure Portal. Het is een omgekeerde proxy die wordt 
gebruikt door andere openbare services die deel uitmaken van Azure AD. Wanneer u die services gebruikt (bijvoorbeeld Azure AD B2C), 
worden de aanvragen automatisch doorgestuurd naar de gateway. 
