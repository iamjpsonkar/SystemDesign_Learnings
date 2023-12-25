# **System Design**

## Overview of System Design

### **What is System Design?**
**System design** is the process of defining the architecture, components, modules, interfaces, and data for a system to satisfy specified requirements. It's a crucial phase in software development that focuses on how the system will fulfill the needs and requirements identified during the analysis phase.

System design is a crucial phase in the software development life cycle. It involves defining the architecture, components, modules, interfaces, and data for a system to meet specified requirements. Essentially, it's the process of making decisions about the system's structure and organization to achieve its desired functionality.

### **Key Aspects of System Design**
1. **Architecture**: The overall structure and organization of the system.
2. **Components**: The building blocks or modules that make up the system.
3. **Interfaces**: How different components interact with each other.
4. **Data Design**: Defining how data will be stored, accessed, and managed.

### **Importance of System Design**

- **Efficiency**: Well-designed systems are efficient, ensuring optimal use of resources.
    - A well-designed system optimizes resource utilization, ensuring efficient operation.
    - It minimizes bottlenecks, and unnecessary operations, and maximizes performance.
- **Scalability**: A good design allows the system to grow and handle increased loads.
    - Scalability refers to the system's ability to handle increased loads and growth.
    - A good system design accommodates scalability, allowing the system to expand as needed.
- **Reliability**: System design aims for a high level of reliability, reducing the chances of system failures.
    - Reliability is about minimizing the chances of system failures.
    - A reliable system is robust, resilient, and capable of recovering gracefully from errors.

### **Principles of System Design**

- **Modularity**:
    - **Definition**:  Breaking down the system into manageable and independent modules or components.
    - **Advantages**: Hiding complex details while exposing necessary functionalities to simplify the system's representation.
- **Abstraction**:
    - **Definition**: Hiding complex details while exposing necessary functionalities.
    - **Advantages**: Enhances clarity, reduces complexity, and allows for a higher-level view.
- **Simplicity**: 
    - **Definition**: Striving for simplicity in design without compromising functionality.
    - **Advantages**: Simplicity aids in understanding, and maintenance, and reduces the chances of errors.

### **Different Approaches to System Design**

#### **Top-Down Approach**: 
*Starting with the larger system and breaking it down into smaller components.*

**Overview**:

*The **top-down approach** is a systematic way of designing a system by starting with a high-level view and gradually decomposing it into more detailed components. It's a hierarchical process where the system is broken down into sub-systems or modules, and each module is further refined until the entire system is represented.*

**Steps**:
1. **Start with a General View**: Begin by understanding the system as a whole.
2. **Decomposition**: Break down the system into smaller, more manageable parts.
3. **Refinement**: Continue breaking down each part until detailed components are identified.
4. **Integration**: Combine the detailed components to form the complete system.

**Advantages**:
- **Clarity**: Offers a clear and structured way to understand the system.
- **Progressive Detailing**: Allows for a gradual and detailed development of the system.

**Challenges**:
- **Dependency on Initial Understanding**: The effectiveness depends on the accuracy of the initial high-level view.

#### **Bottom-Up Approach**:
*Building the system from the ground up, starting with individual components.*

**Overview**:

*The **bottom-up approach** is the opposite of the top-down approach. It starts with the smallest, most basic units of the system and gradually combines them into larger structures. It's an incremental approach where the system is built from the ground up.*

**Steps**:
1. **Identify Basic Units**: Start with the smallest, fundamental components of the system.
2. **Build Components**: Develop each component independently.
3. **Integration**: Combine the developed components to create more complex structures.
4. **Achieve System Level**: Continue integrating until the entire system is constructed.

**Advantages**:
- **Early Results**: Allows for early prototypes and functional components.
- **Flexibility**: Easier to adapt to changes during development.

**Challenges**:
- **Integration Complexity**: Integrating various components can be challenging.
- **Possibility of Inconsistencies**: Lack of a holistic view initially might lead to inconsistencies.

### **Case Studies of Well-Designed Systems**

#### **Examples**:
- **Amazon Web Services (AWS)**:
    - **Overview**: AWS is a comprehensive cloud computing platform that provides a wide range of services, including computing power, storage, and databases.
    - **Design Highlights**: AWS is designed with a modular architecture, allowing users to choose and pay for only the services they need. It is highly scalable, and reliable, and provides a vast array of tools for developers.
- **Google's Infrastructure**:
    - **Overview**: Google's infrastructure supports a multitude of services, including search, Gmail, and Google Drive.
    - **Design Highlights**: Google's infrastructure is distributed, with data centers strategically located globally. It employs advanced algorithms for load balancing and fault tolerance, ensuring high availability and responsiveness.

#### **Analysis**:
Common Traits in Well-Designed Systems:
- **Modularity**: Both AWS and Google's infrastructure exhibit modularity by offering a range of services that can be independently utilized.
- **Scalability**: Scalability is a key feature in both systems. AWS allows users to scale resources up or down based on demand, and Google's infrastructure is designed to handle enormous amounts of data and user requests.
- **Reliability**: Reliability is a critical factor. Both systems have redundancy and fault-tolerance mechanisms in place to ensure uninterrupted service.
- **Flexibility**: Flexibility is evident in the customizable nature of services provided by AWS and the adaptability of Google's infrastructure to support various applications.

### Exercise | Requirement Gathering

####  **Scenario**: 
*Imagine you are tasked with designing a system for an online e-commerce platform that facilitates the buying and selling of various products. The platform aims to connect buyers with sellers, providing a seamless shopping experience. Your goal is to analyze and document the system requirements.*

#### **Tasks**

1. **Stakeholder Identification**:
    - **Definition**: Identify and list all stakeholders involved in the e-commerce platform.
    - **Example Stakeholders**: Customers (buyers), Sellers (vendors), Administrators, System Developers, Payment Processors, Customer Support
2. **Gathering and Analyzing Requirements**:
    - **Definition**: Use techniques like interviews, surveys, and research to gather detailed requirements.
    - **Example Techniques**:
        - **Interviews**: Conduct interviews with potential users to understand their needs and preferences.
        - **Surveys**: Distribute surveys to collect quantitative data on user expectations.
        - **Research**: Analyze existing e-commerce platforms and market trends.
3. **Prioritizing Requirements**:
    - **Definition**: Assign priorities to each requirement based on its importance to the success of the e-commerce platform.
    - **Example Criteria for Prioritization**:
        - **Critical Functionality**: Features essential for the core functionality of buying and selling.
        - **User Experience**: Enhancements that significantly improve the user experience.
        - **Market Trends**: Prioritize features aligned with current e-commerce market trends.
4. **Documenting Requirements**:
    - **Definition**: Create clear and concise documentation for each identified requirement.
    - **Example Documentation Template**:
        - **Requirement ID**: R001
        - **Description**: The system should allow registered users to add products to their shopping cartS.
        - **Priority**: High
        - **Stakeholders**: Customers, Sellers
        - **Dependencies/Constraints**: Users must be registered and logged in to add products to the shopping cart.

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

### Exercise | Requirements analysis

#### **Scenario**: 
*You are now tasked with gathering requirements for an online banking system. The system aims to provide a secure and user-friendly platform for customers to manage their accounts, transfer funds, and view transaction history.*

#### **Tasks**:
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

## System Architecture

*Key components of system architecture, considerations for choosing the right architecture, and factors related to scalability and performance.*

