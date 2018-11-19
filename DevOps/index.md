# DevOps

## What is DevOps?

It is a set of working **practices** centred on development of code and delivery of that code to a live "production" environment. This can include traditional application development as well as infrastructure deployment automation ("Infrastructure As Code" or IAC), configuration management, etc.

It grew out of Agile software development movement as a **culture** of collaboration between Dev + Ops, as a means of resolving the often conflicting aims of software development and service operations:
  * Dev = **Speed** of feature releases, etc.
  * Ops = **Stability** of service

It is not:
* A standard
* A job title
* A set of tools

## KPIs

In DevOps teams, all share same goals, including speed of delivery & stability of service, with shared KPIs:

* Time to market (TTM)
* Few prod failures
* Immediate recovery from failure

## Tools

There are myriad tools available to support DevOps work. The following web page lists many of the commonly used ones:

* https://xebialabs.com/periodic-table-of-devops-tools

### Continuous Integration, Delivery & Deployment

#### Continuous (Build) Integration

* Automated build and testing
* Produces an artefact (package) that can be deployed

#### Continuous Delivery

Continuously maintaining code in a deployable state

#### Continuous Deployment

Frequently deploying small changes to production
The more often you deploy the better (usually)

#### Rollback

Easy to roll back to a known-good version
Problems can be patched and the new version re-deployed

#### Tools

* Tools used often based on programming language:

| Build Tool | Use |
| --: | :-- |
| [make](https://www.gnu.org/software/make/manual/make.html) | application compilation on linux |
| [maven](https://maven.apache.org/) | java |
| [npm](https://docs.npmjs.com/about-npm/) | javascript |
| [packer](https://www.packer.io/intro) | builds (virtual) machine images |
| Jenkins | Server-side CI builds |
| TravisCI | Server-side CI, esp. with GitHub |
| Bambooo | Server-side CI, esp. with Jira |


### Infrastructure As Code (IaC)

Automate the creation of (virtual) servers, containers, etc.

Configuration files held in source control and use automation to build the server/container/etc. using that configuration file.

### Configuration Management

maintaining and changing the state of pieces of infrastructure in a consistent, maintainable and stable way

Configuration Management complements & is enabled by Infrastructure-as-code techniques.

**Declarative** configuration:
  Configuration describes target configuration

**Procedural** configuration:
  Write scripts to configure target machines

#### Tools

| Tool | Model | Description |
| --: | :-: | :-- |
| Ansible | Agentless | Declarative configuration |
| Ansible Tower | Centralized | Declarative configuration |
| Chef | Server & Agent | Procedural configuration |
| Puppet | Server & Agent | Declarative configuration |
| Salt | Server & Agent | Event-driven automation | 

### Monitoring

* Infrastructure monitoring
  * CPU
  * Network
  * Memory
  * etc.
* Application monitoring
  * Web server response times
  * etc.

* Aggregation (data collection)
  * Elastic (ELK)
* Analytics

#### Tools

| Tool | Target | Description |
| --: | :-: | :-- |
| AppDynamics | Applications | Code-level diagnostics |
| Nagios | Infrastructure | |
| NewRelic | Infrastructure | |
| SenSu | Infrastructure | |

### Orchestration

Supports processes or workflows, e.g. provisioning

See [page on containerization](./Containers.md)

#### Tools

| Tool | Description |
| --: | :-: | :-- |
| Docker swarm | Infrastructure |
| Kubernetes | |
| ZooKeeper | |
| Terraform | |


### Microservices

 Isn't this really App Architecture rather than DevOps itself?
