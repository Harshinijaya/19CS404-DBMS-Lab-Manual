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
<img width="887" height="718" alt="Screenshot 2026-08-04 101151" src="https://github.com/user-attachments/assets/e3a45c9e-3032-4e1d-9a15-44122d52a636" />

Entities and Attributes
| Relationship         | Cardinality | Participation        | Notes                                                                                     |
| -------------------- | ----------- | -------------------- | ----------------------------------------------------------------------------------------- |
| MEMBER — PROGRAM     | M : N       | Partial              | A member can join multiple programs, and a program can have multiple members.             |
| PROGRAM — TRAINER    | M : N       | Partial              | A program can have multiple trainers, and a trainer can be assigned to multiple programs. |
| MEMBER — SESSION     | 1 : M       | Total for SESSION    | A member can book multiple personal training sessions.                                    |
| TRAINER — SESSION    | 1 : M       | Total for SESSION    | A trainer can conduct multiple personal training sessions.                                |
| SESSION — ATTENDANCE | 1 : 1       | Total for ATTENDANCE | Attendance is recorded for each personal training session.                                |
| MEMBER — ATTENDANCE  | 1 : M       | Total for ATTENDANCE | A member can have multiple attendance records.                                            |
| MEMBER — PAYMENT     | 1 : M       | Total for PAYMENT    | A member can make multiple payments for memberships and sessions.                         |
| SESSION — PAYMENT    | 1 : 0..1    | Partial for PAYMENT  | A session may or may not have a payment.                                                  |


### Assumptions
- 
- 
- 

---

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
<img width="1027" height="737" alt="Screenshot 2026-08-04 101239" src="https://github.com/user-attachments/assets/a534ad03-6b95-4a08-8f9b-c3ea71b31ab1" />


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
<img width="1280" height="838" alt="ER3" src="https://github.com/user-attachments/assets/0f79a017-6bec-427d-bdf3-e72d0ff3ad3d" />


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
