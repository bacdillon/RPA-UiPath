## Alfred – Intelligent Invoice Processing Automation
![IMAGE ALT TEXT HERE](https://vimeo.com/1078179667/76c54ce610?share=copy) <br>

**Process Flow Description**<br>
1. REFramework Initiation -
Initializes configuration settings, opens required apps, and closes unnecessary ones. On error, exception handling ends the process.

2. Email Processing -
Monitors inbox for subject "Invoice Entry Request for Processing - [Today’s Date]". Downloads attachments to Files\Invoice. Skips if no email or on failure.

3. Intelligent Document Processing -
Loads invoice files, digitizes using OCR, classifies using Keyword Classifier, extracts data via ML Extractor. Sends to Validation Station if needed. Exports to Datasets_Extraction and readable format in Export folder.

4. Consolidate Export Invoice -
Reads exported files, creates headers, appends data into SummaryReport.xlsx in Summary folder. Deletes temporary formatted sheets.

5. REFramework Get Transaction Data -
Uses DataRow (not QueueItem) for transaction items. Retrieves rows from DataTable after app initialization.

6. REFramework Process Transaction -
Validates data. If Invoice No. or Bill To is missing, triggers Business Rule Exception and sends email. Enters data in CRM. Ends if no data remains.

7. REFramework Set Transaction Status -
Sets each transaction’s status (Success, Business, or System Exception). Logs status in Summary Report before moving to next item.

8. REFramework End Process -
Closes applications, moves SummaryReport.xlsx to archive with today's date, formats report, archives all files, and emails final report to relevant stakeholders.

![alt_text](https://github.com/bacdillon/RPA-UiPath/blob/main/Alfred%20%E2%80%93%20Intelligent%20Invoice%20Processing%20Automation/img/summary.jpg)




