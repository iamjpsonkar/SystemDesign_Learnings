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

### Exercise | Requirement Analysis

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
        - **Description**: The system should allow registered users to add products to their shopping carts.
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

### **Stakeholder Identification and Analysis**

#### **Techniques for Stakeholder Identification**:

- **Brainstorming**:
    - **Process**: Gather a diverse group of people to generate a list of potential stakeholders.
    - **Benefits**: Encourages collective input and ensures a broad perspective.
- **Surveys and Questionnaires**:
    - **Process**: Distribute surveys to potential users, employees, and other involved parties.
    - **Benefits**: Collects feedback from a large audience, especially useful in large-scale projects.
- **Interviews**:
    - **Process**: Conduct one-on-one or group interviews with individuals representing different roles.
    - **Benefits**: Provides in-depth insights, and allows for clarification of roles and expectations.

#### **Importance of Understanding Stakeholder Perspectives**:
- **Diverse Needs**: Different stakeholders may have diverse needs and expectations from the system.
- **Conflict Resolution**: Understanding stakeholder perspectives helps in resolving conflicts and finding compromises.
- **Holistic Design**: A comprehensive understanding of stakeholders ensures a system that meets the requirements of all involved parties.

### **Requirements Gathering Techniques**

#### **Overview**:
*Requirements gathering is a critical step in system design, ensuring a thorough understanding of what the system needs to accomplish. Various techniques can be employed to gather requirements effectively.*

#### **Common Techniques**:

1. **Interviews**:
    - **Process**: Conduct one-on-one or group interviews with stakeholders to gather information.
    - **Benefits**: Provides detailed insights, allows for clarification, and builds a rapport with stakeholders.
2. **Surveys and Questionnaires**:
    - **Process**: Distribute structured surveys to a broad audience and collect responses.
    - **Benefits**: Gathers quantitative data, useful for large-scale user feedback.
3. **Observation**:
    - **Process**: Observe users in their natural environment to understand how they currently perform tasks.
    - **Benefits**: Offers insights into actual user behavior and identifies pain points.
4. **Workshops**:
    - **Process**: Bring together stakeholders for interactive sessions to discuss and define requirements.
    - **Benefits**: Encourages collaboration, captures diverse perspectives, and resolves potential misunderstandings.
5. **Prototyping**:
    - **Process**: Create a simplified model or prototype of the system to gather feedback.
    - **Benefits**: Allows stakeholders to interact with a tangible representation, uncovering additional requirements.

#### **Choosing the Right Technique**:
- **Nature of the Project**: The complexity and scale of the project influence the choice of technique.
- **Time Constraints**: Some techniques, like surveys, may be quicker to implement than workshops.
- **Accessibility of Stakeholders**: Availability and accessibility of stakeholders may determine the feasibility of certain techniques. 

### **Types of Requirements**

#### **Distinguishing between Functional and Non-functional Requirements**:
- **Functional Requirements**:
    - **Definition**: Describes what the system should do and the specific functionalities it should provide.
    - **Examples**:
        - Users should be able to create an account.
        - The system should allow users to add products to their shopping cart.
        - An admin should be able to manage user accounts.
- Non-functional Requirements:
    - **Definition**: Describes qualities or characteristics that the system should have, such as performance, security, and usability.
    - **Examples**:
        - The system should respond to user actions within 2 seconds.
        - Data should be encrypted during transmission.
        - The user interface should be intuitive and user-friendly.

#### **Importance of Both Types**:
- **Functional Requirements**:
    - Define the core features and capabilities of the system.
    - Directly contribute to the system's primary objectives.
- **Non-functional Requirements**:
    - Ensure the system's overall performance, security, and user experience.
    - Provide criteria for evaluating the success of the system.

### **Use Cases and User Stories**
**Introduction**:
*Use Cases and User Stories are powerful tools for capturing and expressing system requirements in a user-centric manner. They help in understanding how users interact with the system and the specific scenarios in which the system will be used.*

#### **Use Cases**:
- **Definition**: A use case is a description of how a user interacts with a system to accomplish a specific goal.
- **Components**:
    - **Actor**: A user or system that interacts with the system.
    - **System**: The main subject under discussion.
    - **Use Case**: Describes a specific interaction or flow of events.

**Example**:
- **Use Case**: The user makes a purchase.
- **Actor**: Customer
- **System**: E-commerce platform
- **Flow**:
    1. The customer adds items to the shopping cart.
    2. The customer proceeds to checkout.
    3. The customer provides shipping information.
    4. The customer completes the purchase.
