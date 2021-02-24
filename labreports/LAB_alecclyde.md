# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Alec Chappell  
**GitHub Handle:** @alecclyde  
**Repository:** [Alecclyde's Forked Repository](https://github.com/alecclyde/cis411_lab2_arch)  
**Collaborators:** 
___

# Step 1: Confirm Lab Setup
- [x] I have forked the repository and created my lab report
- [x] I have reviewed the [lecture / discussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [x] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
This application helps those who wish to do volunteer more and help others. This aggregates all volunteer events and organizations into one app so volunteers can find events easier.

## Step 2.1 Representative Use Cases  

| Use Case #1 |Volunteers|
|---|---|
| **Title** |Sign up for a Service Event |
| **Description / Steps** | This use case describes how a volunteer would sign up for a service event that is hosted by a Service Agency. |
| **Primary Actor** |The Volunteer |
| **Preconditions** |Volunteer has an account. There is a Service Event for the Volunteer to sign up for.|
| **Postconditions** |The service agency can access the list of people who sign-up for the event. |

| Use Case #2 |Service Agencies|
|---|---|
| **Title** |Add a Service Event |
| **Description / Steps** |This use case describes how a Service Agency would create a service event that volunteers could sign up for. |
| **Primary Actor** |Service Host |
| **Preconditions** |The Service Agency has already registered their organization. |
| **Postconditions** |The service agency's event is updated on the database. The event is listed for volunteers to see. |

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
| Name | Organization Page | EventFeedController |
| Location | Volunteer Page | CreateEventController |
| Event Title | Event Feed | EditProfileController |
| Event Description | Map Event Page | SignUpEventController |

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