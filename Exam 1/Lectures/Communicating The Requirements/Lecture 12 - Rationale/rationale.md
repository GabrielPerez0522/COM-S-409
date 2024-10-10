
# Lecture 12: Communicating the Requirements - Rationale

## 1. Introduction
This lecture discusses the importance of documenting the rationale behind requirements, helping teams understand why a requirement exists and how it fits into the broader context of the project.

---

## 2. Rationale Defined
- **Definition**: The rationale is the reason or justification for a requirement (Chap. 12, p. 282).
- Including rationale is crucial to avoid unnecessary or overly strict requirements, providing context and justification for decisions.

### Why Include Rationale?
- Helps developers find the fit criteria.
- Allows teams to identify overly strict requirements.
- Aids in making trade-offs between conflicting requirements.
- Helps testers understand the priority of requirements.
- Supports maintainers in evaluating the impact of changes.

---

## 3. Example: NASA Study on Flight Software Complexity
- In a NASA mission, a scientist initially required 99% data completeness for observations. 
- The flight software team designed a complex system based on this requirement, adding redundant elements and fault detection.
- Upon review, the scientist relaxed the requirement as it was overly stringent, but the damage was done—time and effort were wasted due to a lack of initial rationale.

### Recommendation:
- Project management should emphasize the importance of requirements rationale and ensure proper rationale documentation to prevent similar issues (Lutz et al., 2013).

---

## 4. Avoiding Overly Strict Requirements
- **Easing Requirements**: Consider making requirements less stringent when feasible, especially if they are impractical for the project.
- **Removing Requirements**: If a requirement is inconsistent with the project’s budget or timeline, it may be necessary to remove it.
- **Variations and Alternatives**: Consider alternative approaches to requirements, or relaxing them at runtime, especially for non-critical systems.

---

## 5. Summary
Including the rationale for each requirement is a key part of ensuring the success of a project. It provides context, aids in decision-making, and helps avoid unnecessary work due to overly strict or poorly justified requirements. Proper rationale documentation reduces the risk of costly errors and wasted effort.

