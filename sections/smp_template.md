# Template (+ best practices, FAIR, and relevant resources)

## Table of contents

1. [Purpose](#purpose)
2. [Project management](#project-management)
   1. [Risk analysis](#risk-analysis)
   2. [Repository](#repository)
   3. [Software licensing and compatibility](#software-licensing-and-compatibility)
   4. [Maintenance](#maintenance)
   5. [Support / Resources (during development)](#support--resources-during-development)
   6. [Citation](#citation)
3. [Engineering](#engineering)
   1. [Software Engineering quality](#software-engineering-quality)
   2. [Version control](#version-control)
   3. [Packaging](#packaging)
   4. [Testing](#testing)
4. [Documentation](#documentation)
   1. [User documentation](#user-documentation)
   2. [Deployment documentation](#deployment-documentation)
   3. [Developer documentation](#developer-documentation)

_____________________________________________________________________________________________________________________

## Purpose

> **What to write:**
>
> Provide general information such as: what problem does it solve, who is the intended audience, what are its advantages and limitations, etc..
> 
> Explain why developing new software is necessary. 
> New software should not be developed when it would be more cost-efficient and beneficial for the overall community to contribute to existing software.

_____________________________________________________________________________________________________________________

## Project management

### Risk analysis

> **What to write:** 
> 
> Describe the main external factors that should be considered by developers and users of the software.
> For example, compliance with privacy policies, security considerations, reliability requirements, portability / vendor lock, etc..

### Repository

> **What to write:** 
> 
> How will you make your software publicly available?
> 
> The most important consideration is that potential users of the software are able to get a copy they can use.
> If you do not plan to make it publicly available you should provide a justification.
> 
> How will you make your software findable? 
> Are you using a registry (that assigns a unique identifier to your software)?

> **Notes:**
> 
> Put all source files in a public version-controlled repository, preferably GitHub or GitLab.
> 
> To improve findability of the software, it should be shared in existing software registries. 
> Preferably, software is added to a registry specific to the domain and/or programming language. 
> Software can be shared in multiple registries if they are relevant to the software.

> **Resources:**
> 
> [Awesome list of software registries](https://github.com/NLeSC/awesome-research-software-registries)
> 
> [Archiving in Software Heritage](https://www.softwareheritage.org/howto-archive-and-reference-your-code/)

### Software licensing and compatibility

> **What to write:** 
> 
> What license will you give your software? 
> Preferably the licence should be as open as possible, and as closed as necessary.
> 
> Does your software respect the licences of libraries and dependencies it uses?
> How will you check that?
> Software licences must be compatible with the licence of external components (dependencies, libraries, etc.) that the software uses.

> **Notes:**
> 
> [What happens if you don't use a license](https://choosealicense.com/no-permission/)
> 
> Recommended license: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)

> **Resources:**
> 
> [Licensing & Compliance resources (Free Software Foundation guide)](https://www.fsf.org/licensing/)
> 
> [Licensing (The Turing Way guide)](https://the-turing-way.netlify.app/reproducible-research/licensing)
> 
> [Public License Selector (quiz)](http://ufal.github.io/public-license-selector/)
> 
> [ChooseALicense.com](https://choosealicense.com)
> 
> [Software Licenses in Plain English (tl;drLegal)](https://www.tldrlegal.com)
> 
> [Sharing software info (eScience)](https://esciencecenter-digital-skills.github.io/research-software-support/modules/licenses/how_to_share)

### Maintenance

> **What to write:** 
> 
> How do you plan to procure long term maintenance of your software?
> What level of support will be provided for users of the software and how will this support be organised?
> 
> Make sure there are arrangements in place for the maintenance and reuse of your software. 
> This could be through a community of developers who will continue to maintain it, 
> or by including the maintenance of software as part of future projects, 
> or by increasing the user base. 
> 
> Whenever suitable, develop a retirement strategy for your software.

### Support / Resources (during development)

> **What to write:** 
> 
> How do you plan to procure developement and long term maintenance of your software?
> 
> Plan resources for support-related activities such as training, hiring research software engineers, infrastructure, hardware, etc.. 
> The level of support should be in line with promises made regarding the level of service provided by your software (e.g., service level agreements).

### Citation

> **What to write:** 
> 
> How will users of your software be able to cite your software? 
> Please provide a link to your software citation file (CFF) if available.

> **Resources:**
> 
> [Software citation (The Turing Way guide)](https://the-turing-way.netlify.app/communication/citable/citable-cff.html#cm-citable-cff)
> 
> [Citation metadata generator (CFF INIT)](https://citation-file-format.github.io/cff-initializer-javascript/#/)

_____________________________________________________________________________________________________________________

## Engineering

> **NOTES:**

### Software Engineering quality

> **What to write:** 
> 
> Do you follow specific software quality guidelines?
> If yes, which ones?
> Does your code adhere to relevant code quality standards (styling, modularity, etc.)?

> **Resources:**
> 
> [OpenSSF Best Practices Badge Program](https://bestpractices.coreinfrastructure.org/en)
> 
> **Python-specific resources:**
> 
> [Python Code Quality: Tools & Best Practices](https://realpython.com/python-code-quality/)
> 
> [Stylized presentation: PEP 8 — the Style Guide for Python Code](https://pep8.org)
> 
> [PEP 8 – Style Guide for Python Code](https://peps.python.org/pep-0008/)

### Version control

> **What to write:** 
> 
> How will you manage versioning of your software?
> Adequate versioning of research software facilitates management of research software, allowing for the identification of specific versions of the software.

> **Notes:**
> 
> Ideally, use "semantic versioning" in the form MAJOR.MINOR.PATCH (e.g. v2.1.5).

> **Resources:**
> 
> [Best practices for version control (The Turing Way guide)](https://the-turing-way.netlify.app/reproducible-research/vcs.html)

### Packaging

> **What to write:** 
> 
> How will your software be packaged and distributed? 
> Do you use appropriate package managers to allow users to install/deploy your software with ease?
> Please provide a link to available packaging information (e.g., entry in a packaging registry, if available).

> **Resources:**
> 
> [Packaging (The Turing Way guide)](https://the-turing-way.netlify.app/reproducible-research/renv/renv-package.html)
> 
> [Python packages](https://py-pkgs.org)
> 
> [R packages](https://r-pkgs.org)

### Testing

> **What to write:** 
> 
> How will your software be tested? 
> Different types of testing (unit, functional, integration, linting, typing, regression, etc.) could be used. 
> Tests in turn should also be documented. 
> Coverage tools should also be used to assess the extent of the tested code.

> **Resources:**
> 
> [General guide for testing (The Turing Way guide)](https://the-turing-way.netlify.app/reproducible-research/testing/testing-guidance.html)

_____________________________________________________________________________________________________________________

## Documentation

> **Resources:**
> 
> [Documentation writing (eScience guide)](https://guide.esciencecenter.nl/#/best_practices/documentation)

### User documentation

> **What to write:** 
> 
> How will your software be documented for users?
> Please provide a link to the documentation if available.
> How will you document your software’s contribution guidelines and governance structure?

### Deployment documentation

> **What to write:** 
> 
> How will you document the installation requirements of your software? 
> Please provide a link to the installation documentation if available.
> 
> If applicable, please also include a complete and unambiguous description of dependencies to other software, datasets, and hardware.

### Developer documentation

> **What to write:** 
> 
> How will your software be documented for future developers?
> Explain how the software can be modified (docstrings, in-line comments, etc.), tested, and contributed to (governance, code of conduct, contributing guidelines, etc.).
