# DevOps

Culture of collaboration betweeb Dev + Ops
Set of Practices
Includes use of Tools

* Not a standard
* Not a job title

## History

* Grew out of Agile software development movement

## Culture / Goals

* Collaboration Dev + Ops
  * Dev = Speed of delivery, esp. features?
  * Ops = Stability of service
  * DevOps = Share same goals, inc. KPIs

## Concepts & Practices

### KPIs

* Time to market (TTM)
* Few prod failures
* Immediate recovery from failure

### Continuous Integration, Delivery & Deployment

#### Continuous Integration

Automated build and testing
Produces an artefact (package) that can be deployed

#### Continuous Delivery

Continuously maintaining code in a deployable state

#### Continuous Deployment

Frequently deploying small changes to production
The more often you deploy the better (usually)

#### Rollback

Easy to roll back to a known-good version
Problems can be patched and the new version re-deployed

### Infrastructure As Code (IaC)

Automate the creation of (virtual) servers, containers, etc.

Configuration files held in source control and use automation to build the server/container/etc. using that configuration file.

### Configuration Management

maintaining and changing the state of pieces of infrastructure in a consistent, maintainable and stable way

 Configuration Management complements & is enabled by Infrastructure-as-code techniques.

### Orchestration

### Monitoring

### Microservices

 Isn't this really App Architecture rather than DevOps itself?

## Tools
