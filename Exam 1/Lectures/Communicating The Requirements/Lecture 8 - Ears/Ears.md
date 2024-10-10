# Lecture 8: Communicating the Requirements

## Key Concepts:

### 1. Importance of Clear Requirements
- **Why are requirements hard to write?**
  - Finding out what is actually needed is challenging.
  - Expressing requirements clearly in text can lead to:
    - **Ambiguity**: Vague or unclear wording.
    - **Premature design decisions**: Including implementation details too early.
    - **Difficult to test**: Requirements that are hard to validate through testing.
  
### 2. EARS (Easy Approach to Requirements Syntax)
- **EARS** is a structured method for writing clear, concise, and testable requirements.
- It simplifies the communication of requirements, reduces misunderstandings, and ensures that the right product is being built.

### 3. Types of EARS Templates:
EARS classifies all requirements into **five basic templates**:

#### 1. Ubiquitous Requirements:
   - Requirements that always apply to the system.
   - **Template**:  
     ```  
     The <system> shall <response>.
     ```
   - **Example**: "The library system shall comply with data privacy regulations."

#### 2. Event-Driven Requirements:
   - Triggered by an external event detected by the system.
   - **Keyword**: **WHEN**
   - **Template**:
     ```
     WHEN <event>, the <system> shall <response>.
     ```
   - **Example**: "WHEN a book is reserved, the system shall send a notification to the user."

#### 3. State-Driven Requirements:
   - Active while a certain state is true.
   - **Keyword**: **WHILE**
   - **Template**:
     ```
     WHILE <state>, the <system> shall <response>.
     ```
   - **Example**: "WHILE the book is available, the system shall allow reservations."

#### 4. Option-Based Requirements:
   - Requirements that apply only under specific conditions.
   - **Keyword**: **WHERE**
   - **Template**:
     ```
     WHERE <condition>, the <system> shall <response>.
     ```
   - **Example**: "WHERE premium membership is active, the system shall allow extended loan periods."

#### 5. Unwanted Behavior Requirements:
   - Defines the system's response to errors or unwanted events.
   - **Keyword**: **IF/THEN**
   - **Template**:
     ```
     IF <unwanted event>, THEN the <system> shall <response>.
     ```
   - **Example**: "IF the book database is unavailable, THEN the system shall notify the administrator."

---

### 4. Combining EARS Templates:
EARS templates can be combined to handle more complex requirements.

- **Example**:
WHILE the library is open, WHEN a user returns a book, the system shall update the book status to 'available.'

- **Another Example**:

---

## Benefits of EARS:
- **Improved clarity**: Requirements are written in a structured way that’s easy to understand.
- **Reduces ambiguity**: Clear separation of system states, events, and conditions.
- **Easy to test**: The structure allows easy validation of whether the system meets its requirements.

---

