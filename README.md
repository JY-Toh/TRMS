# TRMS
PEGA Project
The link below will guide you to my presentation slide for a project I did using PEGA called 'Tuition Reimbursement Management System'.
https://docs.google.com/presentation/d/14-hVMk9dujI_6R1mZd3W8nhlWte_97DJE-zAeWiFsug/edit?usp=sharing

The project requirements are as follows:
Tuition Reimbursement Management System (TRMS)
TRMS Overview
The purpose of TRMS is to provide a system that encourages quality knowledge growth relevant to an individual’s expertise.
Currently, TRMS provides reimbursements for university courses, seminars, certification preparation classes, certifications, and technical training. 
The decision has been made to develop a BPM solution for this system to improve the timeliness and accuracy of approvals. 
The current system relies solely on email communication, requiring manual lookups of available funds and is error-prone due to inbox clutter and incorrect routing of tasks.  
Furthermore, there is no way to record and report on reimbursements awarded, and so the company has no way to identify highly-invested courses that could be developed to be offered in-house.

Business Rules
Each employee is allowed to claim up to $1000 in tuition reimbursement a year.   
Event types have different standard reimbursement coverage: 
University Courses                  80%
Seminars                            60%
Certification Preparation Classes   75%
Certification                       100%
Technical Training                  90%
Other                               30%  
The monetary amount available for an employee to reimburse is defined by the following equation:
AvailableReimburstment = TotalReimburstment ($1000) – PendingReimburstments – AwardedReimburstments.  

Complete the Tuition Reimbursement Form
All Employees must complete the Tuition Reimbursement form one week prior to the start of the event.  
This form must collect (required): basic employee information; date, time, location, description, cost and type of event; work-related justification.  
The projected reimbursement should be provided as a read-only field.

Business Rules
If an employee provides an approval email, that approval step is skipped (cannot skip BenCo Approval).  
If the course is < 2 weeks from beginning, the request is marked urgent.

Direct Supervisor Approval
The direct supervisor must provide approval for Tuition Reimbursement.  
The Direct Supervisor can request additional information from the employee before approval. 

Business Rules
If denied, the Direct Supervisor must provide a reason.  
If the direct supervisor is also a department head, then the department head approval is skipped.  

Department Head Approval
The department head must provide approval for Tuition Reimbursement.  
The Department Head can request additional information from the employee or direct supervisor before approval.

Benefits Coordinator Approval
The BenCo must provide approval for Tuition Reimbursement.   
This stage is not skippable for any reason.  
The BenCo can request additional information from the employee, direct supervisor, or department head before approval. 
The BenCo has the ability to alter the reimbursement amount.

Business Rules
If the BenCo changes the reimbursement amount, the Employee should be notified and given the option to cancel the request. 
If the BenCo does not approval in a timely matter, an escalation email should be sent to the BenCo’s direct supervisor.  


