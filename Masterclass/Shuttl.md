# Introduction
Shuttle is a platform which will help you from taking your code from GitHub to production.

has many products -
- Apollo: finds anti-patterns
- CI: deployment build file, run tests, etc
- Ephemeral, QG(Quality Governance): Ephemeral means temporary. Swiggy has around 800 microservices. The Ephemeral environment let's you test the service with the rest of them in an isolated environment.
- Coast: CLI tool that will help perform operations on different types on environments.

## Ephemeral Environment
Ephemeral Environment is a personalized testing environment provisioning platform which is a simulation of production environment.

> Temporary & isolated environment. 

### Features 
- Isolation
- Temporary Nature
- Replicating Production Conditions
- Allows upstream and downstream testing
- time efficient testing

(integ.conf) is used for ephemeral

Canary - You only want few percent of users to use the service so it let's you do that