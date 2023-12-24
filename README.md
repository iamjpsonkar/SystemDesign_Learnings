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
1. user must be logged-in, before buying
2. seller must have added some products in web app, to get the desired result.
---