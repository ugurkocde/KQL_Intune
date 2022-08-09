## Query Pack for Log Analytics

This is essentially a Template which will deploy all queries from this repository into your Log Analytics Workspace.

**I am going to add all queries as soon as we reach day 50 of the #50DaysofKQLforIntune**

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fugurkocde%2FKQL_Intune%2Fmain%2FQuery%2520Pack%2Fazuredeploy.json)

# Guide

1.  Click on the [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fugurkocde%2FKQL_Intune%2Fmain%2FQuery%2520Pack%2Fazuredeploy.json) button. It will open the Azure portal.

2. Select your Resource group, Region and Resource Name. Click on Review + create.

3. Wait for the deployment to finish (aprox. 5 min). Done :)

4. The queries will be visible in the Logs inside your LA Workspace. You will find them if you search for **Intune** under the queries option:

5. You can also enable or disable the imported query pack here:



# Links

1. ![Query packs in Azure Monitor Logs (preview)](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/query-packs)
2. ![Log Analytics Query packs](https://techcommunity.microsoft.com/t5/azure-observability-blog/log-analytics-query-packs/ba-p/2314721)