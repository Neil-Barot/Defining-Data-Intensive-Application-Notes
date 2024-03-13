# Chapter 1: Reliable, Scalable, and Maintainable Applications

## Key Terms:
- **Reliability**: The ability of a system to tolerate hardware and software faults. Accounts for any human error.
- **Scalability**: Measues the load and performance of a system. The ability of a system to deal with growth.
- **Maintainability**: The operability, simplicity, and evolvability of a system.
- **Fault**: A deviation or defect within a system that can lead to errors or failures in its operation

## Modern Systems are Data-Intensive  
- CPU power tends not to be a limitation for most computers causing them to be data-intensive as opposed to compute-intensive.
- Amount, complexity, and rate of change of data tend to be much larger issues
- Built from standard building blocks that provide commonly needed functionality including: databases, caches, search indexes, stream processing, and batch processing.
- Considerations must be made when using these building blocks as things such as different database types and cacheing algorithms might be more or less appropriate for a specific requirement.

## Thinking About Data Systems

Many modern applications have very demanding or wide ranging requirements, making it unfeasible for a single tool to efficiently meet the data processing and storage needs of the application. To resolve this issue, the various tasks are broken down such that they can be delegated to a tool that is suited to deal with it. These various tools are then stitched together using machine code.

When combining various tools in order to provide a service, the interface or API usually hides implementation details. You essentially used various general purpose tools in order to create one tool that is much more specific in its use.

There are many factors that may influence the design of a date system. Some of which include:
- Skills and experience of the people involved with it
- Legacy system dependancies
- Time scale for delivery
- Organization's Tolerance of different types of risl,
- Regulatory constraints

Three incredibly important concerns in most software systems include it's reliability, scalability, and maintainability.

## Reliability

Typical expectations of a reliable system:
- App performs as user expected
- Can tolerate user error or unexpected usage of software
- Under expected conditions, the performance is acceptable
- Prevents unauthorized access and abuse.

Assuming the above expectations are synonimous with "working correctly" a system that is reliable will "continue working correctly even when things go wrong."

Systems that can anticipate and cope with faults are considered to be fault tolerant or resilient. Faults aren't necessarily the same thing as a failure, as while a fault is a deviation from a system's spec, a failure stops the system from providing the required service to the user. Sincie it is impossible to completely prevent faults, it is best to design systems that prevent faults from causing failures.

There is a general preference for tolerating faults instead of preventing them, despite this there are cases where prevention is better than a cure. An example of this is for security matters.

## Hardware Faults

