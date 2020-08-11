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

### [Deploy Academy](https://deployacademy.pl/)

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
* Green Blue
* Canary Deployment 

## AWS Learning Library