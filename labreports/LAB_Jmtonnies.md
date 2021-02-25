# Lab Report: Continuous Integration
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Joseph Tonnies  
**GitHub Handle:** Jmtonnies  
**Repository:**  https://github.com/Jmtonnies/cis411_lab2_arch
**Collaborators:** Alecclyde, ArturD0nnelly

# Step 1: Confirm Lab Setup
- [ ✓ ] I have forked the repository and created my lab report
- [ ✓ ] I have reviewed the [lecture / discsussion](../assets/04p1_SolutionArchitectures.pdf) on architecture patterns.
- [ ✓ ] If I'm collaborating on this project, I have included their handles on the report and confirm that my report is informed, but not copied from my collaborators.

# Step 2: Analyze the Proposal
Creating a user tracking, volunteer system that allows application submission, and company / event tracking all in one app.

## Step 2.1 Representative Use Cases  

| Request to join a volunteer event | |
|---|---|
| Actor: Volunteer | |
| Preconditions:<br>1. The perspective volunteer is already registered on the app <br>2. A company has posted a listing| |
| Description / Steps:<br>1.0 Request to join a volunteer event<br><dd>1. User specifies a certain event they would like to volunteer for<br><dd>2. The system verifies that the posting is valid (time, date, is it cancelled).<br><dd>3. The system checks to see if the event is full.<br><dd>4. The system asks the user what times they would like to volunteer.<br><dd>5. The user selects the time slots they would like to volunteer for.<br><dd>6. The system asks user to confirm their selection of times<br><dd>7. The system sends a reminder near the time of the Volunteers time slot<br><dd>8. The system tracks the users time of volunteership and job description for later review by user | |
| Postconditions:<br><dd>1. The user actually volunteers at the event<br><dd>2. The system sends a reminder<br><dd>3. the system record time and date the user volunteered | |

| Adding a volunteer event or position | |
|---|---|
| Actor: Service Agencies | |
| Preconditions:<br><dd>1. A company or person is registered and verified with the app<br><dd>2. The company or person has a volunteer event | |
| Description / Steps<br>1.0 Request to add an event or position <br><dd>1. A company or person specifies a day and time they will be having a volunteer position or event<br><dd>2.The USer <br><dd><br><dd><br><dd><br><dd><br><dd><br><dd>  | |
| Postconditions | |

## Step 2.2 Define the MVC Components

| Model | View | Controller |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |

## Step 2.3 Diagram a Use Case in Architectural Terms
INSERT IMAGE HERE with a Description.

# Step 3: Enhancing an Architecture

## Step 3.1 Architecture Change Proposal
INSERT Architectural change proposal here, and how it meets the two new requirements.  Explain both the benefits and draw backs of your proposal.

## Step 3.2 Revised Architecture Diagram
INSERT IMAGE HERE with a Description.

# Step 4: Scaling an Architecture
INSERT Architectural change proposal here, and how it meets the four new requirements.  Explain both the benefits and draw backs of your proposal.  If the changes are significant, then you need to explain why the changes are necessary versus a nice-to-have enhancement.
