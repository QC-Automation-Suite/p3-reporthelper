# p3-ReportHelper
***
# QC Automation Suite/ QC Report Helper
The QC Report Helper Robot is here to help make the process of finishing and filling out information regarding QC and the different batches easier.  Not only will this robot make it easier to fill out information, it will also make it faster and much more organized when filling out said informaiton.

***

## MVP Functionalities
- [ ] Should be able to extract data from Caliber and populate that data into the MS Form Report
- [ ] Should be able to extract data from the SurveyMonkey PowerBI Dashboard and populate that data into the MS Form Report
- [ ] Should be able to identify concerning associates based on QC grade trends:
    -- Rules: 1 = red, 2 = yellow, 3 = green, 4 = blue
    -- Flags: Any reds, 2+ reds in a row, no greens, any certain grade that is below a benchmark for QC
    -- Limitation: Each blue cancels out a red
- [ ] Should be able to do automated emails upon completion of tasks with attached PDF copies of any report documents to the user
- [ ] Should be able to allow user to enter notes of their own into the form after populating fields

## Stretch Goals
- [ ] Should be able to create a summary of survey feedback from the SurveyMonkey PowerBI Dashboard into the form
- [ ] Should be able to extract notes from an excel sheet and put it into Caliber.

## Tech Stack
- UiPath Studio
- UiPath Orchestrator
- UiPath Activities
- UiPath Robot
- Web API
- Excel Automation
- Attended Automation
- Git

------------
------------

<ins>DOCUMENTATION</ins> 

## General Information

- QC Report Helper is an automation designed to store and implement data. Stored data will be extracted from data given by Caliber and Survey Monkey. This data will automatically fill the required fields of a survey in MS Forms; excluding three required manual inputs. At its’ end, the automation will create a pdf file and send it in an email.

## Automation Inputs

- in_auditor (website input that selects desired information from automation)
- in_email (website input that that selects desired email to send PDF from automation)


## Automation Outputs

- Report.Helper.Dispacter – Dictionary to Orchestrator Queue
- Report.Helper.Performer – Queue to MS Forms

## Startup documentation

Steps For Orchestrator

Queue 
-Create a queue name justAqueue

Queue Trigger
-For queue item select justAqueue 
-For process name select the process Report.Helper.Performer.

Steps For Web App

Open website at https://cloud.uipath.com/revaturemdamle/apps_/default/run/production/ID2faaf178bcab4bc5a9b4619c5b6b2d6b?origin=appsHomePage.

Sign in with Microsoft Account

Input auditor name and email

## License Prerequisites 

- UiPath Unattended & Attended Robots
- Orchestrator Community Edition

## Software Prerequisites

- Windows 10
- UiPath 2021.10.3

## UiPath Studio Project Dependencies (minimum package version requirements)

- Default

