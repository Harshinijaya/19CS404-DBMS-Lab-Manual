# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_fitness.png)


### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|---------------------|-------|
| MEMBER | Member_ID (PK), Name, Membership_Type, Start_Date | Stores member registration details. |
| PROGRAM | Program_ID (PK), Program_Name | Stores gym programs such as Yoga, Zumba, and Weight Training. |
| TRAINER | Trainer_ID (PK), Trainer_Name | Stores trainer details. |
| MEMBER_PROGRAM | Member_ID (PK, FK), Program_ID (PK, FK) | Represents the programs joined by each member. |
| PROGRAM_TRAINER | Program_ID (PK, FK), Trainer_ID (PK, FK) | Represents trainers assigned to each program. |
| SESSION | Session_ID (PK), Member_ID (FK), Trainer_ID (FK), Session_Date, Session_Time | Stores personal training session details. |
| ATTENDANCE | Attendance_ID (PK), Member_ID (FK), Session_ID (FK), Attendance_Date, Status | Records attendance for each session. |
| PAYMENT | Payment_ID (PK), Member_ID (FK), Session_ID (FK), Amount, Payment_Date, Payment_Type | Tracks payments for memberships and sessions. |

### Relationships and Constraints


| Relationship | Cardinality | Participation | Notes |
|--------------|-------------|---------------|-------|
| MEMBER — PROGRAM | M : N | Partial | A member can join multiple programs, and a program can have multiple members. |
| PROGRAM — TRAINER | M : N | Partial | A program can have multiple trainers, and a trainer can be assigned to multiple programs. |
| MEMBER — SESSION | 1 : M | Total for SESSION | A member can book multiple personal training sessions. |
| TRAINER — SESSION | 1 : M | Total for SESSION | A trainer can conduct multiple personal training sessions. |
| MEMBER — PAYMENT | 1 : M | Total for PAYMENT | A member can make multiple payments for memberships and sessions. |
| SESSION — PAYMENT | 1 : 0..1 | Partial for PAYMENT | A session may or may not have a payment. |

### Assumptions

- Each member has a unique Member_ID.
- Each program has a unique Program_ID.
- Each trainer has a unique Trainer_ID.
- A member can join multiple programs.
- A program can have multiple members.
- A program can be assigned to multiple trainers.
- A trainer can be assigned to multiple programs.
- Each personal training session is booked by one member and conducted by one trainer.
- Attendance is recorded for each training session.
- A member can make multiple payments for memberships and training sessions.
- A payment may be associated with a membership or a personal training session.
- Membership type and start date are recorded during member registration.

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_library.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_restaurant.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
