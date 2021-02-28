# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Robbie Dorsey  
**GitHub Handle:** airgo32  
**Repository:** https://github.com/airgo32/cis411_lab2_arch  
**Collaborators:** Micah Johnson (@mcjo163), Josiah McCracken (@scribhneoir)
___

# Step 1: Confirm Lab Setup
- [X] I have forked the repository and created my lab report
- [X] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [X] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
Serve Central is a solution to make volunteer events easier for people to find. Users can find and register for lots of local volunteer events all on one app.

## Step 2.1 Representative Use Cases  

| Use Case #1 | |
|---|---|
| Title | Create an event |
| Description / Steps | 1. The agency starts the process of creating an event<br>2. The agency adds a title, description, location, date and time, and event category<br>3. The agency adds any extra fields that they want attendees to fill out<br>4. The event is created and the information is stored in the Serve Central database|
| Primary Actor | Service Agency |
| Preconditions | 1. The agency is registered with Serve Central<br>2. The agency already has an idea and planned time and place |
| Postconditions | 1. The agency has an event scheduled with a time and place<br>2. Users can locate and register for the new event<br>3. The agency is notified about new attendees for their event |

| Use Case #2 | |
|---|---|
| Title | Register for an event |
| Description / Steps | 1. The user selects an event which they want to attend<br>2. The user fills out any information requested by the agency<br>3. The event is added to the user's list of upcoming events |
| Primary Actor | Volunteer |
| Preconditions | 1. The user must be registered on Serve Central<br>2. There must be at least one event scheduled by an organization |
| Postconditions | 1. The user is now registered for a specific event<br>2. The user is notified about time conflicts if this event overlaps with another |

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
| Users | Create an account / Register an organization | Add new user to database |
| Organizations | Create a new event | Request data for event view |
| Planned Events | Browse nearby events | Update event attendance |
| Past Events | View user profile | Add new organization to database |
|  |  | Add new event to database |

## Step 2.3 Diagram a Use Case in Architectural Terms
This UML Sequence diagram describes the process for a user to view an event.    
![UML Sequence Diagram](..\assets\View_Event_UML_Sequence_Diagram.jpg "UML Sequence Diagram for viewing an event")  

# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal
For incorporating these new requirements, I think it would be feasible to stick with the MVC architecture. This could be handled by creating an API for accessing Serve Central data. This would meet the first new requirement by allowing third parties to access the data by using the API. The second solution could also be handled by the API, allowing the organizations to create their own forms and use the Serve Central API to access the database.

## Step 3.2 Revised Architecture Diagram
INSERT IMAGE HERE with a Description.

# Step 4: Scaling an Architecture
INSERT Architectural change proposal here, and how it meets the four new requirements.  Explain both the benefits and draw backs of your proposal.  If the changes are significant, then you need to explain why the changes are necessary versus a nice-to-have enhancement.

# Extra Credit
If you opt to do extra credit, then include it here.