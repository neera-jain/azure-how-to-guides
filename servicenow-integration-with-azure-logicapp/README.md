
# Content
1. Service Now setup
2. Azure Logic App Creation

## ServiceNow Setup
Setup a demo developer instance of ServiceNow. 
1. Navigate to https://developer.servicenow.com/ 
2. Create a new account by sign-up
3. Click on the Request Instance button on the side header.
![alt text](https://developer.servicenow.com/app_store_learnv2_buildmyfirstapp_rome_servicenowbasics_images_bmfa_requestinstance.png)
4. Select your prefered location and create the instance. 
5. When your instance is available, the Your instance is ready! dialog provides the URL, Username, and Current password for the instance.
![alt text](https://developer.servicenow.com/app_store_learnv2_buildmyfirstapp_rome_servicenowbasics_images_bmfa_getdevinstance.png)
6. Note the credentials and the URL generated, and use it to login.

## Azure Logic App Creation
1. Sign in to the Azure portal (portal.azure.com) with your Azure account.
2. In the search box, enter logic apps and select Logic apps.
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/find-select-logic-apps.png)
3. On the Logic apps page, select Add.
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/add-new-logic-app.png)
4. Fill out the details and create the logic app with consumption plan type. 
![alt text](https://learn.microsoft.com/en-us/azure/logic-apps/media/quickstart-create-first-logic-app-workflow/create-logic-app-settings.png)
5. After the delpoyment of logic app is complete, navigate to the "Logic App Designer" section under the Development tools.
6. Add a new step for "When a Http Request is received"
7. Add the next step as ServiceNow actions - Create Record. 
8. In the connection pop up, fill the connection details(ServiceNow developer instance ) and click create. This automatically validates the connection and uses this setting. 
9. Once the connection is created, this connector will use the ServiceNow API with a POST request in the background. Select the record type as Incident and fill out the required fields. 
10. For dynamic content when LogicApp is triggered, in the HTTP request received section, add the desired JSON schema. This schema can later be used in the create ticket section to populate dynamic data.





# References
https://learn.microsoft.com/en-us/azure/logic-apps/quickstart-create-first-logic-app-workflow

https://learn.microsoft.com/en-us/connectors/service-now/

https://developer.servicenow.com/dev.do#!/learn/learning-plans/rome/new_to_servicenow/app_store_learnv2_buildmyfirstapp_rome_exercise_obtain_a_personal_developer_instance

https://blog.opstree.com/2021/06/08/servicenow-integration-with-azure-alerts-step-by-step-setup/
