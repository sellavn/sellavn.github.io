---
layout: default
title: Home
---
# Professional Self-Assessment

## Introduction

The completion of the Computer Science program at Southern New Hampshire University marks a pivotal evolution in my technical capability. Supplementing academic coursework with concurrent full-time experience as a Tech Support Technician, this portfolio demonstrates my readiness to transition into a professional Cloud Engineering role. The included capstone project represents the synthesis of this journey: evolving a basic C++ course planner into a production-ready Python application complete with SQLite integration. This work demonstrates proficiency across software engineering, algorithmic optimization, and database management, all underpinned by a rigorous security-first mindset.

---

## Professional Skills Development

### Collaboration & Communication

Throughout the program, I learned that software development is fundamentally collaborative. Classes such as **CS-250 Software Development Lifecycle** taught me Agile methodologies and stakeholder communication, while **CS-255 System Analysis** reinforced the collaborative planning and execution that occurs throughout the SDLC. The capstone's modular architecture and comprehensive documentation reflect this collaborative mindset, code is written to be understood, critiqued, forked and maintained by others.

My enhancement narratives exemplify effective technical communication. Rather than listing changes, each explains the problem, approach, challenges, and lessons learned, explaining in a manner where both technical and non-technical audiences are kept in mind.

### Algorithms & Data Structures

CS-300 Data Structures and Algorithms provided the foundation for the majority of the capstone, but the key difference is where I replaced O(n) linear search in the original project with O(1) hash map lookups and implemented DFS for cycle detection. The performance benchmarks showed modest gains at small scale (1.9x speedup with 4 courses) but projected 1000x advantages at 4,000 courses, proving that algorithm selection matters for scalability.

The DFS implementation uses three sets to track visited nodes, current recursion path, and reported cycles. This serves to prevent infinite loops and duplicate errors \- something that was learned through making mistakes through previous iterations. This attention when testing to edge cases separates working code from production-ready code.

### Software Engineering & Databases

The program emphasized principles over technologies \- modularity, separation of concerns. Enhancement One transformed a monolithic C++ file into eight Python modules, each with a single responsibility. Enhancement Three integrated SQLite with proper normalization, foreign key constraints, and strategic indexes, going beyond basic CRUD to implement recursive CTEs for prerequisite chain analysis.

The ETL pipeline that migrates CSV to SQLite demonstrates that production systems require robust data migration strategies with transaction safety and error handling, not just schema design.

### Security Mindset

CS-305 Software Security taught me to consider vulnerabilities during initial design, not as afterthoughts \- as well as how devastating the effects can be in a multitude of ways if left unchecked. The capstone reflects this throughout, every database query uses parameterized statements, all input is validated, and security audit documentation proves compliance systematically.

What distinguishes a security mindset from awareness is anticipating adversarial behavior. When implementing the database layer, I considered what happens if users input special characters or attempt SQL injection. Parameterized queries aren't a feature; they're the minimum standard for responsible development.

---

## Portfolio Artifacts

### Enhancement One: Software Engineering & Design

Transformed a monolithic C++ console app into a professional Python CLI with modular architecture, argparse subcommands, configuration management, and data persistence. Demonstrates clean interfaces, maintainable organization, and user experience prioritization.

### Enhancement Two: Algorithms & Data Structures

Replaced linear search with hash map indexing (O(1) vs O(n)) and implemented DFS cycle detection with comprehensive edge case handling. Includes performance benchmarking showing projected 1000x speedup at scale.

### Enhancement Three: Databases

Integrated SQLite with normalized schema (3NF), transaction-based migration, 100% parameterized queries, and advanced SQL (recursive CTEs for prerequisite chains). Demonstrates database design, query optimization, and security-conscious development.

### Cohesion

Together, these artifacts showcase the full development lifecycle: architectural design from the code review, performance optimization throughout the milestones, and data persistence and security in the latter half of the project. The progression mirrors real-world software maturation from prototype to production.

### Career Readiness

My professional focus centers on infrastructure automation and Cloud Engineering, where the skills demonstrated in this capstone: Python scripting, database optimization, and security-conscious development. All of these have direct application within the industry. Professional distinction lies not just in implementation, but in a holistic approach to software development: prioritizing user experience, anticipating security threats, planning for scalability, and maintaining robust documentation. This portfolio evidences the ability to design, implement, optimize, and secure real-world systems, transforming academic theory into production-ready software solutions.


### [View My Capstone Project Repository](https://github.com/sellavn/CS-499-Capstone-Project)

---

## Milestone 1 Code Review

