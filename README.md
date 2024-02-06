# Azure-Boards-Automate-state-transitions-Project
I've created logic apps that will Automate Azure Boards state transitions of parent work items based on child work items.
here is flow of the Logic app.
![flow of the Logic app is like this:](https://github.com/usman-ahmad-22/Azure-Boards-Automate-state-transitions-Project/blob/main/84541089-46361500-acbc-11ea-927a-7d76d730526e.png).

it is efficient and cost-effective way for states automation.
my project team requirments are that "parent work items should not be close if there are any Active child work items". 
1st Step: you need to add a trigger step and connect your DevOps org account with this app from azure devops connector its API name is visualstudioteamservices  then select sub step when work items is closed then select your project and parent work item type.
2nd Step: get child work items details and select your child work item type then i use for each loop, if condition and OR operator in designer to check if any child work item is active
3rs Step: if any child work item is active condtion becomes True then create next step in true block update work item details then click other parameters then select other fields then insert these values system.state = True
