# p3-reporthelper
# P3 Project Specs
***
# QC Automation Suite/ QC Report Helper
The QC Report Helper Robot is here to help make the process of finishing and filling out information regarding QC and the different batches much easier 

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
