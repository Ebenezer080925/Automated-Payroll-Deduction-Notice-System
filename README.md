# Automated-Payroll-Deduction-Notice-System
An end-to-end automation that generates per-customer financial PDFs from live spreadsheet data and emails them monthly — built in two parallel versions (cloud-based and on-premise) to match different client infrastructure.

README.md
/n8n-version/
    workflow.json
    screenshots/
/excel-vba-version/
    SSS_Automation.xlsm (with sample/fake data only)
    modules/ (exported .bas files, readable without opening Excel)
demo-screenshots/

## The problem 
###  1.A business needed to send monthly SSS deduction notices to 400++ customers, each with a personalized PDF breakdown cut from a combined spreadsheet, plus a page extracted from a 2,500+ page combined statement PDF.
###  2.Why two versions — one client runs cloud-based tooling (n8n), another relies on existing on-premise Excel/Outlook — you adapted the same logic to both environments.
###  3.Technical challenges solved — this is the part that actually impresses people reading code:
    -Programmatic PDF generation from spreadsheet data with no native PDF tool (Google Sheets export trick / Excel's ExportAsFixedFormat)
    -Automatically locating and extracting specific page ranges from a massive combined PDF using text-scanning
    -Safe, resumable batch processing (loop sequencing, rate-limit handling)
###  4.Outcome — quantify it: "Reduced a previously 100% manual monthly task to a single click, processing 2,500+ pages and 60+ personalized emails automatically"

Personal Details are closed 
## This is where the specifi details of the customer detail to work with will be picked 
![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Picking%20sheet.png)

## After picking the specific customer detials it then goes to the sheet where the SSS details is filtered out and then save specific persons own as pdf
![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/pdf%20sheet.png)

## Then also move to the Statement pdf to save out the specicfic customer Statement then save as pdf 
![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Statement%20pdf.png)

## The Drafted image after saving the pdfs
![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Drafted%20Image.png)


The Automations does this process repeatedly for all this customers 

# n8n version 
![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/n8n%20Workflow%20.png)
[JSON.Code](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Email%20and%20pdf%20download%20Automation%20sender.json)
 The process is go to the Mail sheet pick the specific Customer download the statement which has been already loaded in my drive then filter put the SSS then download as pdf then chnage the names of the pdfs both to the name of the customer draft the mail and then send the mail to there email which picked ealier in the mail sheet 

 # Excel-vba-version 
 ![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Vba%20Codes%20.png)
 The Vba macro code has abput 5 module with each module have different codes doing different works 
 Fromm the first command to run the full process RunFULLSSSAutomation -> GetPageRange -> GenerateSSSPdf -> SplitStatementPdf -> SendCustomerEmailFull  
 which is now in .display so the person sending can view manually before sending and also be sent automatically by changing it from .Display to.Send 

 ![](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Screenshot%202026-10-06%20225750.png)
 That's it in the display form bfore sending already loaded in draft which can be converted to direct send 

