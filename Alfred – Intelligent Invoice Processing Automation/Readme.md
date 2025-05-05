## Alfred – Intelligent Invoice Processing Automation
## Watch Alfred in Action 👇	
![IMAGE ALT TEXT HERE](https://github.com/bacdillon/RPA-UiPath/blob/main/Alfred%20%E2%80%93%20Intelligent%20Invoice%20Processing%20Automation/DU.gif)
**1.RE-Framework- Initiations** <br>
The initial state begin to read the settings, the configuration data stored in the dictionary, initialize applications, and close all the unnecessary applications.  
If there is an error while initializing, an exception handling mechanism is activated, where implemented throughout the framework and end the process.

**2.Email Processing**<br>
The bot monitoring for any incoming emails with the subject: "Invoice Entry Request for Processing - [Today’s Date]". If the condition has met, download the invoices attachments and saves to the Files\Invoice folder.
If there is no incoming email with the latest invoice attachment or system failure, the process 

**3.Intelligent Document Processing**<br>
The process loads the define files and data for extraction and look up the for each downloaded invoice in the folder. 
Digitize the invoice document (UiPath Document OCR) to detect text and its location. 
After Digitization, the invoice document to be Classify (Intelligent Keyword Classifier). Once the invoice document has been classified, the bot is able to recognize the relevant fields.
Proceed to Data Extraction (Machine learning Extractor) where data in a structured manner. If any missing fields, human can confirm the extraction validation from Extraction Validation Station.
The process exports the extracted results and output in Datasets_Extraction. Then export and save each in a readable format in the Export folder for further processes. 

**4.Consolidate Export Invoice**<br>
The process starts collecting, reading each extracted data in a readable format from the Export folder.(i.e., 10280 Mike Inc..xlsx, 10281 Sam Co..xlsx …) .
The process begin create the column headers the such as Invoice Number, Invoice Date… Once was created, appending all the values require and save in the SummaryReport.xlsx located at Summary folder.
Next, delete both sheets (Simple Fields –Formatted and Items –Formatted) output from Export Extraction 

**5.RE-Framework -Get Transaction Data**<br>
The data retrieval state, which is used to get the transaction. 
For this process, the Transaction Item was configured and replaced with the Variable Type as DataRow instead of the default settings QueueItem.
Once the bot successfully initialized all the applications it requires for process. Hence, it looks for any transaction items in the DataTable to process.

**6.RE-Framework -Process Transaction**<br>
The process execute Data Validation, follow by Business Validation. 
If the invoice number and Bill To are empty, not found, Business Rule Exception was trigger, writes the status in Summary Report and sent email notification.
In this state, the transactions are processed that are fetched from the previous state. 
Launch the Order Entry CRM application, perform data entry retrieve from Transaction Item. 
If there is no record  to process, the bot goes to the end process state.

7. RE-Framework -Set Transaction Status
ReFramework has a prebuilt SetTransactionStatus workflow that can be used to set the Transaction Status of an item to either Success, Business Exception or System Exception

While performing data entries, the transaction values and status will be written in the Summary Report. 

After the successful transaction, the bot will now move forward with the next transaction item to be process.

8. RE-Framework –End Process
This is the final state of RE-Framework that the bot has completed processing all the transaction items successfully and closes all the application.

The process move Summary Report to Archive\ SummaryReport folder with today date. Format the Cells , Autofit the Range and archive all the files (Downloaded invoices, extracted data in a readable format) in main Archive folder for future reference.

Once archives completed, attach the compiled and generated with the processing status Summary report who have assigned to the cases with the invoices to be process.






