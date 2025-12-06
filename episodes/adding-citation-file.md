---
title: "Adding a CITATION File"
teaching: 8
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

* What is a CITATION file and why is it important?
* How can you tell others how to cite your software directly on GitHub?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

* Describe the purpose of a CITATION.cff file
* Add and customize a CITATION.cff file to enable GitHub citation features

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

A `CITATION.cff` file provides citation metadata directly in your repository. When added to GitHub, it enables the "Cite this repository" button, making it easy for users to grab a properly formatted citation.

This file can include author names, ORCID IDs, version numbers, DOIs, and preferred citation formats.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Mention that the `.cff` file is readable and editable as plain text. If time allows, demo GitHub’s built-in citation UI once the file is present.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: challenge

## Challenge 1: What Should a Citation File Include?

What metadata should you include in a CITATION.cff file?

:::::::::::::::::::::::: solution

Include: title, authors (with ORCID), version, release date, DOI, and a preferred citation format or publication if relevant.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::: challenge

## Challenge 2: Add a CITATION.cff File

Create a `CITATION.cff` file in your GitHub repo with minimal metadata.

:::::::::::::::::::::::: solution

1. In the root of your repository, create a new file named `CITATION.cff`
2. Add content such as:

```yaml
authors:
  - family-names: Doe
    given-names: Jane
    orcid: https://orcid.org/0000-0002-1825-0097
title: MyResearchSoftware
version: 1.0.0
doi: 10.5281/zenodo.1234567
```

3. Commit the file and refresh the repo page to see "Cite this repository"

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: keypoints

* CITATION.cff files make citation info visible and usable
* GitHub displays citation options when this file is present
* Use ORCID, DOI, and version info to ensure accurate credit

::::::::::::::::::::::::::::::::::::::::::::::::
