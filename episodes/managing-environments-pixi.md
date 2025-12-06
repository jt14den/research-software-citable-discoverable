---
title: "Managing Reproducible Environments with pixi"
teaching: 12
exercises: 3
---

:::::::::::::::::::::::::::::::::::::: questions

* How can I make my software reproducible across machines?
* What is a simple way to manage Python and R environments for a project?
* How does using `pixi` improve the citable quality of my research software?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

* Explain why environment management is important for reproducible research.
* Create a minimal `pixi.toml` to define project dependencies.
* Use `pixi` to run code in a clean and isolated environment.
* Understand how environment files support citation, reuse, and FAIR software principles.

::::::::::::::::::::::::::::::::::::::::::::::::

## Why Environments Matter

Software often fails to run outside the original researcher's machine because of
differences in library versions, dependencies, or missing system requirements.
Environment management captures the “state” in which your software runs.

Defining an environment:

* helps others reproduce your results
* reduces troubleshooting time
* strengthens the reusability and citable quality of your software
* supports FAIR4RS principles

`pixi` provides an easy and fast way to manage environments for Python, R, and more.

---

## Installing pixi

Visit [https://pixi.sh](https://pixi.sh) for full installation instructions.

Common installation command for macOS/Linux:

```bash
curl -fsSL https://pixi.sh/install.sh | bash
```

Windows users can install via MSI installer or `winget`.

::::::::::::::::::::::::::::::::::::: callout

`pixi` ships its own toolchain.
Learners do not need Python, R, or compilers pre-installed on their system.

::::::::::::::::::::::::::::::::::::::::::::::::

## Creating a pixi Project

Create a new directory and initialize a pixi project:

```bash
mkdir myproject
cd myproject
pixi init
```

This command creates a `pixi.toml` file, which defines your environment.

Add Python and a package:

```bash
pixi add python
pixi add numpy
```

Add R and a package:

```bash
pixi add r
pixi add r-dplyr
```

Your `pixi.toml` now documents dependencies for anyone who wants to reproduce or build upon your software.

---

## Running Code with pixi

Run Python code inside the environment:

```bash
pixi run python script.py
```

Run R code inside the environment:

```bash
pixi run Rscript analysis.R
```

The environment is isolated, repeatable, and portable.

---

## How pixi Supports Citation and Reuse

Environments are part of the scholarly record.
A documented environment:

* ensures others can run the software described in a paper
* reduces replication failures
* provides metadata that complements a DOI and `CITATION.cff`
* strengthens compliance with FAIR4RS principles

When your software is deposited (e.g., Zenodo, Figshare), include:

* your `pixi.toml` file
* instructions for running code via `pixi run`

This helps future users reproduce results more reliably.

---

:::::::::::::::::::::::::::::::::::::: challenge

## Challenge: Add a dependency

Add `pandas` or `r-ggplot2` to your environment using `pixi`.
What changes do you observe in the `pixi.toml` file?

:::::::::::::::::::::::: solution

Run:

```bash
pixi add pandas
```

or:

```bash
pixi add r-ggplot2
```

The `[project.dependencies]` section of the `pixi.toml` file now includes the new package as an explicit dependency.

:::::::::::::::::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: keypoints

* Environments are essential for reproducible, citable research software.
* `pixi` provides fast, language-agnostic environment management for Python and R.
* The `pixi.toml` file documents dependencies that support FAIR4RS principles.
* Use `pixi run` to execute code inside a clean and reproducible environment.

::::::::::::::::::::::::::::::::::::::::::::::::
