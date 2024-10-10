
# EARS Tutorial Study Guide

## 1. Introduction
EARS (Easy Approach to Requirements Syntax) is a structured approach for writing system requirements in Natural Language (NL), commonly used in industries like aerospace and automotive.

## 2. Motivation
- Top-level system requirements are often written in NL by non-experts, leading to ambiguity.
- EARS provides simple, easy-to-apply guidance to avoid problems caused by unconstrained NL.

## 3. EARS Concepts
There are two main classes of requirements in EARS:
- **Normal operation**: System behaves as expected.
- **Unwanted behavior**: System response to deviations, failures, or disturbances.

### EARS Templates
There are five main EARS templates, four for normal operation and one for unwanted behavior. These templates help structure requirements in a consistent and clear way.

#### 3.1 Normal Operation
- **Ubiquitous**: Requirement is always active. No preconditions or triggers.
- **Event-driven**: Requirement is triggered by a specific event.
- **State-driven**: Requirement is active while the system is in a specific state.
- **Option**: Applicable only if a certain feature is included.

#### 3.2 Unwanted Behavior
- **If-then**: Triggered when specific unwanted behavior or failure occurs.

## 4. EARS Syntax
### 4.1 Generic Structure
`<Optional preconditions> <Optional trigger> the <System name> shall <System response>`

#### Ubiquitous Example:
- "The laptop shall have a minimum battery life of 5 hours."

#### Event-driven Example:
- "When the laptop is off and the power button is pressed, the laptop shall boot up."

#### State-driven Example:
- "While the laptop is in power-saving mode, it shall reduce the screen brightness."

#### Option Example:
- "Where a long-life battery is fitted, the laptop shall last for at least 10 hours."

#### Unwanted Behavior Example:
- "If the car detects an attempted intrusion, the car shall trigger the alarm."

## 5. Complex Requirements
- Complex requirements can be handled by combining keywords (When, While, Where, If-Then) to specify richer system behaviors.
- Example: "While the car is being driven, if the driver attempts to engage reverse gear, the car shall prevent engagement."

## 6. Strengths and Weaknesses of EARS
### Strengths:
- Provides rigor and consistency.
- Easy to learn and apply.
- Widely used in industry.

### Weaknesses:
- Limited inter-requirement coupling.
- Unsuitable for highly complex requirements.

## 7. Summary
EARS is a versatile and widely applicable approach for writing NL requirements. It forces deeper consideration of system behavior and helps eliminate ambiguity in requirements.