#### **User Stories**:
**Definition**:
*A user story is a brief, simple description of a feature told from the perspective of the person who desires the functionality.*

- **Components**:
    - **Role**: The user or system role involved.
    - **Action**: What the user wants to do.
    - **Benefit**: The value or benefit the user gains.

**Example**:
- **User Story**: As a customer, I want to be able to track the delivery of my purchased items so that I know when to expect them.

### Exercise | Requirement Elicitation

#### **Scenario**: 
*You are now tasked with gathering requirements for an online banking system. The system aims to provide a secure and user-friendly platform for customers to manage their accounts, transfer funds, and view transaction history.*

#### **Tasks**:
1. **Stakeholder Identification**:
    - Identify and analyze stakeholders for the online banking system.
    - Consider both internal (bank employees) and external (customers) stakeholders.
2. **Requirements Gathering**:
    - Choose and justify a requirements-gathering technique for the online banking system.
    - Provide a sample set of questions or methods you would use in an interview or survey.
3. **Types of Requirements**:
    - List at least three functional and three non-functional requirements for the online banking system.
4. **Use Cases and User Stories**:
    - Create a use case or user story related to a fund transfer scenario in the online banking system.

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


## **System Architecture**

### **Introduction to System Architecture**

#### **Definition**: 
***System Architecture** refers to the high-level structure of a software system, defining how different components and modules interact with each other. It outlines the organization of a system, including hardware and software components, their relationships, and how they work together to achieve the system's objectives.*

#### **Importance**:

1. **Blueprint for the System**: It serves as a blueprint, providing a conceptual model of the entire system.
2. **Communication Tool**: It helps communicate the design and structure of the system to stakeholders.
3. **Foundation for Development**: It provides the foundation for the development team to build the system.

### **Key Components of System Architecture**

1. **Hardware Components**:
    - **Examples**: Servers, storage devices, and network infrastructure.
    - **Role**: Physical components that support the execution of software.
2. **Software Components**:
    - **Examples**: Operating systems, middleware, databases.
    - **Role**: Programs and applications that run on the hardware, enabling functionality.
3. **Network Components**:
    - **Examples**: Communication protocols, routers, and switches.
    - **Role**: Enable communication and data exchange between different system components.

### **Exercise | Designing System Architecture**

#### **Scenario**:
You are tasked with designing the system architecture for an e-commerce platform. The platform must handle a large number of concurrent users, provide fast response times, and ensure data security.

#### **Tasks**:
- **Identify Key Components**:
    - List the key hardware, software, and network components necessary for the e-commerce platform.
- **Choose an Architecture**:
    - Select an architecture type (e.g., Monolithic, Microservices, Client-Server) based on the requirements of the e-commerce platform.
    - Justify your choice with specific reasons.
- **Scalability and Performance**:
    - Propose strategies for ensuring scalability and high performance in the e-commerce platform's architecture.
    - Consider load balancing, caching, and other relevant techniques.
- **Documentation**:
    - Create a clear and concise document outlining the chosen architecture, key components, and scalability/performance considerations.

#### **Solution**:

---
- **Key Component**
    - **Hardware**
        1. **Server**:
            - **Role**: Physical machines or virtual instances, where the e-commerce web app will run
            - **Example**: Web servers, Application Server
        2. **Storage**:
            - **Role**: Data storage for web applications, database and file storage
            - **Example**: Relational Database, Object storage
    - **Software**:
        1. **Tech Stack**:
            - **Role**: This includes a programming language, framework and database
            - **Example**: Nodejs, Reactjs, MongoDB
        2. **Message Queue**:
            - **Role**: For asynchronous communication between different components
            - **Example: Apache Kafka for building event-driven architecture. 
    - **Network**:
        1. **Internal Connectivity**
            - **Role**: Network components for internal connectivity
            - **Example**: Router, Switches
- **Architecture**
    - **chosen architecture**: Microservices Architecture
    - **justification**: 
        1. **Scalability**: Microservices allow independent scaling for each service
        2. **Flexibility**: Customisation for each service allows flexibility
        3. **Fault tolerance**: An issue in one service, will not affect the other service working.
- **Scalability and Performance**
    - **Load balancing**: Distribute incoming network traffic on multiple servers to ensure optimal use of resources.
    - **Caching**: Use a cache system, to avoid extra load on the database.
    - **Asynchronous Processing**: Use message queues for asynchronous processing of tasks to improve system responsiveness
