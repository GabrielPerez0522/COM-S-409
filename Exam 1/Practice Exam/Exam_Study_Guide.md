
# Exam Study Guide

## Question 1: Event-Driven Requirements

### Q1.1: The SafeBox customer tells you “The LED needs to light up at the time that the patient closes the pillbox compartment.” Which EARS template should be used to state this requirement?
- **Answer**: The EARS template to use for this requirement is **Event-driven**.

### Q1.2: What is the keyword for this template?
- **Answer**: The keyword for this template is **WHEN**.

### Explanation:
This requirement describes a situation where the system responds to an event (the closing of the pillbox compartment), which aligns with the Event-driven EARS template. The keyword "WHEN" is used to define the trigger event in the template.

---

## Question 2: How does the SafeBox software know the state of the compartment’s lid?
- **Answer**: The SafeBox software knows the state of the compartment’s lid through **Sensors**.

### Explanation:
The system uses sensors to detect whether the pillbox compartment is open or closed. This input allows the system to trigger the LED or other functionalities as needed.

---

## Question 3: Exception Scenario for "Reschedule Missed Pill"

### Q3: Identify and briefly describe an exception (off-nominal) scenario for the SafeBox Scenario “Reschedule Missed Pill,” where the precondition “Compartment contains Pill” is also met in the exception scenario. 
- **Answer**: An example of an exception scenario is that **the pill cannot be rescheduled due to a medication conflict with other pills**.

### Explanation:
The system is designed to handle cases where a missed pill can be rescheduled, but an exception might occur when rescheduling would cause a medication conflict. This describes a valid scenario that is not part of the normal flow but should still be considered in system behavior.

---

## Question 4: Mine Safety Control System (MSCS)

### Q4.1: List the Adjacent Systems that are not sensors in the Context Diagram for the Mine Safety Control System. 
- **Answer**: The adjacent systems are:
  - **Pump**
  - **Alarm**
  - **Operator**

### Explanation:
Adjacent systems are those with which the Mine Safety Control System (MSCS) communicates but are not part of the internal logic of the system, such as sensors. These external systems are critical for the functioning of the mine safety system.

### Q4.2: List the data/signals that the Mine Safety Control System sends to Adjacent Systems.
- **Answer**:
  - **Turn Pump On/Off**
  - **Turn Alarm On/Off**
  - **Alert Operator**

### Explanation:
These signals are the commands the MSCS sends to the adjacent systems, dictating their behavior in response to monitored conditions, such as water levels and dangerous gas concentrations.

### Q4.3: Which of these use cases does not belong in the Product Use Case Diagram for the Mine Safety Control System?
- **Answer**: The use cases that do not belong are **1, 4, 5, 6**:
  - 1. Methane sensors placed appropriately
  - 4. Pump malfunctions
  - 5. Carbon monoxide reaches dangerous levels
  - 6. Miners evacuate mine area

### Explanation:
These use cases either describe physical actions outside the control of MSCS (like sensor placement and evacuation) or involve external system behavior that the MSCS does not directly control.

### Q4.4: What is the rationale for the requirement to keep the pump off if the methane level is high?
- **Answer**: The rationale is to **avoid explosion**.

### Explanation:
Methane is a highly flammable gas, and operating a pump in an environment with a high methane concentration could trigger an explosion. Therefore, the system must ensure the pump is turned off under such conditions.

---

## Question 5: Eliciting and Documenting Requirements

### Q5: Which two of the following approaches are particularly well suited to elicit and document the requirements in this case?
- **Answer**: The two most suited approaches are:
  - **a) Establishing a glossary**
  - **c) Creating a use case diagram and documenting the use cases**

### Explanation:
A glossary ensures that all stakeholders use consistent terminology, which is critical in complex systems like MSCS. Use case diagrams provide a clear, structured way of understanding system behavior and interactions.

---

## Question 6: Nonfunctional Requirement Category

### Q6: What category of nonfunctional requirement is this: “FINDER shall save parameter settings in a persistent way so that they can be restored after battery failure”?
- **Answer**: The category is **Performance**, specifically under reliability.

### Explanation:
This requirement addresses the system’s ability to maintain functionality (saving and restoring settings) even after a failure, which is a key aspect of system reliability and performance.

---

## Question 7: True or False Questions (409 Only)

### Q7.1: “The X software application shall comply with the accessibility standards of company Y, available at Y.com/Z” is a non-functional requirement.
- **Answer**: **True**

### Q7.2: “The system shall have high availability from 8 a.m. to 6 p.m on weekdays” is a non-functional requirement.
- **Answer**: **True**

### Q7.3: Some requirements describe qualities the software product being developed must have instead of what it must do.
- **Answer**: **True**

### Q7.4: Sending a “TURN OFF” command to the SafeBox LED is an event, not a state.
- **Answer**: **True**

---

## Question 8: Soft Goal (509 Only)

### Q8: Is this a soft goal? Explain why or why not: “SafeBox should notify the caregiver as soon as possible about a missed pill.”
- **Answer**: **Yes**, this is a soft goal because it expresses a **preference** for notifying the caregiver quickly, but does not specify an exact measurable threshold.

### Explanation:
Soft goals are often more subjective and describe a preferred system behavior without precise metrics. This goal expresses a general preference for timely notifications.

---

## Question 9: Phenomena Classification (509 Only)

### Q9: Label each as a “Shared phenomenon”, “Environmental phenomenon”, “Software phenomenon”, or “Environmental assumption”:

- **(a) Train is physically moving.**  
  - **Answer**: **Environmental Phenomenon**

- **(b) Train’s measured speed is X.**  
  - **Answer**: **Shared Phenomenon**

- **(c) Train’s position is updated in the controller’s internal database.**  
  - **Answer**: **Software Phenomenon**

### Explanation:
Environmental phenomena are events that occur outside the software’s direct control, shared phenomena are observed by both the environment and software, and software phenomena are internal to the system.

