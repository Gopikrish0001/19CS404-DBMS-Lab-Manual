# Experiment 1: Entity-Relationship (ER) Diagram
# NAME :GOPIKRISHNAN M
# REGISTER NO: 212223043001
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name

## Scenario Chosen:
University 

## ER Diagram:

![er diagram university](https://github.com/user-attachments/assets/571fb603-3cac-4921-a335-f04756f16b2c)


## Entities and Attributes:
- University -
  Reg. No,Address,Student,DOB
- Mail ID -
  Course,Mobile No,Faculty
- Course -
  Course Code,Credits,Prerequisite,Students Enrolled,Course Name
- Instructors -
  Name,Course Taken,Address,Experience


## Relationships and Constraints:
- University–Student Relationship
Cardinality: One-to-Many (A university can have many students, but each student belongs to one university.)
Participation: Total (Every student must be associated with a university.)

- Student–Course Relationship
Cardinality: Many-to-Many (A student can enroll in multiple courses, and a course can have multiple students.)
Participation: Partial (A student may or may not enroll in a course.)

- Course–Instructor Relationship
Cardinality: Many-to-Many (A course can be taught by multiple instructors, and an instructor can teach multiple courses.)
Participation: Partial (A course may exist without an instructor assigned initially.)

- Extension (Prerequisite):
  In the course entity, prerequisites are modeled as an attribute indicating which course(s) must be completed before enrolling in the course. This adds dependency between different course entities.

## Design Choices:
- Entities:
Entities were chosen based on major participants in a university system (University, Student, Course, Instructor).
- Relationships:
Relationships were modeled to reflect real-world connections: students belong to a university, enroll in courses, and courses are conducted by instructors.
- Attributes:
Attributes cover important details needed for university operations — e.g., student contacts, course details, instructor background.
- Assumptions:
Each student belongs to only one university.
Courses can have prerequisites, but it’s optional.
Instructors can take multiple courses and have their own experiences noted separately.
Some relationships are partial, meaning entities can exist without always needing the related entity immediately (e.g., a course can exist before any students enroll).

## RESULT
Thus the ER daigram have been successfully drawn and explained briefly.
