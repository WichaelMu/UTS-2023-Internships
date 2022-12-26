# UTS 2023 Internships
Michael Wu

[GitHub](https://github.com/WichaelMu)

[LinkedIn](https://www.linkedin.com/in/michael-wu-3842b512b/)

## My understanding of Continuous Integration and Continuous Delivery.
Continuous Integration (CI) is a process used by a team of software developers to automate the process of testing and building a software product or service. The entire process, alongside Continuous Delivery and Deployment (CD), consists of several notable phases. Notably, the task or action that first commences the CI/CD workflow, the execution of automated unit tests after code compilation, and then delivery or deployment to live production. Development teams would maintain a single source repository on sites such as GitHub.

CI/CD significantly lowers the risk of releases with incremental pushes to the GitHub repository by ___Continuously Integrating___ with the production product, reduces the time and cost to publish and deploy a product with automated services provided by Azure's suite of cloud services, and increases and maintains high team morale with seamless development.

## What are some tools for this and why are they used?
### GitHub
A core tool for CI/CD is a version control service such as GitHub. Especially useful for teams of developers, it means multiple individuals can work on a software's source simultaneously and commit changes when ready. Version control means that developers can roll back to a previously known working state of a program or track the changes to your software. GitHub provides a wide range of services and connections to third parties, such as Azure DevOps.

### Azure DevOps
Azure DevOps is a broad and general tool used to manage a software product. Azure DevOps unifies and automates the development, testing, quality assurance, building, and deploying process with built-in services such as Pipelines, Environments, and Releases.

With a ` Service Connection ` on Azure DevOps, developers can link a GitHub repository to an Azure DevOps Project. Any commits to a specified branch will be intercepted and begin the CI/CD workflow with Azure Pipelines (assuming the Pipelines setup has been correctly initialised). Azure Pipelines would automatically compile and run any unit tests built into the source code. Should any compilation or testing failures be reported, Azure Pipelines will terminate the CI/CD process and not continue the remaining stages of deployment. In any other case, the Pipeline workflow will succeed, and Azure DevOps will automatically build, package, and deploy the software product, e.g., a Website, to a safe testing environment that clones the production environment with a service such as ` Azure Web App Services `.
### Azure Web App Services
Azure Web App Services is an HTTP service that manages and controls web applications such as Websites or APIs. It is a cloud computing solution that finalises the process of CI/CD as the source code from GitHub gets packaged and published to live and production web servers.

## Sources
My understanding of the philosophy of CI/CD, along with its practices and tools, was developed over 12 weeks at UTS' very own [Advanced Software Development (41026)](https://handbook.uts.edu.au/subjects/details/41026.html), where I was taught how to develop an e-commerce website using GitHub and its integration with Azure DevOps with live deployment to Azure Web App Services, receiving an overall grade of 94.

My understanding is attributed to [Dr. Bo Liu](https://profiles.uts.edu.au/Bo.Liu) for his lectures and workshops and his role as a Senior Lecturer and Subject Coordinator for Advanced Software Development at UTS.
