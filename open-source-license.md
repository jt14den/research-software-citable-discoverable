---
title: "Choosing an Open-Source License"
teaching: 8
exercises: 5
---

:::::::::::::::::::::::::::::::::::::: questions

* Why do you need a license for your code?
* How can an open-source license increase reuse and citation?
* What licenses does the UC system recommend?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

* Explain why unlicensed software is legally restricted
* Describe the main categories of open-source licenses
* Choose an appropriate license for a UC research project
* Add a license file to a GitHub repository
* Identify UC resources for licensing decisions

::::::::::::::::::::::::::::::::::::::::::::::::

## Why licensing matters

When researchers publish code without a license, most people assume it is "public."
Legally, it is not. Copyright law applies automatically. Without a license:

* others cannot reuse, modify, or redistribute the code
* collaboration becomes uncertain and risky
* the sustainability of the project suffers

Clear licensing communicates permission and expectations.
This reduces friction and supports open, reproducible research.

::::::::::::::::::::::::::::::: callout

### UC Context: Working with Tech Transfer

At UC, software created using university resources is typically owned by The Regents of the University of California. Before releasing code under an open-source license, check with your campus Tech Transfer office to:

* Verify ownership
* Ensure no third-party restrictions apply
* Select the appropriate license for your project

Each UC campus has specific processes - this lesson focuses on general best practices.

::::::::::::::::::::::::::::::::

## Understanding license categories

Open-source licenses fall into two broad groups.

### Permissive licenses

**Examples: BSD, MIT, Apache 2.0**

These allow broad reuse with minimal restrictions.
Anyone can copy, modify, or redistribute the code.
They are common in research because they're simple and maximize flexibility.

**The UC system recommends BSD licenses** as the first choice for most projects because they:

* originated at UC Berkeley
* are simple to understand
* protect both the institution and authors
* integrate well with most other licenses
* have minimal restrictions

### Copyleft licenses

**Example: GPL 2.0**

These require that derivative works also remain open-source.
This protects openness across the lifecycle of a project.

::::::::::::::::::::::::::::::: callout

### Note on GPL 3.0

The UC system does **not recommend GPL 3.0** for university-owned software due to patent provisions that may conflict with UC policies. If you need copyleft protection, consult your campus Tech Transfer office about GPL 2.0 or alternatives.

::::::::::::::::::::::::::::::::

## How to choose a license for your UC project

The UC Open Source Software Workgroup identified five "low-risk" licenses suitable for most projects:

**For most research software:**
* **BSD 3-Clause** → UC's primary recommendation (simple, protective, widely compatible)
* **MIT** → Very similar to BSD, slightly simpler (no non-endorsement clause)

**For specific needs:**
* **Apache 2.0** → Explicit patent protection (good for industry collaborations)
* **BSD 2-Clause** → Simplified BSD (removes non-endorsement clause)
* **ECL 2.0** → Educational focus (variant of Apache 2.0)

### Simple decision guide

1. **Default choice:** Start with **BSD 3-Clause**
   - Recommended by UC
   - Protects your institution
   - Simple and widely used

2. **Alternative:** Use **MIT** if you want the simplest possible license
   - Nearly identical to BSD
   - Slightly shorter text

3. **Special case:** Use **Apache 2.0** if working with industry partners
   - Explicit patent protection
   - Preferred by some companies

:::::::::::::::::::::::::::::: callout

### UC Resources

* [UC OSS Chart and Companion Guide](https://security.ucop.edu/resources/open-source-software-licensing.html) - Detailed license comparison
* [UC OSPO License Guide](https://ucospo.net/oss-resources/template-guides/license-guide/) - Templates and guidance
* Contact your campus Tech Transfer office for project-specific advice

::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::: challenge

## Challenge: Add a BSD License to Your Repository

Let's add the UC-recommended BSD 3-Clause license to your demo repository:

1. Navigate to your repository on GitHub
2. Click "Add file" → "Create new file"
3. Name it `LICENSE`
4. Click "Choose a license template"
5. Select **BSD 3-Clause License**
6. Update the copyright holder to "The Regents of the University of California" (if UC-owned)
7. Update the year to 2025
8. Commit the file

**Verify:** Refresh your repository page. Do you see "BSD-3-Clause license" displayed?

:::::::::::::::::::::::: solution

You should see "BSD-3-Clause license" in the repository sidebar. GitHub automatically detects and displays your license.

Your LICENSE file should start with:
```
BSD 3-Clause License

Copyright (c) 2025, The Regents of the University of California
All rights reserved.
```

If you don't see the license badge:
- Check the file is named exactly `LICENSE` (no extension)
- Verify it's in the root directory
- Confirm you committed the changes

:::::::::::::::::::::::::::::::::
::::::::::::::::::::::::::::::::

## Communicating your license

After adding a LICENSE file, reference it in your README so users immediately understand usage terms.

Add this section near the top of your README:
```markdown
## License

This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
```

**Why this matters:** Users reading your README on platforms other than GitHub (Zenodo, email, exported PDFs) will see your license terms even without GitHub's automatic detection.

::::::::::::::::::::::::::::: challenge

## Exercise: License Scenarios

Which license would you recommend for each UC research scenario?

**Scenario 1:** A Python package for ecological data analysis. You want maximum adoption across academia and industry.

**Scenario 2:** A data visualization tool developed with a biotech partner who may commercialize derivatives.

**Scenario 3:** A simple utility script you're sharing with collaborators.

:::::::::::::::::::::::: solution

**Scenario 1:** BSD 3-Clause (UC's default recommendation, maximum flexibility and adoption)

**Scenario 2:** Apache 2.0 (explicit patent protection important for industry partnerships)

**Scenario 3:** Either BSD 3-Clause or MIT (both work well for simple sharing; BSD preferred by UC)

In all cases, verify with your campus Tech Transfer office before releasing.

:::::::::::::::::::::::::::::::::
::::::::::::::::::::::::::::::::

## Summary

Licensing is foundational to making research software usable, citable, and shareable.
In this episode, you added a BSD license to a repository following UC recommendations.

::::::::::::::: keypoints

* Without a license, software is legally restricted and not reusable
* UC recommends BSD 3-Clause as the default license for most projects
* Permissive licenses (BSD, MIT, Apache 2.0) maximize flexibility and adoption
* Always consult your campus Tech Transfer office for UC-owned software
* GitHub makes adding standard licenses straightforward

:::::::::::::::
