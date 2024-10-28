## Helpdesk Agent Attended Automation
**Objective** <br>
The process will automate the creation of help desk tickets using data from an Excel sheet.<br>
Once the bot is invoked, it will check whether there are new request files available to process. If available, the bot will read the ticket data from the spreadsheet. The data is used to create support tickets in the Zoho Desk application.

## High level workflow - Helpdesk Agent Process Diagram
![alt_text](https://github.com/bacdillon/RPA-UiPath/blob/main/Helpdesk%20Agent%20Attended%20Automation/img/Helpdesk%20Agent%20High%20level%20workflow%20process%20diagram.jpg)

## Project need enhancements
1. Rename the Request file as Request + DateTimeStamp before move it to the Request folders
2. Capture all the fields (not just mandatory 3 fields) to create the ticket in Zoho
3. Enhance attended automation to include the option to Stop Automation by using a hotkey
4. Implement using UiPath Assistant to trigger check any new ticket(s)
5. Work out with Re-framework to improved error handling, better transaction management and enhanced logging capabilities. This is to standardized approach automation, make it easier to scale and maintain RPA solutions

## Watch Alfred in Action 👇	
![IMAGE ALT TEXT HERE](https://github.com/bacdillon/RPA-UiPath/blob/main/Helpdesk%20Agent%20Attended%20Automation/img/Helpdesk-Agent-Attended-Automation.gif)

<!--
[![IMAGE ALT TEXT HERE](https://github.com/bacdillon/RPA-UiPath/blob/main/CRM%20Alfred%20Bot/img/Alfred%20Action.jpg)](https://youtu.be/alLasPiRb-k)
-->
