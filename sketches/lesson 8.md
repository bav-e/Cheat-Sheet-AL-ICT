# **Plan for Lesson 8 Cheat Sheet: Database Design**

### **The Goal**

To create a comprehensive, single-page reference sheet that focuses heavily on the theoretical aspects of database design, particularly ER Diagrams and Normalization, which are crucial for A/L essay questions. The SQL section will be condensed to cover only the essential commands needed for MCQs and structured questions.

### **The Structure: "From Blueprint to Implementation"**

The cheat sheet will be structured into four logical parts, prioritizing the design and theory aspects over practical SQL implementation.

## **Content List for the Cheat Sheet**

### **Part 1: The "Why" \- Database Fundamentals**

*(This section provides the necessary theoretical foundation.)*

* **Core Concepts:** Data vs. Information, Structured vs. Unstructured Data.  
* **Database:** An organized collection of structured information.  
* **Database Models (Evolution):**  
  * Flat-file: Simple text files. *Problem: High redundancy.*  
  * Hierarchical: Tree-like structure (one-to-many).  
  * Network: Graph-like structure (many-to-many).  
  * Relational: The modern standard; data stored in tables.  
  * Object-Relational: Combines relational and object-oriented concepts.

### **Part 2: The "Blueprint" \- Conceptual Design (ER & EER Diagrams)**

*(This is the main focus area for the essay question.)*

* **ER Diagrams (Entity-Relationship Diagrams):** The visual blueprint of a database.  
  * **Components & Standard Symbols:**  
    * Entity: Rectangle.  
    * Attribute: Oval.  
    * Key Attribute: Oval with underlined text.  
    * Relationship: Diamond.  
* **Relationship Cardinality (How many are related?):**  
  * One-to-One (1:1)  
  * One-to-Many (1:M)  
  * Many-to-Many (M:M)  
* **EER (Extended ER) Diagrams:**  
  * A brief note on its purpose: Used for more complex designs involving specialization and generalization.

### **Part 3: The "Structure" \- Relational Model & Normalization**

*(This part is also crucial theory for essay questions.)*

* **Relational Schema (The Logical Plan):**  
  * **Terminology:** Relation (Table), Tuple (Row), Attribute (Column).  
* **Key Types (The rules that link the data):**  
  * **Candidate Key:** An attribute that can uniquely identify a row.  
  * **Primary Key (PK):** The chosen candidate key. *Cannot be NULL, must be UNIQUE.*  
  * **Alternate Key:** A candidate key that was *not* chosen as the PK.  
  * **Foreign Key (FK):** A primary key from one table used in another to create a link.  
* **Normalization (The "Quality Control" process):**  
  * **Purpose:** To reduce **data redundancy** and avoid **anomalies** (errors during Insert, Update, Delete).  
  * **Functional Dependencies (The rules behind normalization):**  
    * Partial Dependency: A non-key attribute depends on only a *part* of a composite PK.  
    * Transitive Dependency: A non-key attribute depends on *another non-key attribute*.  
  * **The Normal Forms (Step-by-step refinement):**  
    * **1NF:** No repeating groups / All values are atomic.  
    * **2NF:** Must be in 1NF \+ No partial dependencies.  
    * **3NF:** Must be in 2NF \+ No transitive dependencies.

### **Part 4: The "Tools" \- Essential SQL Commands**

*(This section is condensed for MCQs and structured questions.)*

* **SQL Sub-languages:**  
  * **DDL (Data Definition Language):** Defines the structure.  
  * **DML (Data Manipulation Language):** Manages the data.  
* **Essential DDL Commands:**  
  * CREATE TABLE  
  * ALTER TABLE  
  * DROP TABLE  
* **Essential DML Commands:**  
  * INSERT INTO  
  * UPDATE ... SET ... WHERE  
  * DELETE FROM ... WHERE  
* **The Core SELECT Query:**  
  * SELECT columns FROM table WHERE condition.  
  * **Key Clauses:** ORDER BY, GROUP BY, INNER JOIN.  
* **Essential Constraints:**  
  * NOT NULL, UNIQUE, PRIMARY KEY, FOREIGN KEY, CHECK.