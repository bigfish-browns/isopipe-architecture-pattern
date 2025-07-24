# IsoPipe Architecture Pattern

**Purpose:**  
To isolate read and write pipelines within a single microservice so that read operations are always healthy and unaffected by write failures.

## Key Features
- Runtime isolation between read and write flows
- Separate thread pools and circuit breakers
- API Gateway segregation
- Health check decoupling

## Use Case
Telecom microservices requiring continuous availability of read APIs like SIM Status, MNP, Plan Lookup while write services like Activate SIM may face DB or downstream failure.

## Inspired by
- Circuit Breaker
- Bulkhead
- CQRS

## License
Apache 2.0
