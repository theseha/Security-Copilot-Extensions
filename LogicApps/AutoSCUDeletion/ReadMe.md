# **Delete Security Copilot Capacity only when the capacitiy exists**

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https://raw.githubusercontent.com/theseha/Copilot-for-Security-Plugin/main/LogicApps/AutoSCUDeletion/azuredeploy.json)

If you are working on daily SCU creation and deletion with Logic Apps, you might want to deal with the exceptional cases such as no deployed SCU before automatic deletion or already deployed SCU before automatic creation. This Logic App flow is to deal with checking whether SCU is provisioned or not before deleting it. You can use my ARM template to deploy the Logic App flow. However, you need to do an additional work to get your Bearer access token required during the Logic App deployment. You can go to Azure CLI, and type a command below:

```sh
az login
az account get-access-token --resource https://management.azure.com/

You can enter the token when it is requested on Azure Portal.

Hope it helps.
