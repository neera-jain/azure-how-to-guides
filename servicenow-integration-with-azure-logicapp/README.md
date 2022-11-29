
# Content
1. Service Now setup
2. Azure Logic App Creation

## ServiceNow Setup

## Azure Logic App Creation
1. Sign in to the Azure portal (portal.azure.com) with your Azure account.
2. In the search box, enter logic apps and select Logic apps.
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/find-select-logic-apps.png)
3. On the Logic apps page, select Add
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/add-new-logic-app.png)
4. Fill out the details and create the logic app with consumption plan type. 
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/create-logic-app-settings.png)
5. After the delpoyment of logic app is complete, navigate to the "Logic App Designer" section under the Development tools.
6. Add a new step for "When a Http Request is received"
7. Add the next step as ServiceNow actions - Create Record. 
8. In the connection pop up, fill the connection details and click create. This automatically validates the connection and uses this setting. 
9. Once the connection is created, this connector will use the ServiceNow API with a POST request in the background. Select the record type as Incident and fill out the required fields. 
10. For dynamic content when LogicApp is triggered, in the HTTP request received section, add the desired JSON schema. This schema can later be used in the create ticket section to populate dynamic data.





# References
https://learn.microsoft.com/en-us/azure/logic-apps/quickstart-create-first-logic-app-workflow

https://learn.microsoft.com/en-us/connectors/service-now/


https://blog.opstree.com/2021/06/08/servicenow-integration-with-azure-alerts-step-by-step-setup/