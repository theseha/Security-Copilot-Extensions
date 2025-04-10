You might considering sending summarized Defender XDR or Sentinel incidents to Microsoft Teams to manaage and recognize incidents as soon as possible with simplified but important information.

If you create a Logic App without any granular manipulation, the summary which will be sent to Teams may be in status of low visibility. From Security Copilot, you can get only necessary information. After that, parse the information and create a HTML table with those information. Then, it will be well delivered to Teams message with better visibility.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftheseha%2FCopilot-for-Security-Plugin%2Frefs%2Fheads%2Fmain%2FLogicApps%2FIncidentSummaryToTeams%2Fazuredeploy.json)



![Logic App Designer](https://raw.githubusercontent.com/theseha/Copilot-for-Security-Plugin/main/LogicApps/IncidentSummaryToTeams/teamstable.png)

![Logic App Designer](https://raw.githubusercontent.com/theseha/Copilot-for-Security-Plugin/main/LogicApps/IncidentSummaryToTeams/IncidentToTeams.png)
