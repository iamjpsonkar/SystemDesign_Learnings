# **System Design**

## Overview of System Design

**What is System Design?**

**System design** is the process of defining the architecture, components, modules, interfaces, and data for a system to satisfy specified requirements. It's a crucial phase in software development that focuses on how the system will fulfill the needs and requirements identified during the analysis phase.

**Importance of System Design**

- **Efficiency**: Well-designed systems are efficient, ensuring optimal use of resources.
- **Scalability**: A good design allows the system to grow and handle increased loads.
- **Reliability**: System design aims for a high level of reliability, reducing the chances of system failures.

**Principles of System Design**

- **Modularity**: Breaking down the system into manageable and independent modules.
- **Abstraction**: Hiding complex details while exposing necessary functionalities.
- **Simplicity**: Striving for simplicity in design to enhance understandability.

**Different Approaches to System Design**

- **Top-Down Approach**: Starting with the larger system and breaking it down into smaller components.
- **Bottom-Up Approach**: Building the system from the ground up, starting with individual components.

### Exercise

#### Requirement Analysis

**Scenario**: *Imagine you are tasked with designing a system for an online e-commerce platform that facilitates the buying and selling of various products. The platform aims to connect buyers with sellers, providing a seamless shopping experience. Your goal is to analyze and document the system requirements.*

#### **Tasks**

1. **Stakeholder Identification**:
    - Identify and list all stakeholders involved in the e-commerce platform. This may include customers, sellers, administrators, and any other relevant parties.
2. **Gathering and Analyzing Requirements**:
    - Use techniques like interviews, surveys, and research to gather detailed requirements.
    - Analyze each requirement for clarity, feasibility, and relevance to the overall system goals.
3. **Prioritizing Requirements**:
    - Assign priorities to each requirement based on its importance to the success of the e-commerce platform.
    - Consider factors such as customer needs, business goals, and regulatory requirements.
4. **Documenting Requirements**:
    - Create clear and concise documentation for each identified requirement. Include details such as:
        1. Requirement ID
        2. Description
        3. Priority
        4. Stakeholders involved
        5. Any dependencies or constraints

### Solution

---
**Requirement ID**: R00001

**Description**: This system connects buyers and sellers, via a web-based application, where a buyer can buy multiple products using the web app from the seller.

**Priority**: High

**Stakeholders**: Customer (Buyer), Seller

**Dependencies/Constraints**: For this system to work, some products need to be present in the system and a logged-in, user can add the products and buy them from the seller.
1. user must be logged in, before buying
2. the seller must have added some products in the web app, to get the desired result.
---

## Understanding System Requirements

### Requirements analysis
**Requirements analysis** is a critical phase in system design, and a thorough understanding of stakeholder needs is essential for a successful design.

**Topics**:
- Stakeholder Identification and Analysis:
    - Techniques for identifying and analyzing stakeholders.
    - Importance of understanding stakeholder perspectives and needs.


- Requirements Gathering Techniques:
    - Overview of common techniques such as interviews, surveys, and workshops.
    - Selecting the appropriate technique based on the nature of the project.

- Types of Requirements:
    - Distinguishing between functional and non-functional requirements.
    - Examples and importance of each type in system design.

- Use Cases and User Stories:
    - Introduction to use cases and user stories as tools for requirement elicitation.
    - Creating effective use cases and user stories.

### Exercise

**Scenario**: *You are now tasked with gathering requirements for an online banking system. The system aims to provide a secure and user-friendly platform for customers to manage their accounts, transfer funds, and view transaction history.*

**Tasks**:
1. **Stakeholder Identification**:
Identify and analyze stakeholders for the online banking system.
Consider both internal (bank employees) and external (customers) stakeholders.
2. **Requirements Gathering**:
Choose and justify a requirements-gathering technique for the online banking system.
Provide a sample set of questions or methods you would use in an interview or survey.
3. **Types of Requirements**:
List at least three functional and three non-functional requirements for the online banking system.
4. **Use Cases and User Stories**:
Create a use case or user story related to a fund transfer scenario in the online banking system.

### Solution

---
**Requirement ID**: R00002

**Description**: Requirement gathering for an online banking system.

**Stakeholders**: New Customers (Users who will open a new account with the bank), Existing Customers (Users who have already an account with the bank), Bank employees (who will manage and maintain the fund), and the Bank itself, which has the actual funds and user data.

**Dependencies/Constraints**:

1. The bank must have funds to run the bank
2. The bank also needs to have a management team.
3. User group that must have money and interest in the bank.

**Requirements Gathering**:

1. Describe the size of the bank and the user group on which the bank will be focused.
2. Feature:
    - Secure fund management
    - Secure user and their data management
    - User-friendly UI
    - viewing the transaction history
    - fund transfer to another bank account
    - new account creation
3. Security, use encryption and https

**Requirements**

- Functional Requirements
    1. Signup and Sign in
    2. View Transaction History
    3. Fund Transfer
- Non Functional Requirements
    1. Security of Data and Users
    2. User-friendly UI
    3. Fast and Efficient System

**Use Cases and User Stories**
Below is the complete journey
1. User A creates an account in the bank
2. Enters details of himself
3. user A submits some money to the bank.
4. user A checks the account balance
5. user A transfers some funds to the account of existing user B
6. user A and user B, both get notified about the money transfer
7. Both the users check the new account balance, also the updated transaction history.
---