- **Documentation**:
    - **System Architecture Document**
        - **Overview**: Design a complete working E-commerce website. Users must be able to add a product and buy it.
    - **Key Component**
        - **Hardware**
            1. **Server**:
                - **Role**: Physical machines or virtual instances, where the e-commerce web app will run
                - **Example**: Web servers, Application Server
            2. **Storage**:
                - **Role**: Data storage for web applications, database and file storage
                - **Example**: Relational Database, Object storage
        - **Software**:
            1. **Tech Stack**:
                - **Role**: This includes a programming language, framework and database
                - **Example**: Nodejs, Reactjs, MongoDB
            2. **Message Queue**:
                - **Role**: For asynchronous communication between different components
                - **Example: Apache Kafka for building event-driven architecture. 
        - **Network**:
            1. **Internal Connectivity**
                - **Role**: Network components for internal connectivity
                - **Example**: Router, Switches
    - **Architecture**
        - **chosen architecture**: Microservices Architecture
        - **justification**: 
            1. **Scalability**: Microservices allow independent scaling for each service
            2. **Flexibility**: Customisation for each service allows flexibility
            3. **Fault tolerance**: An issue in one service, will not affect the other service working.
    - **Scalability and Performance**
        - **Load balancing**: Distribute incoming network traffic on multiple servers to ensure optimal use of resources.
        - **Caching**: Use a cache system, to avoid extra load on the database.
        - **Asynchronous Processing**: Use message queues for asynchronous processing of tasks to improve system responsiveness
---

## **Database Design**
*Database design serves as the backbone of a system, influencing its efficiency, scalability, and data integrity.*

### **Importance of Database Design**
*Database design is a critical aspect of system development, influencing the efficiency, reliability, and performance of the entire system.*

1. **Data Integrity**: Ensuring accuracy and consistency of data by avoiding redundancy and dependency issues.
2. **Efficient Retrieval**: Designing for efficient data retrieval and storage, particularly in scenarios with large datasets.
3. **Scalability**: Allowing the system to scale seamlessly as data volume and user interactions grow.
4. **Relationships**: Simplifying database maintenance tasks, reducing the likelihood of errors and improving overall system reliability.

### **Key Concepts in Database Design**

1. **Entity-Relationship (ER) Modeling**:
    - **Definition**: A visual representation of the relationships between different entities (objects) in the system.
    - **Purpose**: Helps define the structure of the database and how data entities are related.
    - **Practical Application**: Identify entities (e.g., User, Product, Order), and attributes, and establish relationships. For example, a User places multiple Orders.
2. **Normalization**:
    - **Definition**: A process of organizing data to eliminate redundancy and dependency issues.
    - **Purpose**: Reduces data anomalies, improves data integrity, and simplifies database maintenance.
    - **Practical Application**: Identify attributes for each entity and apply normalization rules to minimize data anomalies. For instance, ensuring that data is stored in the most efficient way possible, such as avoiding repeating groups.
3. **Indexing**:
    - **Definition**: Creating indexes on specific columns to speed up data retrieval operations.
    - **Purpose**: Enhances query performance by allowing the database engine to quickly locate and access relevant data.
    - **Practical Application**: Identify columns frequently used in queries and create indexes to optimize data access. For example, indexing on the "product_id" column for efficient product lookups

### **Exercise | Database Design - Entity-Relationship Modeling**

#### **Scenario**:
You are tasked with designing the database for the e-commerce platform discussed in the previous exercise. The database should capture information about users, products, orders, and transactions.

#### **Tasks**:
- **Identify Entities**:
    - List the main entities relevant to the e-commerce platform (e.g., User, Product, Order).
- **Define Relationships**:
    - Establish relationships between entities (e.g., A User can place multiple Orders).
- **Attributes and Data Types**:
    - Identify key attributes for each entity and define their data types (e.g., User has attributes like username, email, password).
- **Normalization**:
    - Apply normalization techniques to eliminate redundancy and dependency issues.

### Solution

---
- **Identify Entities**:
    1. **User**
    2. **Product**
    3. **Order**
    4. **Transaction**
    5. **Payment Mode**
    6. **Aggregator**
    7. **COD Data**
    8. **Product Level COD DATA**
