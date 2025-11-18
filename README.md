# Relational Database Design and Normalization

Designed and engineered a complete, normalized relational database schema based on a set of business requirements. The goal was to apply advanced conceptual modeling (EER) and logical design (normalization) principles to ensure data integrity, scalability, and elimination of anomalies across multiple use cases.

![Database](https://img.shields.io/badge/Database-Relational_Design-00758F.svg)
![Tools](https://img.shields.io/badge/Tools-Draw.io_|_Lucidchart-E96A00.svg)

## 🎯 Project Overview

This project demonstrates the end-to-end database design lifecycle, from analyzing business rules to producing a production-ready, fully normalized logical schema.

The process involved:
1.  **Conceptual Modeling:** Analyzing requirements for complex systems (like a cloud gaming service and a professional networking site) and creating Enhanced Entity-Relationship (EER) diagrams.
2.  **Logical Design:** Translating the conceptual EER models into a logical relational schema (a set of tables and keys).
3.  **Normalization:** Systematically applying normalization rules (from 1NF to BCNF) to the logical schema to eliminate data redundancy and prevent anomalies.

---

## 1. Conceptual Modeling (EER)

The first step was to translate ambiguous business rules into a formal, visual model. This was done using **Enhanced Entity-Relationship (EER) diagrams** in Chen notation.

This stage involved modeling complex data constructs, including:
* **Specialization/Generalization:** (e.g., an `Event` entity generalizing `Social`, `Conference`, and `Sport` sub-types).
* **Shared Subclasses (Multiple Inheritance):** Modeling entities that inherit from two or more superclasses.
* **Categories (Union Types):** Representing relationships where one entity can be one of *several* different entity types.

> **[Image: EER Diagram for the "FindJob" or "Survive" Platform]**
>
> *(**Developer Note:** Place your `FindJob_EER.png` or `Survive_EER.png` image here. It's the best example of your conceptual modeling skill.)*

---

## 2. Logical Design & Normalization

The conceptual EER model was then mapped to a logical relational schema (a blueprint of tables). This schema was then refined using **normalization** to ensure data integrity.

**Process:**
1.  **Identify Functional Dependencies (FDs):** Analyzed the attributes within each relation to determine the FDs (e.g., `StudentID -> StudentName`).
2.  **Decomposition to BCNF:** Systematically decomposed relations that violated normalization rules.
    * **1NF:** Ensured all attributes are atomic.
    * **2NF:** Removed partial dependencies.
    * **3NF:** Removed transitive dependencies.
    * **BCNF (Boyce-Codd Normal Form):** Ensured every determinant is a candidate key, resolving any remaining anomalies.

This process minimizes redundancy and prevents insertion, update, and deletion anomalies, resulting in a robust and maintainable database.

> **[Image: Screenshot of the final normalized relational schema]**
>
> *(**Developer Note:** A screenshot of the text-based schema from **Page 6 of `db-design-normalization.pdf`**  would be perfect here to show the final logical model.)*

---

## 🛠️ Key Skills & Artifacts

This project demonstrates expertise in the foundational principles of database design.

### Key Skills
* **Conceptual Data Modeling:** Translating requirements into abstract models (ER/EER).
* **Logical Data Modeling:** Mapping EER diagrams to relational schemas.
* **Database Normalization:** Applying 1NF, 2NF, 3NF, and BCNF to ensure data integrity.
* **Data Integrity:** Using primary keys, foreign keys, and relationship cardinalities (1:1, 1:N, M:N) to enforce business rules.
* **Design Tools:** `Draw.io` / `Lucidchart`.

### Project Artifacts
* **ER / EER Diagrams:** Conceptual blueprints for systems like "NCCCloud" and "FindJob".
* **Normalization Report:** A step-by-step analysis of functional dependencies and the decomposition process to achieve BCNF.
* **Final Relational Schema:** A "production-ready" logical schema, fully normalized and documented.