# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Isaac Parada  
**GitHub Handle:** isaacparada  
**Repository:** isaacparada/cis411_lab2_arch  
**Collaborators:** 
___

# Step 1: Confirm Lab Setup
- [x] I have forked the repository and created my lab report
- [x] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [ ] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
Serve Central ... ENTER A BASIC SYSTEM INTRODUCTION HERE (1-2 Sentences).

Serve Central helps people to find volunteer service opportunities in their commuinity. It displays local events to users and provides an easy application process for those looking to join an event.
## Step 2.1 Representative Use Cases  

Use Case #1

![Use Case 1](labreports/../Use_Case1.png)
Use Case #2
![Use Case 2](labreports/../Use_Case2.png)

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
| Check Login credentials, add new records for new accounts| Login/signup page | Handle login request |
| Update user/agency information, or Access statistics | Home screen | Home screen features & app navigation|
| Add public events & Querry for nearby events | Events list | Event features|
| Access  event/ organization information | Event/organization pages| Handle requests for all event/organizer pages|

## Step 2.3 Diagram a Use Case in Architectural Terms
![MVC Diagram](labreports/../MVC_Diagram.png)

The main MVC component here is the login system where the user (a volunteer or service agency) creates their account. The information they enter is passed from the dynamic web page through the controller to the model where it is added to the database as a new record. I also included (in less detail) the process of listing and signing up for events. 

# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal
INSERT Architectural change proposal here, and how it meets the two new requirements.  Explain both the benefits and draw backs of your proposal.

## Step 3.2 Revised Architecture Diagram
INSERT IMAGE HERE with a Description.

# Step 4: Scaling an Architecture
INSERT Architectural change proposal here, and how it meets the four new requirements.  Explain both the benefits and draw backs of your proposal.  If the changes are significant, then you need to explain why the changes are necessary versus a nice-to-have enhancement.

# Extra Credit
If you opt to do extra credit, then include it here.