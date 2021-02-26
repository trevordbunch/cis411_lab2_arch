# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Your Name  
**GitHub Handle:** Your GitHub Handle  
**Repository:** Your Forked Repository  
**Collaborators:** 
___

# Step 1: Confirm Lab Setup
- [X] I have forked the repository and created my lab report
- [X] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [X] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
Serve Central ... ENTER A BASIC SYSTEM INTRODUCTION HERE (1-2 Sentences).
- ServeCentral is an app that makes it easier to find and sign up for volunteer opertunities. The app stores all event and company information and all user information.
## Step 2.1 Representative Use Cases  

| Use Case #1 |Volunteer|
|---|---|
| Title |Sign up to volunteer|
| Description / Steps |This use case describes how the volunteer would sign up to volunteer|
| Primary Actor |Volunteer|
| Preconditions |The User has created an account and logged in. Events database is available and on-line. There are events to sign up for.|
| Postconditions |The user is added to the list of volunteers.|

| Use Case #2 |Service agencies|
|---|---|
| Title |Add an event|
| Description / Steps |This use case describes how the service agencies would add an event|
| Primary Actor |Service agency|
| Preconditions |Service agency is authorized. Service agency has added their company information. Events database is available and on-line|
| Postconditions |The event is stored on the events database|

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
|Profile|Profile Page|EditProfileController|
|Events|Events Page|AddEventController|
|Map|Map Page|JoinEventController|
|Company Information|Company Page|EditCompanyInformationController|

## Step 2.3 Diagram a Use Case in Architectural Terms
INSERT IMAGE HERE with a Description.

# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal
INSERT Architectural change proposal here, and how it meets the two new requirements.  Explain both the benefits and draw backs of your proposal.

## Step 3.2 Revised Architecture Diagram
INSERT IMAGE HERE with a Description.

# Step 4: Scaling an Architecture
INSERT Architectural change proposal here, and how it meets the four new requirements.  Explain both the benefits and draw backs of your proposal.  If the changes are significant, then you need to explain why the changes are necessary versus a nice-to-have enhancement.

# Extra Credit
If you opt to do extra credit, then include it here.