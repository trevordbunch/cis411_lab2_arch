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

| Use Case #1 |Volunteer|
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
![](../assets/MVC%20Diagram.jpg)
For the volunteer to make an account, they have to send a request to the controller, where the controller should create an object to send to the model. Then the model sends the result to the controller. It gets sent to the view to show the user to confirm their account was created.
# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal

I would continue using the MVC architecture short-term, as changing the architecture would likely cause issues and is fine for our situation. Serve Central would need to create an API for companies to link their profiles to. An API for the third-party to connect to for the input data. The MVC architecture can get incredibly complicated quickly, this can be especially difficult on the views if the model changes frequently.

## Step 3.2 Revised Architecture Diagram
![](../assets/MVC%20Diagram%20(Updated).jpg) This diagram adds the "Third Party" to the model. I kept the model in the diagram to show the data continuing to flow in the same path. I also added a fork off of the controller, where if the user wants to visit a organization's website, it is grabbed directly from the organization.

# Step 4: Scaling an Architecture
The best way to handle the large bursts of users is to use a load balancing technique in order to decrease downtime and to create redundancy. With the need for increased storage space and for increased insurance for quality back-ups, I would suggest buying and putting servers in different locations (preferably our hot-spots). This would keep us from being susceptible to certain environmental threats, and it would again increase redundancy and access speed. We will also need to add in another interface that allows the 'authorized parties' to issue queries into our database. These queries must be monitored, as we do not want the wrong party gaining access, nor do we want to have an accidental deletion of the entire database and backups.  

The additional architecture is needed to meet all requirements of the new grant. If there is a large event that gains popularity, we have to be ready to accommodate a large flock of users.