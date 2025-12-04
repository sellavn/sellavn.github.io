---
layout: default
title: Home
---

## Welcome to my ePortfolio for CS 499. 

This site is currently under construction and will be updated throughout the course with my project, links to previous repos, narratives, and overall professional self-assessment.

---

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

[View Enhanced Code on GitHub](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/enhancement-one) | [View Original Artifact](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/original-artifacts/CS-300) | [View Full Narrative](https://github.com/sellavn/CS-499-Capstone-Project/blob/main/docs/Category%201%20Narrative%20Valles.docx)

---

## Milestone 3: Enhancement Two - Algorithms

* **Artifact:** CS-300 Project Two (Original: C++)
* **Enhancement:** Advanced Data Structures & Algorithm Optimization

For the Algorithms and Data Structure category, I built on the previous enhancement which used the Course Planner project from CS-300. The goal of this enhancement was to optimize the application's performance and reliability by implementing advanced algorithmic concepts that were not addressed in the previous enhancement.

The enhancements focused on two key areas:
1.  **Optimization:** Replaced inefficient linear searches ($O(n)$) with a Hash Map indexing system ($O(1)$).
2.  **Graph Traversal:** Implemented a Depth-First Search (DFS) algorithm to detect circular dependencies (cycles) in the course prerequisite graph - implemented via the `validate` command.

I also created a custom benchmarking script to quantify the performance improvements, demonstrating a performance increase on small datasets with massive scalability projected for larger datasets.

![Enhancement Two running on Windows](/images/enhancement-two.png)

[View Enhanced Code on GitHub](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/enhancement-two) | [View Original Artifact](https://github.com/sellavn/CS-499-Capstone-Project/tree/main/original-artifacts/CS-300) | [View Full Narrative]([https://github.com/sellavn/CS-499-Capstone-Project/blob/main/docs/Category%202%20Narrative%20Valles%20.docx])
