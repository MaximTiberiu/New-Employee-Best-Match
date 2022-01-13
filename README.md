
# New Employee Best Match

> Windows Application Project for the RPA Course

## Table of Contents
* [General Info](#general-info)
* [Project Requirements](#project-requirements)
* [Technologies](#technologies)
* [Setup](#setup)
* [Status](#status)
* [License](#license)

## General Info
There is a request from an HR company to create a process that would help with picking the best match applicants for specific jobs.
- There is a guideline file to match the skills and experience needed for each type of job.
		- The subject of the e-mail will start with the **NEW_JOB** keyword.
- CVs are sent by e-mail in predefined formats.
		- The subject of the e-mail will start with the **NEW_CV** keyword.
	- This type of files (CVs and guideline files) can also be sent via a form. **(TBD)**
	- The company will provide a template for each file type.
- Each received CV will be placed in a folder dedicated to that job.
- Relevant information (such as skills and experience) must be extracted from the received and saved documents.
- A custom formula will be applied to calculate a score for each CV. This score will determine how suitable the candidate is for the desired position.
- At the end of the process, a list with the top **n** (n - custom number) candidates will be drawn up and sent by email to the company looking for employees.
- Candidates will also receive an email informing them of the result of selection made in this process.
- The guideline file has a deadline. Candidates who violate this deadline will not be accepted. Every day, until the deadline, the hiring company will receive a daily update, with the list of candidates and their scores. **(TBD)**

## Project Requirements

- [x] Multiple workflows (Flowcharts & Sequences) -> *0.5 - 2 pts*;
- [x] Multiple variable types (String, Int, List, Array, DataTable, etc.) -> *0.5 - 1 pt*;
- [x] Logic flow control (For Each / While / Do While / their equivalent in flowchart logic -> *0.5 - 2 pts* ;
- [x] Excel / PDF automation (read/write data, data processing) -> *0.5 - 2 pts*;
- [ ] Web/Windows Application automation (Selectors, Wildcards, data entry/extraction) -> *0.5 - 2 pts*;
- [x] Handling basic exceptions (Element Exists / retry, etc.) -> *0.5 - 1 pt*.

### Extra Requirements
- [ ] Dynamic Selectors -> **+0.5 pt**;
- [x] Data Scraping -> **+0.5 pt**;
- [x] Advanced exception handling -> **+1 pt**;
- [x] Email automation -> **+0.5 pt**;
- [x] Config file (Excel/JSON) -> **+0.5 pt**;
- [ ] UiPath Orchestrator -> **+0.5 pt**;
- [ ] Automation framework -> **+1 pt**;
- [x] Other UiPath Features (Database, API Calls, OCR, etc.) -> **+0.5 - 1 pt**.

## Technologies
- UiPath Studio 2021.10.3
	- Language: VB
	- Dependencies (Windows - Legacy)
		- UiPath.DocumentUnderstanding.ML.Activities = 1.9.1
		- UiPath.Excel.Activities = 2.11.4
		- UiPath.IntelligentOCR.Activities = 5.1.0-preview
		- UiPath.Mail.Activities = 1.12.2
		- UiPath.OmniPage.Activites = 1.8.0
		- UiPath.System.Activities = 21.10.2
		- UiPath.UIAutomation.Activities = 21.10.3
  
## Setup
- To run the application, you must have UiPath Studio and Outlook installed. 
- Also, the above dependencies must be met. To install packages, use the dedicated tab from the main application: *Manage Packages*. 
- Most packages are installed. 
- You will need to install the following packages: *UiPath.DocumentUnderstanding.ML.Activities*, *UiPath.IntelligentOCR.Activities* & *UiPath.OmniPage.Activites*.
- Now, all you have to do is run the **Main.xaml** file. 
- Select the desired config file. If you do not have one, my recommendation is to use the default one from project folder (**./Data/Config.xlsx**). Change the email address used in Outlook in the config file.

## Status
Project is: *finished*. 

## License
>You can check out the full license [here](https://github.com/MaximTiberiu/New-Employee-Best-Match/blob/main/LICENSE).

This project is licensed under the terms of the **MIT** license.
