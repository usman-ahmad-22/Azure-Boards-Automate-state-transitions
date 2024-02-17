# Azure-Boards-Automate-state-transitions-Project
**I created logic apps that will Automate Azure Boards state transitions of parent work items based on child work items.**

workflow of automation is like this:

![workflow of automation is like this](https://github.com/usman-ahmad-22/Azure-Boards-Automate-state-transitions-Project/blob/main/84541089-46361500-acbc-11ea-927a-7d76d730526e.png).

it is efficient and cost-effective way for states automation.
### Automation benefits for  team:
* Provide better visibility and tracking of work item progress and dependencies.
* it can enforce workflow rules and policies to meet quality standards and compliance requirements.
* it can ensure consistency and accuracy of work item states across the project.
* it can save time and effort by reducing manual updates.

**my project team requirments are "parent work items should not be close if there are any Active child work items" so i created workflow for this functionality**
### Workflow Steps:
### 1st Step:
you need to add a trigger step and connect your Azure DevOps org account with this app from azure devops connector its API name is visualstudioteamservices  then select sub step "when work items is closed" then select your project and parent work item type.
### 2nd Step:
"get child work item details" and select your child work item type then i use for each loop, if condition and OR operator in designer to check if any child work item state is active
### 3rd Step:
if any child work item state =  active condtion becomes True then create next step in true block "update work item details" then click on other parameters then select other fields then insert these values System.State = True

**you can also automate other elements of azure devops services with Azure logic apps**
### Support Me
If you find this project useful or would like to support my work,  Your contribution will help me continue to improve this project and create new ones in the future.
You can also show your support by giving this repository a star on GitHub. This will help more people discover and use the project, and let me know that you find it useful. To star the repository, simply click the "Star" button at the top of the page.
