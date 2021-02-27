# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Kyle Luce  
**GitHub Handle:** https://github.com/kylebluce  
**Repository:** https://github.com/kylebluce/cis411_lab2_arch  
**Collaborators:** 
___

# Step 1: Confirm Lab Setup
- [x] I have forked the repository and created my lab report
- [x] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [x] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal

Serve Central is fully functional web and mobile application designed to make volunteering easier. The application provides users with geographic locations of volunteer events near them, allows the user to sign up to volunteer straight on the app, and collects statistics of their volunteer efforts.

## Step 2.1 Representative Use Cases  

| Use Case #1 | |
|---|---|
| Title | Signing up for a Volunteer Opportunity |
| Description | This use case describes how volunteers can sign up for volunteer opportunities in the Serve Central application. |    
| Steps | 1. User logs into the Serve Central application. |
| | 2. User navigates to the list of volunteer opportunities nearby. |
| | 3. User chooses a volunteer opportunity to sign up for. | 
| | 4. User fills in their information and availability on a built-in sign up sheet. | 
| | 5. User confirms their information, completing the sign-up form and is officially registered to volunteer. |   
| Primary Actor | Volunteer (User) |    
| Preconditions | 1. User has an account set up with Serve Central |
| | 2. User qualifies for volunteer opportunity they are interested in. |    
| Postconditions | 1. Serve Central documents the registration information and send it to the Service Agency. |
| | 2. Service Agency receives registration information. |
| | 3. User shows up on the day of the volunteer event and does their volunteer work. |
| | 4. Service Agency confirms user showed up to the event. |
| | 5. Serve Central updates the users service statistics. |  

| Use Case #2 | |
|---|---|
| Title | Posting a Volunteer Opportunity |
| Description | This use case describes how a Service Agency can post a volunteer opportunity. |
| Steps | 1. Service Agency worker logs into the Serve Central application as a Service Agency. |   
| | 2. Worker navigates to a tab where they can start the posting process. |    
| | 3. Worker fills in information about the event. This information includes a description, location, and time of the event as well as the number of volunteers needed and the skills required by volunteers. |    
| | 4. Worker confirms the information which sends the new event form to Serve Central to review and eventually post. |   
| Primary Actor | Service Agency Worker |
| Preconditions | 1. Service Agency has a preexisting account with Serve Central. |
| | 2. Service Agency has detailed information about the Service Opportunity to fill out the form. |
| Postconditions | 1. Serve Central reviews and approves the Service Opportunity Posting. |
| | 2. The Service Opportunity gets posted on the Serve Central Application along with a sign-up sheet. |
| | 3. Serve Central notifies users that there is a new opportunity available to them if the user's location is close to the event. |

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
| New Event Form | Volunteer Opportunities List | Serve Central's New Event Option |
| Registration Form | Registered List | Serve Central's Register Option |
| Volunteer Results | User's Volunteer History | Serve Central's Results Option |
| Rating Form | Service Agency's Rating | Serve Central's Feedback Option |

1. Service Agency uses Serve Central's new event option to manipulate the new event form which updates the volunteer opportunities list.
2. User uses serve central's register option to access the registration form which updates the registered list for a particular event.
3. Service Agency uses Serve Central's results option where the service agency can confirm that the volunteer participated which updates the user's volunteer history.
4. Users uses Serve Central's feedback option which allows them to change the rating form which updates the rating for a Service Agency/Event.

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
