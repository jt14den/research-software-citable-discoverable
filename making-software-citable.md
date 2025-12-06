---
title: "Making Your Software Citable"
teaching: 10
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

- What makes software citable?
- How do releases and DOIs strengthen software citation?
- How do I create a release and, optionally, mint a DOI?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Describe why software citation matters in research.
- Create a versioned release in GitHub.
- Understand when and why to mint a DOI with Zenodo.

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

Software is a research product.  
Like articles and datasets, it should be **cited** so others can acknowledge your work, find the exact version you used, and understand how your software contributed to their results.

Your software becomes **citable** as soon as it includes:

1. **Structured citation metadata**, such as a `CITATION.cff` file.  
2. **A public location where the code is available**.  
3. **A stable version** someone can reference.

A DOI is *optional* but valuable. It strengthens citability by giving each version a persistent identifier.

So far in this lesson, you have:

- shared a public repository  
- added a license  
- created reproducible environments with `pixi`  
- added a `CITATION.cff` file  

In this episode, you will create a **GitHub release** and learn how DOIs fit into software citation workflows.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Some learners may feel anxious about creating a DOI.  
Reassure them that:

- a DOI is not required for citability  
- Zenodo is free and widely used  
- they can watch the demo and complete the steps later

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

## What Makes Software Citable?

Software is citable when:

- it includes authorship and version information  
- the referenced version is stable  
- others can access the code  

A DOI **enhances** these qualities, but does not define them.

::::::::::::::::::::::::::::::::::::: callout

### Why add a DOI?

A DOI is helpful for:

- increasing visibility and discoverability  
- ensuring long-term persistence  
- citing *exact* versions  
- meeting journal and funder expectations  

But the core citability comes from your metadata and release process.

::::::::::::::::::::::::::::::::::::::::::::::::

## Create a Release in GitHub

A release captures a specific version of your software.  
It serves as the “snapshot” that others can cite.

### Steps

1. Open your GitHub repository.  
2. Select **Releases → Draft a new release**.  
3. Create a tag such as `v0.1.0`.  
4. Add release notes summarizing changes.  
5. Publish the release.

Your `CITATION.cff` file will automatically reference this tagged version unless you specify otherwise.

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 1: What belongs in a release?

Take one minute to reflect:

- What information would help a future you understand what changed in this version?

:::::::::::::::::::::::: solution

Useful release notes include:

- what changed  
- what was added or removed  
- what bugs were fixed  
- what might break for users  
- anything important about reproducibility  

Clear release notes help both people and tools interpret your software’s evolution.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::

## Minting a DOI with Zenodo (Optional but Recommended)

If you want a DOI for your release, GitHub and Zenodo integrate easily.

### Steps

1. Sign in at <https://zenodo.org> using your GitHub account.  
2. In Zenodo, enable archiving for your repository.  
3. Create or publish a GitHub release.  
4. Zenodo automatically archives the release and assigns a DOI.  
5. Use this DOI in your papers, documentation, and `CITATION.cff` file.

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 2: Why are versioned DOIs important?

Why might it matter that a DOI points to a *specific* release rather than the whole project?

:::::::::::::::::::::::: solution

Versioned DOIs:

- support reproducibility by identifying an exact snapshot  
- prevent confusion when the software changes  
- allow users to cite precisely the version they used  
- support FAIR4RS and publisher guidelines  

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints

- Software is citable as soon as it includes a citation file and a stable version.  
- GitHub releases create versioned snapshots for citation.  
- DOIs are optional but strengthen discoverability, persistence, and reproducibility.  
- Zenodo can automatically mint a DOI for each GitHub release.

::::::::::::::::::::::::::::::::::::::::::::::::

