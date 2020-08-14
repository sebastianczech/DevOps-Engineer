# DevOps-Engineer

Notes and links useful for DevOps Engineer

## Azure Microsoft Learn

### [Evolve your DevOps practices](https://docs.microsoft.com/pl-pl/learn/paths/evolve-your-devops-practices/)

* **Value stream map (VSM)** - helps you analyze your current release cycle process
* Customer value metrics - **Total lead time** is the time it takes for a feature to make it to the customer. **Process time**i s the time spent on a feature that has value to the customer. **The activity ratio** is process time divided by total lead time: ``ActivityRatio = ProcessTime/TotalLeadTime``
* [Azure DevOps services](https://azure.microsoft.com/en-us/services/devops)
    * Azure Boards
    * Azure Pipelines
    * Azure Test Plans
    * Azure Repos
    * Azure Artifacts
* [What features and services do I get with Azure DevOps?](https://docs.microsoft.com/en-us/azure/devops/user-guide/services?view=azure-devops&viewFallbackFrom=azure-devops%3Fazure-portal%3Dtrue)    
* [DevOps Resource Center](https://docs.microsoft.com/en-us/azure/devops/learn/)
* Elite performers:
    * Deploy more frequently
    * Reduce lead time from commit to deploy
    * Reduce change failure rate
    * Recover from incidents more quickly
* [DevOps](https://docs.microsoft.com/en-us/azure/devops/learn/what-is-devops) - The union of people, process, and products to enable continuous delivery of value to our customers
* [DevOps at Microsoft](https://docs.microsoft.com/en-us/azure/devops/learn/devops-at-microsoft/)
* Key Performance Indicators (KPIs) and quality metrics:
    * Faster Outcomes
        * Deployment Frequency
        * Deployment Speed
        * Deployment Size
        * Lead Time
    * Efficiency
        * Server to Admin Ratio
        * Staff Member to Customers Ratio
        * Application Usage
        * Application Performance
    * Quality and Security
        * Deployment Failure Rates
        * Application Failure Rates
        * Mean Time to Recover
        * Bug Report Rates
        * Test Pass Rates
        * Defect Escape Rate
        * Availability
        * SLA Achievement
        * Mean Time to Detection
    * Culture
        * Employee Morale
        * Retention Rates
* Common quality metrics
    * Failed Builds Percentage 
    * Failed Deployments Percentage 
    * Ticket Volume 
    * Bug Bounce Percentage 
    * Unplanned Work Percentage 
* Azure Boards is a tool in Azure DevOps to help teams plan the work that needs to be done. 
* Agile Manifesto states - responding to change comes before following a plan
* A sprint is a fixed amount of time a team has to complete a set of tasks
* Delivery Plans is an extension for Azure DevOps that helps organizations plan and review work schedules across multiple teams. It's a visualization of one or more work schedules against a calendar backdrop.
* Creating a delivery plan can be valuable at any point in a project.

### [Build applications with Azure DevOps learning path](https://docs.microsoft.com/en-us/learn/paths/build-applications-with-azure-devops/)

* **Azure Pipelines** is a cloud service that you can use to automatically build, test, and deploy your code project.
* Continuous integration (CI) is the process of automating the build and testing of code every time a team member commits changes to version control. 
* A pipeline defines the continuous integration process for the app. It's made up of steps called tasks. The pipeline runs when you submit code changes.
* A build agent builds or deploys the code. When your build or deployment runs, the system begins one or more jobs. An agent is installable software that runs one build or deployment job at a time. 
* The final product of the pipeline is a build artifact.
* Instead of managing each agent individually, you can organize agents into agent pools. An agent pool defines the sharing boundary for all agents in that pool. 
* Service endpoints are a way for Azure DevOps to connect to external systems or services. They are a bundle of securely stored properties that includes but is not limited to:
  * Service name
  * Description
  * Server URL
  * Certificates or tokens
  * User names and passwords
* Pipeline as code refers to the concept of expressing your build definitions as code. 
* A template enables you to define common build tasks one time and reuse those tasks multiple times. You call a template from the parent pipeline as a build step. You can pass parameters into a template from the parent pipeline.
*  Version control system:
   * centralized (e.g. Team Foundation Version Control (TFVC))
   * distributed (e.g. GIT)
* Clone is your local copy of a repository
* Branching - where you can maintain as many copies as you want and merge back only the one you want to keep. Main branch, or trunk, is typically called master
* When your code is ready to be merged into the master branch in the main repository that's shared by all developers, you create what's called a pull request. When you create a pull request, you're telling the other developers that you have code ready to review and you want it merged into the master branch. When your pull request is approved, it becomes part of the master codebase.
* Git commands:
  * Create a Git repository:	``git init``
  * Download a remote repository:	``git clone``
  * Create a branch:	``git checkout``
  * See which files have been changed:	``git status``
  * Stage files to commit:	``git add``
  * Commit files to your branch:	``git commit``
  * Download a branch from a remote repository:	``git pull``
  * Upload a branch to a remote repository:	``git push``
* Origin specifies your repository on GitHub. When you fork code from another repository, it's common to name the original remote (the one you forked from) as upstream.
* By default, a build is triggered when a change is pushed to any file on any branch.
* A continuous integration (CI) build is a build that runs when you push a change to a branch.
* A pull request (PR) build is a build that runs when you open a pull request or when you push additional changes to an existing pull request.
* PR builds help you verify that your proposed changes will work correctly after they're merged to master or another target branch. The final CI build verifies that the changes are still good after the PR was merged.
* Badge - it's important for members of the team to know the status of the build. An easy way to quickly determine the build status is to add a build badge to the README.md file on GitHub. A badge is part of Microsoft Azure Pipelines. It has methods you can use to add an SVG image that shows the status of the build on your GitHub repository. Most GitHub repositories include a file named README.md, which is a Markdown file that includes essential details and documentation about your project. GitHub renders this file on your project's home page.
* Dashboard is a customizable area in Azure DevOps where you can add widgets and extensions to help you visualize areas of your DevOps solution. 
* [Git](https://git-scm.com/)
* [GitHub Desktop](https://desktop.github.com/)
* [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
* [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
* [How to Split Pull Requests – Good Practices, Methods and Git Strategies](https://www.thedroidsonroids.com/blog/splitting-pull-request)
* [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
* [Specify events that trigger pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/build/triggers?view=azure-devops&tabs=yaml)
* Branch strategies:
  * Feature Branch Workflow
  * Gitflow Workflow
  * Forking Branch Workflow
* Branch policies help you to protect your important Git branches. Policies enforce your team's code quality and change management standards. Some examples of the policies you can configure include: the minimum number of reviewers, checking for linked work items, checking for comment resolution, enforcing a merge strategy, and checking for build validation.
* Pull request strategies - add additional conditions to your pull requests to enforce a higher level of code quality in your key branches. A clean build of the merged code and approval from multiple reviewers are some extra requirements you can set to protect your key branches
* ...

## [Beautiful Builds and Continuous Delivery Patterns](https://courses.osherove.com/courses/2796/lectures/54700)

* [Beautiful Builds - Roy Osherove](https://vimeo.com/94193986)
* [Kim van Wilgen - Continuously delivering continuous delivery](https://vimeo.com/240521820)
* Automatic build != Continuous integration
  * what to do vs. when to do it
  * build scripts vs. CI server
  * build scripts: Maven, Rake, Ant
  * CI server: Jenkins, TeamCity, Circle CI, Travis CI
  * build scripts: knowledge about source structure (development)
  * CI server: knowledge about environment (operations)
  * application code vs. ops configurations
  * build scripts: versioned in source control
  * CI server: versioned seperately
* CI server + build scripts = not a good idea
* Coupling *Application Source Structure* to *Operations Knowledge* forces you to change *operational configurations* on simple applicative source changes (e.g. chaning name of folder, which is containting tests)
* Coupling *Operations Knowledge* to *Application Source Control* forces you to change *application source* and check in on simple operational changes (e.g. changing IP address of FTP server to store built app - in this case in script use environment variable and on CI server set value for this environment variable) 
* Continuous delivery - why ?
  * how long before you:
    * compile ?
      * continuously
    * test ?
      * continuously
    * deploy ?
      * continuously
* ...

## [Deploy Academy](https://deployacademy.pl/)

* Maturity Model CD
* Build pipeline:
  * Build backend 
  * Test backend + Code Coverage
  * Build frontend
  * Test frontend 
  * Code coverage front
* Badge
* Relese pipeline
* Deployment bazy danych
* Parametry konfiguracyjne i hasła
* Repo:
  * Git flow
  * Trunk Based Development
  * Master only
  * Duże zmiany
  * Pull requesty
* Feature Switch
* Infractacture as a code
* Piramida testów
* Build script, deploy script
* Agenty i rozbicie pipelinów
* Artefakty
* Cache
* TIP
* Continuous Deployment
* Downtime
* Rollback
* [Green Blue](https://martinfowler.com/bliki/BlueGreenDeployment.html)
* [Canary Deployment](https://octopus.com/docs/deployment-patterns/canary-deployments)
* [Jerzy Wickowski - CI/CD Co to? Po co? Jak?](https://jerzywickowski.pl/prelekcje/cicd-co-to-po-co-jak/)

## AWS Learning Library

* ...

## Other materials

* [The Roadmap to Becoming a DevOps Professional — From Server to Serverless](https://jobsfordevops.com/blog/how-to-become-a-devops-engineer/)
* [How to screen the most important DevOps skills](https://devskiller.com/screen-important-devops-skills/)
* [What are the best resources for learning about DevOps?](https://www.quora.com/What-are-the-best-resources-for-learning-about-DevOps)
* [DevOps Tutorial: Complete Beginners Training](https://www.guru99.com/devops-tutorial.html)
* [Training materials for DevOps](https://gist.github.com/ssmythe/ae1449b116ece85dc10d)
* [DevOps Tutorial: The Ultimate Guide To DevOps (25+ Tutorials)](https://www.softwaretestinghelp.com/devops-tutorials/)
* [CNCF Cloud Native Interactive Landscape](https://landscape.cncf.io/)
* [An Illustrated Guide to OAuth and OpenID Connect](https://developer.okta.com/blog/2019/10/21/illustrated-guide-to-oauth-and-oidc)
* [Distroless Docker Images](https://github.com/GoogleContainerTools/distroless)
* [What Web Can Do Today](https://whatwebcando.today/)
* [Pact - contract testing](https://docs.pact.io/feature_support)
* [JVM bloggers](http://jvm-bloggers.com/)
* [Presto - distributed SQL query engine for Big Data](http://prestodb.github.io/)
* [Datadog - integrations](https://docs.datadoghq.com/integrations/postgres/)
* [Open Platform for NFV (OPNFV) - Deploy your own Xtesting CI/CD toolchains](https://wiki.opnfv.org/pages/viewpage.action?pageId=32015004)
* [Knative - Kubernetes-based platform to build, deploy, and manage modern serverless workloads](https://cloud.google.com/knative)
* [DevSpace - Deploy & Develop Kubernetes Apps](https://devspace.sh/)
* [Garden - garden automates the repetitive parts of your workflow to make developing for Kubernetes and cloud faster and easier](https://garden.io/)
* [Jepsen databases analyses](https://jepsen.io/analyses)
* [JFHCI - just f-ing hard code it](http://udidahan.com/2012/02/26/common-cqrs-abuses/)
* [Google Best Practices for Java Libraries](https://jlbp.dev/)
* [Cisco DevNet: APIs, SDKs, Sandbox, and Community for Cisco Developers - Cisco DevNet](https://developer.cisco.com/)
* [Cisco DevNet: Learning Labs](https://learninglabs.cisco.com/)
* [Course: NetDevOps and network programmability basics](https://developer.cisco.com/video/net-prog-basics/)
* [Source code: Network Programmability Basics](https://github.com/CiscoDevNet/netprog_basics)
* [VxLAN – przyczyny powstania i zasada działania](https://www.nastykusieci.pl/podstawy-vxlan-1/)
* [Understanding VXLANs](https://www.juniper.net/documentation/en_US/junos/topics/topic-map/sdn-vxlan.html)
* [VxLAN Overview](https://networkdirection.net/articles/routingandswitching/vxlanoverview/)
* [Hands-on with NetDevOps](https://github.com/juliogomez/netdevops)
* [Catalog of refactorings](https://refactoring.com/catalog/)
* [Trunk based development](https://trunkbaseddevelopment.com/)
* [The Complete CI/CD Collection](https://dzone.com/articles/the-complete-cicd-collection-tutorials)
* [Beautiful Builds by Roy Osherove](https://www.slideshare.net/royosherove/beautiful-builds-by-roy-osherove)  
* [Pipeline Driven Organization](https://pipelinedriven.org/)
* [TIP - together we build](https://telecominfraproject.com/together-we-build-growing-new-ecosystems-and-accelerating-deployments/)
* [Badges](https://docs.gitlab.com/ee/user/project/badges.html)
* [Octopus Deploy - repeatable, reliable deployments](https://octopus.com/)
* [CI/CD Patterns](https://continuousdelivery.com/implementing/patterns/)
* [Periodic Tableof DevOps Tools](https://digital.ai/periodic-table-of-devops-tools)
* [DevOps Roadmap](https://roadmap.sh/devops)