# Week 2 — Project Report, System Design and Database Planning

## Problem / Challenge

After finalizing the project idea, the next challenge was converting the initial concept into a structured Software Engineering project.

The project report had to clearly describe the system architecture, technology stack, functional requirements and interactions between different components. We also needed to represent the proposed system using appropriate UML diagrams.

Another problem was deciding what information would need to be stored in the database because Athena would require both institutional information and structured campus information.

## Problems Faced

One of the main difficulties was deciding which information should be represented as database entities and how the entities should be related.

For example, rooms should not be stored directly against an institution because a room belongs to a floor, and a floor belongs to a building.

The hierarchy was therefore defined as:

Institution → Building → Floor → Room

This helped make the database structure more consistent and extensible.

## Solution

We planned a relational database structure for Athena.

The initial database design included tables for:

> Institutions

> Students

> Administrators

> Departments

> Courses

> Buildings

> Floors

> Rooms

> Events

> Knowledge Documents

Relationships were established using primary keys and foreign keys.