- **Define Relationships**:
    - **User** relates with
        - **Order**: User A, placed an order with order_id as `ord0000001`
        - **Transaction**: User A, paid some amount with transacton_id as `TR0000001`
        - **COD Data**: User A, has COD data, such as cod order limit  with id as `COD0000001`
    - **Product** relates with
        - **Product Level COD DATA**: Product P, has COD data such as product level cod charges
    - **Order** relates with
        - **User**: Order is placed by User
        - **Product**: The order contains a list of product IDs, which were part of the order
        - **Transaction**: Order payments are linked with a transaction
        - **COD Data**: If COD order, all details for COD order linked
    - **Transaction**: relates with
        - **User**: Each transaction is linked with a user
        - **Order**: Each transaction is linked with an order
        - **Payment Mode** Each transaction is linked with a payment mode.
    - **Payment Mode**: relates with
        - **Aggregator** Each payment mode is powered by an aggregator.
    - **Aggregator**: relates with
        - **Payment Mode**: Each payment mode is linked to an aggregator
    - **COD Data** relates with
        - **User**: Each user is linked with COD Data
        - **Order**: Order is linked to COD Data if a COD order were placed
    - **Product Level COD DATA**
        - **Product**: Product level COD Data
- **Attributes and Data Types**:
    1. **User**
        - user_id: String
        - name: String
        - email: String
        - phone_number: String
        - user_cod_id: String
    2. **Product**
        - product_id: String
        - product_name: String
        - product_price: Float
        - prouct_cod_id: String
    3. **Order**
        - order_id: String
        - transaction_id: String
        - user_id: String
        - amount: Float
        - order_time: Datetime
        - product_ids: String
    4. **Transaction**
        - transaction_id: String
        - order_id: String
        - user_id: String
        - amount: Float
        - is_cod: boolean
        - payment_mode_id: Integer
    5. **Payment Mode**
        - payment_mode_id: Integer
        - payment_mode_name: String
        - aggregator_id: Integer
    6. **Aggregator**
        - aggregator_id: Integer
        - aggregator_name: String
        - is_active: boolean
    7. **COD Data**
        - cod_id: String
        - cod_limit: Float
        - user_id: String
    8. **Product Level COD DATA**
        - prouct_cod_id: String
        - cod_limit: Float
- **Normalization**
    - Already in Normalized form
---

## **Security in System Design**

### **Importance of Security in System Design**

*Security is a critical aspect of system design, protecting against potential threats and ensuring the confidentiality, integrity, and availability of data.*

#### **CIA | Confidentiality, Integrity, Availability**
- **Confidentiality**:
Protecting sensitive information from unauthorized access.
- **Integrity**:
Ensuring that data remains accurate and unaltered.
- **Availability**:
Guaranteeing that the system and its resources are available when needed.

### **Key Concepts in System Security**

#### **Authentication**
*Authentication is the process of verifying the identity of a user, system, or device.*

- **Methods**:
    - **Passwords**: Traditional but should be strong and secure.
    - **Biometrics**: Fingerprint, facial recognition.
    - **Two-Factor Authentication (2FA)**: Adds an extra layer of security.

#### **Authorization**
*Authorization is the granting of access rights to authenticated users based on their roles and permissions.*

- **Implementation**:
    - **Role-based Access Control (RBAC)**: Assigns permissions based on user roles.
    - **Access Control Lists (ACLs)**: Lists specifying user permissions for specific resources.

#### **Encryption**:
*Encryption involves converting data into a secure format to prevent unauthorized access.*

- **Types**:
    - **Symmetric Encryption**: Uses a single key for both encryption and decryption.
    - **Asymmetric Encryption**: Utilizes a pair of public and private keys.

### **Exercise | Security in System Design**

#### **Scenario**:

*Enhance the security of the e-commerce platform by identifying potential security threats and proposing measures to mitigate risks.*

#### **Tasks**:

- **Identify Security Threats**:
    - List potential security threats (e.g., unauthorized access, data breaches).
- **Authentication Measures**:
    - Propose authentication methods to ensure only legitimate users access the system.
- **Authorization Strategies**:
    - Define authorization strategies to control access rights based on user roles.
- **Encryption Techniques**:
    - Specify encryption techniques to secure sensitive data during transmission and storage.

### **Solution**

---
- **Security Threats**:
    - Unauthorized access to the database will cause
        - order data issue
        - aggregator data issue
        - product pricing issue
        - cod limit issue
    - Data breach to the database will cause
        - leak of private information about users 
        - leak of aggregator credentials
        - leak of orders made by the customer
- **Authentication Measures**:
    - Access to the database must be password-protected
- **Authorization Strategies**:
    - Read and Write access must be maintained via RBAC and ACLs
- **Encryption Techniques**:
    - user data and aggregator data must be encrypted to avoid issues in case of a data breach
---