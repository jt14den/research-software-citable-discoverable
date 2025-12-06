---
title: "Making Software Citable with a DOI"
teaching: 10
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

* What is a DOI and why does it matter for software?
* How can you generate a DOI for your code on GitHub?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

* Explain the role of DOIs in software citation
* Archive a GitHub repository with Zenodo to generate a DOI

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

A Digital Object Identifier (DOI) provides a permanent, citable reference to a specific version of your software. Archiving your GitHub repository with Zenodo is a simple way to mint a DOI and increase the visibility and credibility of your code.

This also supports reproducibility: others can cite and use the exact version you used in your research.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

If participants don’t have a Zenodo account yet, have them watch or follow along. Mention that Zenodo is free and integrates directly with GitHub.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 1: Why Versioned DOIs?

Why is it important to generate DOIs for specific software versions?

:::::::::::::::::::::::: solution

Versioned DOIs let others cite the exact code version used in a study, ensuring reproducibility and avoiding ambiguity about features or bugs.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::: challenge
## Challenge 2: Create a DOI with Zenodo

Link your GitHub repository to Zenodo and archive your first release.

:::::::::::::::::::::::: solution

1. Sign in at [https://zenodo.org](https://zenodo.org) using GitHub
2. Authorize Zenodo to access your GitHub repositories
3. In GitHub, create a tagged release (e.g. v1.0.0)
4. Zenodo will archive the release and assign a DOI

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints

* DOIs make software citable in scholarly work
* Zenodo can generate DOIs for GitHub repositories
* Version-specific DOIs support reproducibility

::::::::::::::::::::::::::::::::::::::::::::::::