Here is the informal code review for my CS 499 capstone project. In this video, I walk through the existing functionality of my selected artifacts, analyze areas for improvement, and discuss my enhancement plan.

<iframe id="odysee-iframe" style="width:100%; aspect-ratio:16 / 9;" src="https://odysee.com/%24/embed/%40sellavn%3Ae%2FMilestone-1-NV%3Ae?r=4Z3jD1oxc5GQHp5icGrbhnQZ52t2dCZF&signature=b18b4fd9bd53f9613d80d24333aff4331721b55d039756069410531505a822c0034920130785807f8ee5413b350b17c90ab1ec6b232b35c2d4fd59b9c7b86361&signature_ts=1762724968" allowfullscreen></iframe>

---

## Milestone 2: Enhancement One - Software Engineering

* **Artifact:** CS-300 Project 2 (Course Planner in C++)
* **Enhancement:** Python CLI Tool

Enhancement One transforms a basic C++ course planning application into a professional Python command-line interface (CLI) tool. The enhancement demonstrates modern software engineering practices including:

- **Modular Architecture:** Separation of concerns across multiple modules (CLI, course logic, data models, configuration)
- **CLI Design:** `argparse` interface with subcommands (`load`, `list`, `search`, `clear`)
- **Configuration Management:** External config files for flexible deployment
- **Data Persistence:** `pickle` based caching for session continuity
- **Type Safety:** Comprehensive type hints and dataclasses
- **Cross-Platform Compatibility:** Works on Windows, macOS, and Linux

![Enhancement One running on macOS](/images/enhancement-one.png)

[View Enhanced Code on GitHub](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/enhancement-one) | [View Original Artifact](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/original-artifacts/CS-300) | [View Full Narrative](https://github.com/sellavn/CS-499-Capstone-Project/blob/main/docs/Category%201%20Narrative%20Valles.md)

---

## Milestone 3: Enhancement Two - Algorithms

* **Artifact:** CS-300 Project Two (Original: C++)
* **Enhancement:** Advanced Data Structures & Algorithm Optimization

For the Algorithms and Data Structure category, I built on the previous enhancement which used the Course Planner project from CS-300. The goal of this enhancement was to optimize the application's performance and reliability by implementing advanced algorithmic concepts that were not addressed in the previous enhancement.

The enhancements focused on two key areas:
1.  **Optimization:** Replaced inefficient linear searches `O(n)` with a Hash Map indexing system `O(1)`.
2.  **Graph Traversal:** Implemented a Depth-First Search (DFS) algorithm to detect circular dependencies (cycles) in the course prerequisite graph - implemented via the `validate` command.

I also created a custom benchmarking script to quantify the performance improvements, demonstrating a performance increase on small datasets with massive scalability projected for larger datasets.

![Enhancement Two running on Windows](/images/enhancement-two.png)

[View Enhanced Code on GitHub](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/enhancement-two) | [View Original Artifact](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/original-artifacts/CS-300) | [View Full Narrative](https://github.com/sellavn/CS-499-Capstone-Project/blob/main/docs/Category%202%20Narrative%20Valles.md)

## Milestone 4: Enhancement Three - Databases

* **Artifact:** CS-300 Course Planner (Original: C++) & CS-360 Project (SQLite Baseline)
* **Enhancement:** Production-Ready SQLite Integration

For the Databases category, I enhanced the Course Planner to transition from volatile memory/file-based storage (Pickle/CSV) to a persistent SQLite relational database. While I added on the previous two enhancements which used CS-300 Project Two as an artifact - for Enhancement Three specifically, I used CS-360 Project 3, specifically the SQLite database component from that project to serve as a baseline. 

The enhancements focused on key areas such as:

- **ACID Compliance:** Transaction management with automatic rollback on errors.
- **Security:** Full implementation of parameterized queries to prevent SQL injection.
- **Normalization:** Implementation of a junction table for many-to-many course prerequisites.

Later in the following modules, I implemented my stretch goals in Enhancement Three so it serves as the definitive version of the project. The two stretch goals I implemented are:

1.  **Recursive Common Table Expressions (CTE):** A custom SQL query that analyzes the complete prerequisite chain for any course, finding all direct and indirect dependencies.
2.  **System Logging:** A dedicated logging system (`course_planner.log`) configured via `config.ini` to track operations and debugging data.

![Enhancement Three running on Linux(Mint)](/images/enhancement-three.png)

[View Enhanced Code on GitHub](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/enhancement-three) | [View Original Artifact](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/original-artifacts/CS-360) | [View Full Narrative](https://github.com/sellavn/CS-499-Capstone-Project/blob/main/docs/Category%203%20Narrative%20Valles.md)
