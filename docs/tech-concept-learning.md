---
id: tech-concept-learning
title: Tech Concept Learning
---

# Tech Concept Learning

## Domain-Driven Design

In acceptance of [Conway’s Law](https://en.wikipedia.org/wiki/Conway%27s_law), the team has adopted [Domain Driven Design](https://learn.microsoft.com/en-us/archive/msdn-magazine/2009/february/best-practice-an-introduction-to-domain-driven-design) to produce systems that align better with the company and are easier to build and maintain.

> 💡 Domain-Driven Design is neither a framework nor a library — but rather an approach to software development that fundamentally changes how you approach problems as a software developer.

## Domain Driven Design Resources

### Videos

- [Domain Driven Design: The Good Parts](https://www.youtube.com/watch?v=L3SvIKdLt88) (50 minutes)
- [DDD Fundamentals Playlist](https://www.youtube.com/playlist?list=PL2E-vlKoo_v3ch9oZWYZWwRbqdVoWHY8X)

### Books

- [Learning Domain-Driven Design](https://www.amazon.com/dp/1098100131)
- [Domain-Driven Design (Blue Book)](https://www.amazon.com/gp/product/0321125215/)

---

# Atomic Design

An approach used to help structure concepts in UI development.

## Atomic Design Resources

### Websites

- [Atomic Design](https://atomicdesign.bradfrost.com/) — Brad Frost
- [Atomic Design & Storybook](https://bradfrost.com/blog/post/atomic-design-and-storybook/) — Brad Frost
- [Structuring Storybook](https://storybook.js.org/blog/structuring-your-storybook/) — Storybook Blog
- [Atomic Design in Figma](https://www.figma.com/blog/creating-atomic-components-in-figma/) — Figma Blog

---

# General Architecture Concepts

## Event Types

- **Document Events**  
  Triggered when a field in a payload has been updated  
  *(e.g., Applicant’s last name is updated)*  
  Naming Convention: **Nouns** → `available-pizza-toppings`

- **Business Events**  
  Triggered when a business fact has occurred  
  *(e.g., Case Worker approves Pathways Application)*  
  Naming Convention: **Past Tense Verb** → `pizza-delivered`

- **Commands**  
  When an external system expects the system to perform a particular action  
  Naming Convention: **Verb** → `order-pizza`

- **Synchronous Requests**  
  When an external system connects, sends a message, and waits for an immediate response  
  Naming Convention: **Verb prefixed with request** → `request-order-pizza`

---

## Testing

- [Sub-Second Acceptance Tests](https://www.youtube.com/watch?v=AJ7u_Z-TS-A)

---

# BDD — Behavior Driven Development

- [BDD with Cucumber (Training Course)](https://school.cucumber.io/courses/bdd-with-cucumber-javascript)

Please also refer to the OneNote document in:
**CXA-UX and Dev → Standards → BDD**

---

# TDD — Test Driven Development

Please refer to the OneNote document in:
**CXA-UX and Dev → Standards → TDD**

---

# Documentation Concepts

- [Introduction](https://thepaulrayner.com/blog/2013/05/07/succeeding-with-ddd-documentation/)
- UML Sequence Diagrams  
  - [Intro Article](https://www.geeksforgeeks.org/unified-modeling-language-uml-sequence-diagrams/)