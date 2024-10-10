
# Lecture 11: Data and State Models

## 1. Introduction
In this lecture, we focus on data and state models in the context of software requirements. The lecture covers data models, CRUD checks, and state models to help identify, refine, and communicate requirements effectively.

---

## 2. Data Models (Chapter 10)
Data models represent the business data and the relationships between them. They are often depicted using UML class diagrams and are essential during the requirements phase.

- **Definition**: A data model shows the classes of data and the associations between them.
- **Visual Representation**: High-level diagrams focusing on logical links and cardinalities.

![img](./images/10.4.png)

### Key Concept:
Each data class must be created, referenced, updated, and deleted as required by the use cases.

- **CRUD Check**: Ensure no class is missing requirements by checking if it has Create, Read, Update, and Delete operations.

---

## 3. Data Terminology and Dictionary
- **Class**: A collection of elementary data items that represent something important to the business.
- Examples: Customer, Employee, Order, Product, Service.
- **Data Dictionary**: A specification of the terms used in the requirements, down to the elemental level. This ensures consistent terminology across the project.

---

## 4. State Modeling (not covered in the textbook)
State models are widely used in real-time systems, where external stimuli influence the system's behavior.

- **State Machine Model**: Captures system behavior by showing how it changes state in response to events.
- **State Transitions**: Events that trigger a shift from one state to another.

### Example 1: State Model for a Door
This example demonstrates how a door moves between 'opened' and 'closed' states.

![img](./images/State-Model.png)

---

### Example 2: State Model for a Process
State diagrams help visualize transitions between states, such as a chess game where player turns and outcomes (e.g., win, draw) are the states.

![img](./images/State_model_for_process.png)

---

### Example 3: State Model for a System
In this example, a system receives input from three buttons and outputs signals based on the input sequence.

![img](./images/state_model_for_system.png)

---

## 5. Summary
- Data models and state models are key tools for representing business processes and system behavior.
- CRUD checks help ensure all aspects of a data class are covered in the requirements.
- State models provide a clear, visual representation of how a system or process transitions between states.

For further reading, review Chapters 10 and 17 on data modeling and defining business data.

