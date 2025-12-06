---
title: "Choosing an Open-Source License"
teaching: 8
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

* Why do you need a license for your code?
* How can an open-source license increase reuse and citation?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

* Explain why unlicensed software is legally restricted
* Describe the main categories of open-source licenses
* Choose an appropriate license for a small research project
* Add a license file to a GitHub repository
* Identify resources for further help with licensing decisions

::::::::::::::::::::::::::::::::::::::::::::::::


## Why licensing matters

When researchers publish code without a license, most people assume it is “public.”
Legally, it is not. Copyright law applies automatically. Without a license:

* others cannot reuse, modify, or redistribute the code
* collaboration becomes uncertain and risky
* the sustainability of the project suffers

Clear licensing communicates permission and expectations.
This reduces friction and supports open, reproducible research.

::::::::::::::::::::::::::::::: callout

### Inclusive perspective

Licenses can feel intimidating. We assume no prior legal expertise.
Our focus is practical decision-making with widely used, well-supported licenses.

::::::::::::::::::::::::::::::::

## Understanding license categories

Open-source licenses fall into two broad groups.
We introduce only what learners need at this beginner stage.

### Permissive licenses

Examples: MIT, BSD, Apache-2.0

These allow broad reuse.
Anyone can copy, modify, or redistribute the code with minimal conditions.
They are common in research because they:

* are simple to understand
* maximize downstream flexibility
* integrate well with most tooling

### Copyleft licenses

Example: GPL-3.0

These require that derivative works also remain open.
This protects openness across the lifecycle of a project.

This is a value-driven choice.
Some researchers prefer ensuring openness.
Others prioritize flexibility and interoperability.

### SPDX identifiers

GitHub and most research software registries rely on short standardized identifiers
like `MIT`, `Apache-2.0`, or `GPL-3.0-or-later`.
We will use these throughout the lesson.


## How to choose a license for your project

Many research teams choose:

* **MIT** when they want broad reuse and minimal conditions
* **Apache-2.0** when they need explicit patent protection
* **GPL-3.0** when they want to ensure derivatives remain open

A simple decision rule for beginners:

* If you want others to reuse your code with few restrictions → choose MIT
* If you want openness to persist across reuse → choose GPL-3.0
* If you collaborate with industry, or prioritize explicit patent terms → choose Apache-2.0

:::::::::::::::::::::::::::::: callout

### You are not alone

Most institutions have librarians, research software engineers, or legal staff
who can help with complex cases. You do not need to know everything.

::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::: checklist 

## Adding a license file to your repository

### Step 1: Add a `LICENSE` file

You can create the file manually or through GitHub’s web interface.

**On GitHub:**

* Navigate to your repository
* Select **Add file → Create new file**
* Name it `LICENSE`
* Use **Choose a license template**
* Select MIT, Apache-2.0, or GPL-3.0
* Commit the file

GitHub will automatically tag your project with the chosen SPDX identifier.

### Step 2: Communicate your license in documentation

Add a short note to your README:

> This project is licensed under the MIT License. See `LICENSE` for details.

This improves discoverability and reduces ambiguity for users.

::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::: challenge

## Exercise: Compare permissive and copyleft licenses

Read these two short license descriptions provided in the lesson material.
In small groups or pairs:

* Identify what freedoms each license provides
* Identify one scenario where each license might be preferred

Share one observation with the group.

::::::::::::::::::::::::::::::::

## Summary

Licensing is foundational to making research software usable, citable, and shareable.
In this episode, you selected an appropriate open-source license and added it to a repository.
In the next episode, we will connect licensing with making software *citable* and *discoverable*,
continuing to build the scaffolding that supports open, sustainable research software.

::::::::::::::: keypoints

## Key Points

* Without a license, software is legally restricted and not reusable
* Open-source licenses communicate clear permissions and expectations
* Permissive licenses maximize flexibility
* Copyleft licenses preserve openness
* GitHub supports adding standardized license files through templates

:::::::::::::::

