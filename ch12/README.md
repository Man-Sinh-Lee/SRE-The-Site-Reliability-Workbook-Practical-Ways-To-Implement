### Chapter 12 Summary: Introducing Non-Abstract Large System Design (NALSD)

Chapter 12 of *The Site Reliability Workbook* introduces Non-Abstract Large System Design (NALSD), a practical, iterative approach to system design that Google’s SREs use to align reliability with operational costs and scalability.

---

#### What Is NALSD?
NALSD is a process that involves iterating on system designs to create practical, resilient, and scalable solutions. It encompasses skills such as capacity planning, component isolation, and system degradation. The iterative approach allows SREs to refine designs gradually, building systems that can manage real-world constraints like network and data center limitations.

#### Why “Non-Abstract”?
The “Non-Abstract” in NALSD emphasizes grounding designs in practical constraints. While whiteboard designs often ignore physical limits, NALSD advocates converting theoretical designs into concrete plans that specify actual resources, like CPU or RAM, to ensure systems can operate effectively in production environments. This approach reduces last-minute adjustments due to overlooked physical or logistical limits.

#### AdWords Example: Iterative Design Process
The chapter illustrates NALSD through an example of Google AdWords, focusing on calculating the click-through rate (CTR) of ads. The design evolves through several stages, reflecting real-world scalability and reliability considerations:

1. **Initial Requirements**  
   The AdWords system needs to display an advertiser’s dashboard quickly and provide recent CTR data. The system should handle 500,000 search queries per second and 10,000 ad clicks per second while meeting SLOs of <1-second response time and <5-minute data freshness.

2. **One Machine**  
   The initial design considers using a single machine with a simple SQL database. However, this approach is infeasible due to I/O and memory limits. For example, storing 100 TB of daily log data would require impractically high disk throughput and RAM, leading to multiple single points of failure.

3. **Distributed System**  
   Moving to a distributed design, Google implemented components like **MapReduce** for data processing and **LogJoiner** for data integration. Each iteration in this design aimed to scale components independently, ensuring horizontal scaling for metrics processing and database storage. 

   - **MapReduce** processes large batches of query and click logs to calculate CTR.
   - **Sharded LogJoiner** and **Multidatacenter Calculations** were introduced to further divide tasks across machines and data centers, enhancing both performance and fault tolerance.

4. **Evaluations and Adjustments**  
   Each design iteration addresses scaling and failure resilience. For example, adding more machines to the LogJoiner allows the system to meet SLOs under heavy load. Additionally, distributing components across data centers supports resilience against individual data center failures.

#### Conclusion
The NALSD approach exemplifies iterative, real-world system design focused on reliability. By identifying physical constraints, balancing load across distributed resources, and accounting for failure modes, NALSD enables SREs to build systems that are practical, scalable, and resilient. This structured approach helps reduce long-term operational costs and supports Google’s large-scale production needs.