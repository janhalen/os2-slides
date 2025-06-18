---
marp: true
theme: gaia
paginate: true
class: invert
---

# Dapr in Action – Episode 1  
### Infrastructure Abstraction for Distributed Systems

<!-- This is a presenter note for the introduction slide. Introduce Dapr as a runtime for distributed systems. Emphasize infrastructure abstraction, not microservices. -->

---

![bg](https://images.unsplash.com/photo-1517430816045-df4b7de1d1c0res)

- **Benefits for Distributed Systems**  
  - Simplifies infrastructure concerns  
  - Promotes portability and consistency  
  - Reduces boilerplate and vendor lock-in

- **Sidecar Architecture**  
  - Language-agnostic  
  - Runs alongside your app

- **Hosting Modes**  
  - Standalone  
  - Kubernetes  
  - Serverless

<!-- This is a presenter note for the key concepts slide. Overview of Dapr’s building blocks and architecture. Highlight benefits for teams managing distributed systems. -->

---
### Building Blocks

### State Stores
- Abstracts state management

### Pub/Sub
- Decouples producers and consumers

### Bindings
- Enables event-driven patterns and decoupling


### Observability
- Built-in metrics, tracing, and logging


<!-- This is a presenter note for the building blocks slide. Explain each block with examples. Emphasize flexibility and backend support. -->

---

![bg](https://images.unsplash.com/photo-1504384308090-c894fdcc538d)

- **Sidecar pattern**: Dapr runs next to your app  
- **Exposes APIs**: HTTP/gRPC endpoints for building blocks  
- **Simplifies**: No need to manage SDKs or client libraries

<!-- This is a presenter note for the sidecar architecture slide. Describe how Dapr runs alongside apps. Mention language independence and API exposure. -->

---

![bg](https://images.unsplash.com/photo-150438)


- Easy to install and run

### Kubernetes
- Production-ready
- Scales with your app

### Serverless
- Works with Azure Functions, AWS Lambda
- Ideal for event-driven workloads

<!-- This is a presenter note for the hosting modes slide. Compare standalone, Kubernetes, and serverless. Match modes to use cases. -->

---

![bg](https://images.unsplash.com/photo-1504384308090-c894fdcc538d)

qte, messaging, observability manually  
- **Portability**: Same APIs across cloud, on-prem, hybrid  
- **Consistency**: Standardized patterns and interfaces  
- **Reduced lock-in**: Swap components without changing code

<!-- This is a presenter note for the benefits slide. Focus on simplification, portability, and reduced vendor lock-in. -->

---

![bg](https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit)

Abstracts the complexity of distributed system infrastructure.  
It enables teams to build resilient, scalable applications without being tied to specific cloud services or architectural patterns.

<!-- This is a presenter note for the summary slide. Recap Dapr’s value proposition. Encourage experimentation and adoption. -->
