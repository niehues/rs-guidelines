# SMP components and template

The template for writing an SMP is found [here](smp_template.md). 
The template includes best practices for each component, FAIR, and relevant resources.
However, not all software is equal, and hence not all components are relevant for every project.
Here, we provide a brief overview of the components and their relevance for different types of projects.

Typically, projects can be classified into three categories based on their management needs: 
high, medium, and low.

> For more information, see  [Practical guide to Software Management Plans by eScience Center (latest version)](doi:10.5281/zenodo.7038280)

## How to determine the complexity of a project

Ask yourself the following questions:

* **Purpose:** what is the reason or expected end-use for the software?
* **Reliability:** what is the effect of software failure and/or non-maintenance?
* **Maintenance:** what is the long-term effort needed to maintain the software?

Using the table below and your answers to the questions above, you can determine (or at least approximate) the complexity of your project.

| Criteria              	 | Low                                                                                     	 | Medium                                                                                                          	 | High                                                                                                                               	 |
|-------------------------|-------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| **Example Use Cases** 	 | Single-purpose scripts, automating routine tasks, analyzing a single dataset            	 | Research project output, libraries, or modules, implementing new algorithms                                     	 | Mission-critical software, controlling medical devices, preprocessing telescope data                                               	 |
| **Purpose**           	 | Limited to specific experiment or task; developer is the primary user.                  	 | Primary or secondary output of a research project; reusable as a library, tool, or module.                      	 | Critical function; absence or replacement would threaten research or operation.                                                    	 |
| **Reliability**       	 | Output can be visually inspected or tested with a limited set of inputs.                	 | More difficult to assess due to complexity; affects external research. Requires version control, documentation. 	 | Reliability is paramount; comprehensive architecture design, testing, auditing, and compliance with legal standards are essential. 	 |
| **Maintenance**       	 | Short-term; limited to the project duration, small influence beyond scope.              	 | Lifespan beyond the original project; requires long-term planning, archiving, and post-project maintenance.     	 | Long-term; maintained as long as in use. Requires funding, community support, and continuous maintenance.                          	 |
| **Considerations**    	 | Version control, documentation, versioning, and archiving recommended but not required. 	 | Code auditing, automated testing, software packaging, and distribution are essential.                           	 | Legal requirements (ISO/EC), build/release pipelines, traceability, right to use/distribute, cross-platform support.               	 |

## Relevant components for different levels

Based on the complexity of your project, you can have an indication on which components in the [template](smp_template.md) are relevant for your SMP.

| Category               	 | Component                                	 | Short description                                                                                                             	 | Low	 | Medium		 | High 	 |
|--------------------------|--------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|------|----------|--------|
| **Purpose**              | Purpose                                  	 | General info such as what problem does it solve, who is the intended audience, what are its advantages and limitations, etc.  	 | ✔️	  | ✔️		     | ✔️     |
| **Project management** 	 | Risk analysis                            	 | Factors that could have an impact on your software (privacy, security, reliability, etc.).                                    	 | 		   | 			      | ✔️   	 |
| \|                     	 | Repository                               	 | A (publicly) accessible repository, providing globally unique, persistent, and resolvable identifiers to each release.        	 | 		   | ✔️		     | ✔️   	 |
| \|                     	 | Software licensing and compatibility     	 | A licence specifying conditions of use for your software, including patenting information (if relevant).                      	 | ✔️	  | ✔️		     | ✔️   	 |
| \|                     	 | Maintenance                              	 | Arrangements in place for the maintenance and reuse of your software (+ retirement strategy).                                 	 | 		   | ✔️		     | ✔️   	 |
| \|                     	 | Support / Resources (during development) 	 | Resources for support-related activities such as training, hiring research software engineers, infrastructure, hardware, etc. 	 | 		   | 			      | ✔️   	 |
| L                      	 | Citation                                 	 | Info on how your software should be cited.                                                                                    	 | 		   | ✔️		     | ✔️   	 |
| **Engineering**        	 | Software Engineering quality             	 | Adherence to relevant code quality standards (styling, modularity, etc.).                                                     	 | 		   | ✔️		     | ✔️   	 |
| \|                     	 | Version control                          	 | Use of a version control system.                                                                                              	 | ✔️	  | ✔️		     | ✔️   	 |
| \|                     	 | Packaging                                	 | Package managers to allow users to install/deploy your software.                                                              	 | 		   | ✔️		     | ✔️   	 |
| L                      	 | Testing                                  	 | Tests and their documentation to ensure your software continues to work as intended.                                          	 | 		   | ✔️		     | ✔️   	 |
| **Documentation**      	 | User documentation                       	 | What the software does and how it should be used.                                                                             	 | ✔️	  | ✔️		     | ✔️   	 |
| \|                     	 | Deployment documentation                 	 | System requirements (e.g., dependencies) for deploying the software and instructions for installation and testing.            	 | ✔️	  | ✔️		     | ✔️   	 |
| L                      	 | Developer documentation                  	 | How the software can be modified (docstrings, in-line comments, etc.), tested, and contributed to.                            	 | 		   | ✔️		     | ✔️   	 |

