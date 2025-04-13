## Alfred Bot - Extract Invoice information & store data in Orchestrator
**Objective** <br>
The process has been selected for RPA as part of the larger project initiative conducted within ACME
Systems Inc., the Finance and Accounting department.

The objective of this process automation is linked to the project business case and is mainly intended to:
Deliver faster processing
Reduce redundant activities
Improve overall performance and reliability.

**Business process to automate** <br>
1) Login to ACME application <br>
2) Navigate Invoice search invoices screen <br>
3) Click display all invoices <br>
4) Extract all invoice information <br>
5) Get only Invoice No, Vendor Tax ID, Invoice Date <br>
6) Store the above 3 values into the orchestrator queue (invoice_details) for further processing <br>

**Description of the Project**<br>
**Steps    Short Description** <br>
1.1 Open the ACME System 1 Web Application <br>
1.2 Log in to System 1. Required input data: email and p assword. <br>
1.3 Access the Dashboard - the central location, where the user can pick a specific menu item.<br>
1.4 Access the Invoice Items listing to view all the invoices (Display All Invoices) <br>
1.5 Get only Invoice No, Vendor Tax ID, Invoice Date <br>
1.6 Store the above 3 values into the orchestrator <br>

**Process Flow Chart**<br>

![alt_text](https://github.com/bacdillon/RPA-UiPath/blob/main/ACME%20Invoice-Processing/documents/ACME%20Invoice%20Processing.jpg)

## Watch Alfred in Action 👇	
![IMAGE ALT TEXT HERE](https://github.com/bacdillon/RPA-UiPath/blob/main/ACME%20Invoice-Processing/documents/UiPath-Processing-Invoice.gif)



