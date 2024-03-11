Goal: What principles we use while designing at Swiggy

## Tenets

- Excellence in design is achieved not when these is nothing to add, but when there is nothing left to take away.
- Don't design for something in the future but rather design for today. (Don't guess the future features and design for that)
- High bar for infrastructure security and data protection

## Concerns

- **Availability:** How to provide 99.99% availability. 
- **Elasticity:** How to scale more effectively given unexpected load? (Following the load curve)
- **Security:** How are we handling customer data?
- **Testability:** Do we have the right primitives for functional validation, mock dependency faults and stress/breakage points in our infrastructure?
- **Infrastructure Costs:** With rapid growth, how can we better optimize for infrastructure footprint? (Do More With Less)

## Best Practices: Build & Deployment

 - Gradual & Continuous Deployment (Shuttle Team takes care of CI/CD)
 - Configuration & Infra as code
 
## Best Practices: Runtime & Datastores

- **GoLang:** Most work is IO bound, low CPU utilization. Dynamic stack, lightweight thread context multiplexed on OS threads GoLang is well suited to handle high throughput,
- **GRPC:** Request Multiplexing, Strongly Typed, inbuilt backward compatibility
- **DynamoDB:** Simpler NoSQL key-value data model enables high availability and horizontal scalability due to data partitioning. 
- **Caching:** AWS ElasticCache for ephemeral caching along with a circuit breaker to ***fall back to an acceptable error*** in case of a cache failure.(If the Redis is down, we don't go to the service, rather we use another Redis instance)
- **Messaging:** For subscriber-consumer model, we recommend a managed *Confluent Kafka.* For point to point communication, we recommend AWS SQS.

## Enforcements vs Recommendations

### Enforced:
- DynamoDB as the storage (To use RDS, approval needs to taken and it's most probably not given)
- Shuttle for continuous deployments

### Recommended:
- Reasoning and detailed evaluations in Swiggy context

>Engineers are free to deviate from the recommendations but not from Enforced things. There is no requirement to get AOH review but if you want you can ask for review though taking the recommendations or not is individual choice there are no restrictions. Everyone is responsible for their code and is called OWNER of the code.