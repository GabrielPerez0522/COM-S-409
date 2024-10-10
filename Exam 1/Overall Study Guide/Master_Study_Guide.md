
# Master Study Guide for Exam

## 1. Context Diagrams
- **Definition**: A visual representation of the system and its interaction with external systems or actors.
- **Components**:
  - System (represented as a box)
  - Adjacent systems/actors (external entities)
  - Arrows showing the flow of data/signals between the system and external entities.
- **Example**: The Mine Safety Control System (MSCS) context diagram, where adjacent systems like the **Pump**, **Alarm**, and **Operator** are shown interacting with the MSCS.

## 2. Product Use Case (PUC) Diagrams
- **Definition**: The part of the Business Use Case (BUC) that is handled by the automated system.
- **Example**: In bpMON, the PUC focuses on the software functionality for monitoring systems, while the BUC might include human tasks or hardware actions.
  
## 3. Scenarios and User Stories
- **Scenarios**: Descriptions of how the system will be used, outlining specific sequences of events.
- **User Stories**: A simpler version of scenarios, typically used in Agile frameworks.
  - **Format**: As a <type of user>, I want <some goal> so that <some reason>.
- **Exception Scenario** Example: For SafeBox, if the "pill cannot be rescheduled due to a medication conflict," this would be an exception to the normal flow.

## 4. Functional Requirements (FR) and Nonfunctional Requirements (NFR)
- **Functional Requirements (FR)**:
  - What the system **must do** (actions, processes).
  - Example: “The MSCS shall turn the pump on when the water level is high.”
  
- **Nonfunctional Requirements (NFR)**:
  - Qualities or properties the system **must have**.
  - **Categories**:
    1. Performance
    2. Security
    3. Usability
    4. Reliability
    5. Maintainability
    6. Scalability
    7. Legal/Compliance
    8. Portability
  - **Example**: “FINDER shall save parameter settings in a persistent way so that they can be restored after battery failure” (relates to performance/reliability).

## 5. Requirements Discovery Techniques
- **EARS (Easy Approach to Requirements Syntax)**:
  - A structured method to define system requirements.
  - **Templates**:
    - **Event-driven**: Triggered by an external event (e.g., "When the compartment is closed, the LED shall light up").
    - **State-driven**: Active while the system is in a specific state (e.g., "While the system is in safe mode, the alarm shall remain off").
    - **Ubiquitous**: Always active (e.g., "The system shall always record sensor data").
    - **Option**: Applicable only under specific conditions (e.g., "If a backup battery is present, the system shall provide additional runtime").
- **Context Diagram Analysis**: Helps identify the external systems and their interaction with the main system.
- **Use Case Analysis**: Identifying user interactions with the system to derive functional requirements.
  
## 6. Traceability
- **Two-way Traceability**: Ensures that each requirement can be traced back to a business need and that every business need has corresponding system requirements.
- **Examples**:
  - Traceability between functional requirements and system design components.
  - Mapping nonfunctional requirements to the system’s architectural choices (e.g., performance → database optimization).

## 7. Rationale
- **Definition**: The reasoning or justification behind a requirement.
- **Why Include Rationale?**
  - Helps developers understand the importance and impact of a requirement.
  - Assists testers in determining the priority of testing efforts.
  - Aids maintainers in evaluating the effects of changing or removing a requirement.
  - **Example**: Keeping the pump off when methane levels are high is justified by the need to **avoid explosion** risks.

## 8. Industry Insights
- **Lessons from Industry**:
  - **Importance of Rationale**: As seen in NASA’s Flight Software Complexity study, poorly justified requirements can lead to costly system complexity.
  - **Elicitation Techniques**:
    - Establishing a glossary for consistent terminology.
    - Creating use case diagrams to document system functionality clearly.

## 9. Data and State Models
- **Data Models**: Represent the relationships between data entities within the system.
  - **Example**: A class diagram showing the relationship between a Customer, Order, and OrderLine in a shopping system.
- **State Models**: Represent the different states the system can be in and the transitions between them.
  - **Example**: A state model showing transitions between "empty", "occupied", and "in use" for a room.

## 10. Exam Practice (Based on Old Exam)
- **Question 1**: Which EARS template should be used for a requirement that involves the LED lighting up when the patient closes the pillbox? 
  - **Answer**: Event-driven (Keyword: WHEN).
  
- **Question 2**: How does the SafeBox software know the state of the pillbox compartment’s lid?
  - **Answer**: Through sensors.

- **Question 3**: Exception Scenario: “Pill cannot be rescheduled due to a medication conflict.”
  
- **Question 4**: What is the rationale for keeping the pump off when methane levels are high?
  - **Answer**: To avoid the risk of explosion.

---

### Final Notes:
- **Key Focus Areas**:
  - Context and Use Case diagrams.
  - Functional and Nonfunctional requirements (FR and NFR).
  - EARS templates for clear and structured requirements.
  - Rationale: Always question “why” a requirement exists.
  - Data and State models: Understand both static data relations and dynamic system behavior.
  
Good luck on your exam! Review your old homework, and focus on understanding the techniques, diagrams, and examples discussed in class.
