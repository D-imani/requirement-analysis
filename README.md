# Requirement Analysis in Software Development

The purpose of this document is to gather, analyze and sefine the requirements of the AirBnB clone being developed, stating how it should work and perform.

## What is Requirement Analysis?
Requirement Analysis is a critical phase in the software development lifecycle (SDLC) where the project team gathers, analyzes, and defines the requirements of the software product to be developed.This process ensures that all stakeholders have a clear and mutual understanding of what the system should do and how it should perform.

## Why is Requirement Analysis Important?:
- Clarity and Understanding: It helps in understanding what the stakeholders expect from the software, reducing ambiguity.
- Quality Assurance: Ensures that the final product meets the specified requirements, leading to higher customer satisfaction.
- Basis for Design and Development: Provides a solid foundation for designing and developing the system.
- Cost and Time Estimation: Facilitates accurate estimation of project cost, resources, and time.
- Scope Definition: Clearly defines the scope of the project, which helps in preventing scope creep.

## Key Activities in Requirement Analysis.
* Requirement Gathering. This involves collecting information needed for the development of the system.
  + Interviews: Conducting interviews with stakeholders to gather detailed information about their needs and expectations.
  + Observation: Observing end-users in their working environment to understand their needs.
  + Surveys/Questionnaires: Distributing surveys to collect requirements from a larger audience.
  + Document Analysis: Reviewing existing documentation and systems to understand current functionalities and requirements.
  + Workshops: Organizing workshops with stakeholders to discuss and gather requirements.
* Requirement Elicitation. This is where the ream comes up with ideas for the features for the system.
  + Prototyping: Creating prototypes to help stakeholders visualize the system and refine their requirements.
  + Brainstorming: Conducting brainstorming sessions to generate ideas and gather requirements.
  + Focus Groups: Holding focus group discussions with selected stakeholders to gather detailed requirements.
* Requirement Documentation. It invloves creating a detailed document that lists all functional and non-functional requirements in a Requirement Specification document.
  + User Stories: Writing user stories to describe functionalities from the user’s perspective.
  + Use Cases: Creating use case diagrams to show interactions between users and the system.
* Requirement Analysis and Modeling.
  + Requirement Prioritization: Prioritizing requirements based on their importance and impact on the project.
  + Modeling: Creating models (e.g., data flow diagrams, entity-relationship diagrams) to visualize and analyze requirements.
  + Feasibility Analysis: Assessing the feasibility of requirements in terms of technical, financial, and time constraints.
* Requirement Validation.
  + Review and Approval: Reviewing the documented requirements with stakeholders to ensure accuracy and completeness.
  + Traceability: Establishing traceability matrices to ensure all requirements are addressed during development and testing.
  + Acceptance Criteria: Defining clear acceptance criteria for each requirement to ensure they meet the expected standards.
 
## Types of Requirements.
### Functional Requirements.
**Definition:** They describe what the system should do.
The examples of functional requirements for the booking management project : 
+ Search Properties: Users should be able to search for properties based on various criteria such as location, price, and availability.
+ User Authentication: Secure login and registration process for users.
+ Property Listings: Display properties with essential details and images.
+ User Registration: New users should be able to create an account with personal details and login credentials.
+ Booking System: Users should be able to book properties, view booking details, and manage their bookings.

### Non-functional Requirements
**Definition** They describe how the system should perform.
The examples of non-functional requirements for the booking management project :
+ Reliability: The system should have an uptime of 99.9% and recover quickly from any failures.
+ Scalability: The system should be able to scale horizontally to handle increased traffic.
+ Performance: The system should load pages within 2 seconds and handle up to 1000 concurrent users.
+ Security: Ensure data encryption, secure login, and protect against common vulnerabilities.
+ Usability: The application should have an intuitive UI/UX, making it easy for users to navigate and perform tasks.

## Use Case Diagrams.
**Definition** They show how different users (actors) interact with the system to achieve specific goals (use cases).
**Benefits**
- Help in identifying and organizing system requirements.
- Provide a clear visual representation of system functionalities.
- Facilitate communication among stakeholders and development team.
  ![Use Case Diagram](./alx-booking-uc.png)

## Acceptance Criteria
**Definition** Acceptance criteria are conditions that a feature must meet to be accepted by the stakeholders.
### Importance of Acceptance Criteria
- Help in maintaining quality and meeting user expectations.
- Provide a basis for testing and validation.
- Ensure all parties have a clear understanding of feature requirements.
### Example
1. Access to Checkout Page. Given the user has selected a property and specified check-in/check-out date. When the user clicks “Reserve” or “Book Now” Then they should be redirected to the checkout page
2. Display of Booking Details. Given the user is on the checkout page
Then they should see: Property name and thumbnail, Check-in and check-out dates, Number of guests. Nightly rate, cleaning fee, service fee, and total costCancellation policy summa
3. Guest Information. Given the user has not filled in required guest information Then the form should prompt for full name, contact number, and any required ID verification (if applicable)
4. Payment Options. Given the user is on the checkout page. Then they should be able to choose a payment method (e.g., credit card, PayPal, mobile money if localized)And input fields should validate card number, expiration date, and CVV
5. Successful Payment and Booking Confirmation. Given the user enters valid payment information. When the user clicks “Confirm and Pay” Then: The payment should be processed securely. A success message and booking confirmation number should be shown
