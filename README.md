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
* Automated tests - documentation and the ability to more easily refactor your code are two added benefits of automated testing.
* Test pyramid
* Continuous testing means tests are run early in the development process and as every change moves through the pipeline. 
* Shifting left means considering software quality and testing earlier in the development process.
* What makes a good test?
  * Don't test for the sake of testing
  * Keep your tests short
  * Ensure that your tests are repeatable
  * Keep your tests focused
  * Choose the right granularity
* Security and license ratings in open-source software:
  * [Black Duck](https://www.blackducksoftware.com/) - Black Duck  by Synopsys scans your open-source dependencies against their own database. They keep that database up-to-date with the latest vulnerabilities and give you timely information on fixes, workarounds, and on the exploits. They cover over 80 programming languages, and get their information from many sources.
  * [GitLab](https://about.gitlab.com/) - GitLab  is a CI/CD pipeline tool that enables you to scan the dependencies in code that comes from GitLab repositories. It supports JavaScript, Ruby, Python, PHP, and Java. Their Azure Pipelines extension  enables you to add a GitLab repository as a source.
  * [Sonatype Nexus](https://www.sonatype.com/nexus-repository-sonatype) - Sonatype Nexus  scans your dependencies for known vulnerabilities, licenses, and old or unsupported components. Their Azure Pipelines extension  enables you to upload your artifacts to Sonatype Nexus for scanning.
  * [Veracode](https://www.veracode.com/) - Veracode  is a code scanning tool that integrates with Azure Pipelines to help you find vulnerabilities early in the development process. Their Azure Pipelines extension  stops the build process if there's a severe security risk and gives you guidance on finding and fixing the vulnerability.
  * [WhiteSource Bolt](https://bolt.whitesourcesoftware.com/) - WhiteSource Bolt  is a tool for scanning open-source dependencies for vulnerabilities and licensing. It supports more than 200 programming languages and gives guidance on fixing the vulnerabilities. There are reports for vulnerabilities, licensing, and inventory. Their Azure Pipelines extension  allows for extensive policy configuration as well as viewing the results from the Azure Pipelines portal.
* [What is a public project?](https://docs.microsoft.com/en-us/azure/devops/organizations/public/about-public-projects?view=azure-devops)
* [Quickstart: Change the project visibility, public or private](https://docs.microsoft.com/en-us/azure/devops/organizations/public/make-project-public?view=azure-devops)
* [Setting repository visibility](https://help.github.com/github/administering-a-repository/setting-repository-visibility)
* [Pipeline - specify conditions](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/conditions?view=azure-devops&tabs=yaml)
* [Security Content Automation Protocol - SCAP](https://csrc.nist.gov/projects/security-content-automation-protocol)
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
* Pattern - *shipping skeleton*:
  * created on *walking skeleton* - tiny implementation of the system that performs a small end-to-end function. It should link together the main architectural components. Architecture and functionality can then evolve in parallel.
  * shipping skeleton is a combination of 2 elements:
    * a skeleton of application
    * a shipping system for the skeleton
  * tactic - start a project by creating a fully automated build and production deploy path for the simplest piece of code you can
  * machines:
    * build machine
    * test machine
    * staging machine
    * production machine
  * build configurations:
    * continuous integration build
    * slow build
    * deploy to test servers
    * deploy to staging servers
    * deploy to production
* Triggers and Waves of confidence:  
  * Build configurations - back to coding quickly:
    * 10 CI
    * 20 integration test
    * 30 deploy to test with smoke test
    * 40 deploy to staging with acceptance test
  * Build chain triggers:
    * after CI start deploy to test
    * after deploy to test start deploy to staging
    * after deploy to staging start deploy to production
  * triggering
    * time
    * build finished
    * check in
    * API request
    * retry 
* Slow builds:
  * in many pipelines we are repeating the same things (checkout, compile, unit tests, deploy)
  * if we build something, the use artifacts repository to not build it one more time
  * pattern: cumulative, fast builds - artifact dependencies
  * don't repeat yourself, build it once and store in articacts repository
* Solving versioning with Snapshot Dependencies
  * component depends from other components
    * artifacts are uploaded to repository if the build is successful
    * versioning issues
    * if build 1.0.1 is ok, but 1.0.2 is failed, we cannot use latest version of component
    * solution - snapshot dependencies
      * do not use specific version
      * use tag e.g. latest (for this one which was last successful built)
  * workinh snapshots are skipped
    * no time wasting repeating ourselves
    * build when needed (code check in)
* Many components developed by seperated teams:
  * own CI, Unit Test and Integration Test
  * where do we get the artifacts from, for each component ? 
    * convention is very important
    * pattern: tipping point (publishable binaries) 
* Speeding Up Inter Team Dependencies: API Artifacts
  * contracts for other modules
* Imaginvative world:
  * test env. -> stating env. -> production env.
* Real world
  * test env. -> stating env.  |  production env.
    * use Isolated Deploy Machine (e.g. FTP / shared folder), from which there is scheduled deploy from folder (some kind of proxy)
* Parallel Firehose
  * besides test, stage and production env., there is dev-test and dev-staging env.
  * automated sync on requests / schedule between e.g. dev-test env. and test env.
* Branching strategies:
  * Continous Delivery Strategy:
    * get feedback as quickly as possible
      * get rid of humans in the loop, automate as much as possible
    * as close to customer as possible (production / staging)
      * try to deploy to production as much as possible
  * Feedback levels:
    * compiler
    * test
    * environmental (permissions, performance, ...) - staging and prod
    * customer (user)
  * Common branching reasons:
    * promote (move code to more important environment)
    * create new release
    * create a new feature safely
    * create a new isolated component of the system
    * run on a different platform
  * Strategy 1 - branch per environment (promotions)
    * branches:
      * WIP (working in progress) branch (test env.)
      * MAIN branch (staing env.)
      * PROD branch (staging + production env.)
    * lots of human work (merging)
    * feedback not so fast (only from test env.)
  * Strategy 2 - single trunk (no branches, no merging)
    * only WIP or MAIN branch
    * on release:
      * release branch ?
      * tag ?
    * continouse deployment without release branches:
      * no parallel fire hose (test, stage and prod. env.)
      * with parallel fire hose ( + dev test, + dev stage)
  * Strategy 3 - release branches (dev overlap problem)
    * in the moment of release new branch is created
    * it's good with paraller fire hose, whene release branches are deployed to test, stage, prod and main branch is deployed on dev test, dev stage
  * Strategy 4 - single branch with [feature flags](https://www.martinfowler.com/articles/feature-toggles.html)
    * feature flags are created while starting working on feature. it's removed after it's deployed on production.
    * feature flags are temporary.
    * common uses:
      * hide partial feature from showing in production (dev)
        * enable continous delivery without branching
      * enable feature for certain class of customer or on some kind of environment (business)
    * [feature toggle frameworks list](https://pipelinedriven.org/feature-toggle-frameworks-list)
    * practices:
      * remove flag as soon as possible
      * no nested flags
      * use flags at entry points (single point of contact)
        * usually in UI
      * favor polymorphism (strategy pattern) over condolidations
        * to make code more maintainable
* TeamCity
* CI/CD:
  * component 1,2,3,...,N:
    * 05 - public API
    * 10 - CI
    * 20 - unit test
    * 30 - integration test
    * 40 - TIP
  * deploy chain:
    * 10 - system integration
    * 20 - deploy to test
    * 30 - deploy to staging
    * 40 - deploy to production

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

* Best practices of Running Web application in Cloud:
  * Tools:
    * EC2 (server)
    * Elastic Beanstalk (PaaS)
    * EKS (Kubernetes)
    * ECS (Containers)
    * S3 (Static Site)
    * Amplify (PaaS for Static Pages)
  * Elastic Beanstalk:
    * runs on EC2 host
    * manages:
      * OS
      * language interpreter
      * application server
      * HTTP server
  * Amplify:
    * idea:
      * develop
      * test
      * deploy/host
      * measure
  * Security - network is important - VPC (virtual private cloud):
    * do not put all components (web server, app server, db server) in public network
    * app and db in private network, web server in public network with security group
    * the best solution - load balancer in public, the rest (web, app, db) in private network
    * use jump host to connect to db or app server or the best to use system manager
  * Scalability is important:
    * Auto Scalling is available in many services
  * Speed:
    * Global Accelerator
      * from nearest POP packets are send in private AWS network
    * CDN (content delivery network)
      * CloudFront
  * Threats:
    * examples:
      * DDOS (distributed denial of service)
      * bad bots
      * app vulnerabilities
    * tools:
      * Shield Standard (default enabled)
      * Shield Advanced
      * WAF (web app firewall)
  * AI & MI - examples of services:
    * Polly (to read something)
    * Translate
    * Fraud Detector
    * Personalize
  * Databases:
    * RDS (relational database systems)
    * Key-value
    * Document
    * Graph
    * In-memory
    * Time-series
    * Ledger
  * Microservices
    * each microservices should have his own database, but it will costs too much for RDS
    * DynamoDB is free or cost not too much
  * Cache
    * ElasticCache (Redis, memcache)
  * Continous integration / delivery / deployment
    * CodePipeline
  * Marketing
    * Pinpoint (SMS, mail, voice)
* AWS Kubernetes:
  * Control Plane (Kubernetes master nodes), Data Plane (worker nodes, minions)
  * Options:
    * DIY (do it yourself) - Kops, Kubeadm (hard way)
    * Manager Service - [EKS (Elastic Kubernetes Service)](https://aws.amazon.com/eks/)
      * Worker nodes:
        * Servers on EC2
        * Managed Groups on EC2
        * [Fargate (serverless)](https://aws.amazon.com/fargate/)
  * [eksctl](https://eksctl.io/) - official CLI for Amazon EKS
  * [CDK for Kubernetes](https://cdk8s.io/) - define Kubernetes apps and components using familiar languages
  * [Visual Studio Code from command line](https://code.visualstudio.com/docs/setup/mac)
  * K8s basics:
    * Pod, deployment, service, load-balancer, namespace
    * Ingress - more advanced load balancer
    * Scaling:
      * [HPA - Horizontal Pod Autoscaler](https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/)
      * [Cluster Autoscaler](https://github.com/kubernetes/autoscaler/tree/master/cluster-autoscaler)
      * [VPA - Vertical Pod Autoscaler](https://cloud.google.com/kubernetes-engine/docs/concepts/verticalpodautoscaler)
  * [AWS Cloud Map](https://aws.amazon.com/cloud-map/) - service discovery for cloud resources. Registry contains:
    * namespace
    * service
    * service instance
  * Server-side service discovery patterns:
    * connections are proxied
    * discovery is abstracted way
    * availability and capacity impact
    * additional latency
  * Client-side service discovery patterns:
    * clients connect directly to providers
    * fewer components in the system
    * clients must be registry-aware
    * client-side load balancing
  * Service registers:
    * etcd
    * zookeeper
    * eureka
    * doozerd
    * skydns
  * [Kubernetes ExternalDNS](https://github.com/kubernetes-sigs/external-dns)
  * [AWS App Mesh](https://aws.amazon.com/app-mesh/) - application-level networking for all your services - uses [Envoy](https://www.envoyproxy.io/)
  * Service mesh options:
    * in-process code (sdk) (monitoring, routing, discovery, deployment)
    * out-of-process (sidecar proxy) (pod = miscroservice as container + proxy as container)
    * [sidecar proxy vs. libraries or app code](https://dzone.com/articles/comparing-service-mesh-architectures)
  * Observability:
    * AWS CloudWatch
    * AWS X-Ray
    * [Prometheus](https://prometheus.io/)
    * [Datadog](https://www.datadoghq.com/)
  * Client-side traffic management:
    * traffic shaping
      * service discovery
      * retries 
      * timeouts
      * circuit breakers
      * health checks
    * routing controls
      * protocols support
      * header based
      * cookie based
      * path based
      * host based
  * [Amazon EKS Workshop](https://www.eksworkshop.com/)
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
* [Oh Shit, Git!?!](https://ohshitgit.com/)