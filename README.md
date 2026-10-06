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
[Click here to view the JSON Code](https://github.com/Ebenezer080925/Automated-Payroll-Deduction-Notice-System/blob/main/Email%20and%20pdf%20download%20Automation%20sender.json)
 The process is go to the Mail sheet pick the specific Customer download the statement which has been already loaded in my drive then filter put the SSS then download as pdf then chnage the names of the pdfs both to the name of the customer draft the mail and then send the mail to there email which picked ealier in the mail sheet 

 # Excel-vba-version 
 ![]()

