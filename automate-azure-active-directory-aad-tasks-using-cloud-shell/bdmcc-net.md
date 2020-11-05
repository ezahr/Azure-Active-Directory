
.

## az login --username bosch.peter@outlook.com -t 69aaa45e-5377-432d-9882-57d002892515 --allow-no-subscriptions

## az login --username p.bosch@bdmcc.net -t adc7bffd-2d17-4df5-af5c-f450dcf3e6f7 --allow-no-subscriptions
                                            adc7bffd-2d17-4df5-af5c-f450dcf3e6f7
````
boscp08@kubernetes-worker2:~$ az --username p.bosch@bdmcc.net
Password: Q..V...._2...
[
  {
    "cloudName": "AzureCloud",
    "id": "69aaa45e-5377-432d-9882-57d002892515",
    "isDefault": true,
    "name": "N/A(tenant level account)",
    "state": "Enabled",
    "tenantId": "69aaa45e-5377-432d-9882-57d002892515",
    "user": {
      "name": "p.bosch@bdmcc.net",
      "type": "user"
    }
  }
]

````
## az --username p.bosch@bdmcc.net -t adc7bffd-2d17-4df5-af5c-f450dcf3e6f7 --allow-no-subscriptions\

````
Get Token request returned http error: 400 and server response: {"error":"interaction_required","error_description":"AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access '797f4846-ba00-4fd7-ba43-dac1f8f63013'.\r\nTrace ID: 5c3bd525-61b3-44d4-a70a-fb93e9ddc500\r\nCorrelation ID: d66bc564-8e3b-45d1-8909-988927d3ec8e\r\nTimestamp: 2020-11-05 19:52:45Z","error_codes":[50076],"timestamp":"2020-11-05 19:52:45Z","trace_id":"5c3bd525-61b3-44d4-a70a-fb93e9ddc500","correlation_id":"d66bc564-8e3b-45d1-8909-988927d3ec8e","error_uri":"https://login.microsoftonline.com/error?code=50076","suberror":"basic_action"}
````
## az login --username bosch.peter@outlook.com -t 69aaa45e-5377-432d-9882-57d002892515 --allow-no-subscriptions

````
C:\Users\bosch>az ad user create --display-name mike --password Mypaermy2aa3434$$ --user-principal-name "mike@ugchelen.onmicrosoft.com"
The domain portion of the userPrincipalName property is invalid. You must use one of the verified domain names in your organization.

C:\Users\bosch>

C:\Users\bosch>az login --username bosch.peter@outlook.com -t 69aaa45e-5377-432d-9882-57d002892515 --allow-no-subscriptions
Password:
[
  {
    "cloudName": "AzureCloud",
    "id": "69aaa45e-5377-432d-9882-57d002892515",
    "isDefault": true,
    "name": "N/A(tenant level account)",
    "state": "Enabled",
    "tenantId": "69aaa45e-5377-432d-9882-57d002892515",
    "user": {
      "name": "bosch.peter@outlook.com",
      "type": "user"
    }
  }
]
````
## az ad user create --display-name mike --password Mypaermy2aa3434$$ --user-principal-name "mike@ugchelen.onmicrosoft.com"

