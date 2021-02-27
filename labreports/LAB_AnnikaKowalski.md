# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Annika Kowaslki 
**GitHub Handle: https://github.com/AnnikaKowalski/cis411_lab2_arch
**Collaborators:** 
___

# Step 1: Confirm Lab Setup
- [ yes ] I have forked the repository and created my lab report
- [ yes ] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [ ] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
Serve Central ... ENTER A BASIC SYSTEM INTRODUCTION HERE (1-2 Sentences).
Serve Cetnral is an app that allows users to locate volunteer/serving opportuniues in the local area. It allows users to register for the event throguh the mobile app. 

## Step 2.1 Representative Use Cases  

| Use Case #1 | Volunteer |
|---|---|
| Title | Signing up for a Service Event |
| Description / Steps | This use case will show how to sign up for a service event that is taking place. |
| Primary Actor | Volunteer |
| Preconditions | The volunteer must have an account wiht Serve Central. There must be an event in the local area that the volunteer can sign up for. |
| Postconditions | The service evetn team leader msut be able to view all the mebers who have signed up for volunteer for the event. |

| Use Case #2 | Companies Offering Service Events |
|---|---|
| Title | Adding a Service Event |
| Description / Steps | This use case will describe how a company will list volunteer spots on the Serve Central app for lacal people to sign up for. |
| Primary Actor | Company Hosting the Event |
| Preconditions | The company already has a Serve Central account under the sevice agent category, this allows them to create events. |
| Postconditions | The company's event is then added to the lisst for the locals to see as an opportunity for service/volunteering. |

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
| Name | Organizations Page  | Event Feed Controller  |
| Location  | Volunteer's Feed Page  | Volunteer Feed Controller |
| Event Title | Event Feed Page | Event Feed Controller |
| Event Description  | Decription Feed Page | Description Feed Controller |

## Step 2.3 Diagram a Use Case in Architectural Terms
INSERT IMAGE HERE with a Description.
The volunteer makes a request to the controller for a Serve Central account. The controller then sends is to the model. The model creates the account for the volunteer ands that to the view. The view allows the volunteer to view service opporunitites and they can sign up for ones that  interst the. 

# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal
INSERT Architectural change proposal here, and how it meets the two new requirements. Explain both the benefits and draw backs of your proposal.
I would add an third party API which would allow users to navigate to the website of the organization they are volunteering for. By adding this feature those who are volunteering can understnad the organization's mission and see if that service project is someting thet are interested in. 

## Step 3.2 Revised Architecture Diagram
INSERT IMAGE HERE with a Description.
The data will flow very similarly to the graph that was shown prior. There are some changes and they iincludes...the model now sends information to the thrid party. This is where the the thrid party gets the website information adn sends it back to the model. The view sends the infromation to the organization's page which is how the serivce organization's page updates for the unsers. The user is then able to view the service organization's information wihtout leaving the app for any reason. 

# Step 4: Scaling an Architecture
INSERT Architectural change proposal here, and how it meets the four new requirements. Explain both the benefits and draw backs of your proposal.  If the changes are significant, then you need to explain why the changes are necessary versus a nice-to-have enhancement.
It is great that the organization is grwoing but with the bursts it can be challenging for the company. The company would be able to handle the large burts if they had an easier way to balance all the traffic on the app. It would also be inportant to  make sure that informtaion is not repetitive on the user end as this can cause some lag time and create a  slower app for the user. 

# Extra Credit
If you opt to do extra credit, then include it here.