---
title: "Sharing Research Software Effectively"
teaching: 10
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

- Why share research software in a public repository?
- What are the minimum elements that make a repository useful and discoverable?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Describe why public repositories increase visibility and credit for research software.
- Identify the essential components of a well-structured repository.
- Recognize the “before” state of the demo repository used throughout the lesson.

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

Publishing your research software in a public repository helps others find, understand, reuse, and cite your work. This visibility strengthens the transparency of your research process and increases the likelihood that you receive formal credit.

In this lesson, we start with a minimal example repository. As you move through the episodes, you will progressively improve it until it becomes citable, discoverable, and ready for reuse.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Use **progressive disclosure** by showing only the top-level structure of the demo repository first.  
If learners are new to GitHub, you may display two contrasting examples:  
- a sparse, hard-to-understand repo  
- a clear, well-documented repo  

This contrast reduces cognitive load and helps learners recognize what “good” looks like.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

## The Starting Point

Learners will download or clone the **“before” state** of the example repository:

```bash
software-demo/
├── README.md
├── src/
│ └── analysis.py
└── environment.toml #(pixi environment file)
```

This repository intentionally *lacks* many elements of good research software practice.  
By the end of the lesson, it will include licensing, citation metadata, improved discoverability information, and versioning.

::::::::::::::::::::::::::::::::::::: callout

### Why Make a Repository Public?

Public repositories help you:

- share methods transparently  
- get recognition for software contributions  
- collaborate more easily  
- comply with FAIR4RS recommendations  
- enable DOI assignment for citation  

::::::::::::::::::::::::::::::::::::::::::::::::

---

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 1: Explore What Makes a Repository Useful

Visit any public GitHub repository (your own or a well-known project).  
Identify:

- What information helps you understand or reuse the software?
- What appears to be missing?

:::::::::::::::::::::::: solution

Useful elements commonly include:

- README with context and usage  
- a clear file structure  
- license information  
- installation instructions  
- dependencies or environment files  
- contributors or authorship information  

Missing pieces often include absent documentation, unclear purpose, or no license.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::

---

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 2: Examine the Demo Repository

Open the **software-demo** repository you downloaded.

- What do you notice about its structure?
- What information is present?
- What information would you expect to see but is not yet included?

:::::::::::::::::::::::: solution

Learners may observe:

- README is minimal  
- No license  
- No citation file  
- No metadata to support discoverability  
- Environment file exists but is not yet introduced  

These gaps will be filled across subsequent episodes.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: keypoints

- Public repositories increase findability, reuse potential, and citation credit.  
- A well-structured repository lowers the barrier for others to understand your work.  
- The lesson begins with a minimal “before” repository that will be incrementally improved.

::::::::::::::::::::::::::::::::::::::::::::::::

