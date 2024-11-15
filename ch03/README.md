### Summary of Chapter 3: SLO Engineering Case Studies

#### Evernote’s SLO Story

**Why Did Evernote Adopt the SRE Model?**  
Evernote faced tension between its operations and development teams due to differing goals. Operations prioritized stability, while development sought rapid feature releases, leading to strained relations. The company moved towards an SRE model centered on error budgets and SLOs, bridging the gap between these goals and providing a consistent framework that both teams could support.

**Introduction of SLOs: A Journey in Progress**  
After migrating from physical datacenters to Google Cloud Platform (GCP), Evernote introduced SLOs to align teams internally and with Google’s Cloud team. The initial focus was on a simple uptime SLO, which helped create shared metrics for service quality. Despite an evolving approach, Evernote embraced a “good enough” mentality, allowing flexibility to revise SLOs as needs evolved.

**Breaking Down the SLO Wall Between Customer and Cloud Provider**  
Evernote worked to break down barriers with GCP, focusing on aligning goals and using shared performance dashboards with Google. This relationship enabled proactive issue handling and facilitated a two-way approach to incident management, where Google’s Customer Reliability Engineering (CRE) team actively monitored Evernote’s performance to align with specific SLOs.

**Current State**  
Within nine months, Evernote reached the third version of its SLO model. The company aims to develop more granular SLOs focused on individual API calls and in-client performance metrics. By standardizing Quality of Service (QoS) measures, Evernote now engages in data-driven discussions to improve reliability both internally and with Google.

#### The Home Depot’s SLO Story

**The SLO Culture Project**  
The Home Depot’s (THD) transformation toward microservices and full-stack ownership required a new accountability framework. To meet this, THD launched a cultural initiative, “VALET” (Volume, Availability, Latency, Errors, and Tickets), which created a common language around SLOs. With VALET, THD began defining and measuring SLOs across its microservices.

**Our First Set of SLOs**  
THD’s initial SLOs prioritized availability and latency for API calls among microservices, helping teams set expectations and manage dependencies effectively. SLOs were embedded in developer accountability through regular reviews, providing a clear framework to maintain service quality.

**Evangelizing SLOs**  
The organization engaged in extensive outreach, using tools like training workshops, internal blogs, and marketing materials (e.g., t-shirts, stickers) to promote VALET and SLO culture. This initiative fostered a shared understanding of SLOs, elevating SLO adherence to a priority in performance evaluations.

**Automating VALET Data Collection**  
THD introduced a framework named “TPS Reports” to automate VALET data collection, which transformed operational data into actionable SLO metrics. Integrations with BigQuery and chat platforms allowed real-time reporting and cross-service SLO evaluation, streamlining troubleshooting and review processes.

**The Proliferation of SLOs**  
After initial adoption, THD rapidly expanded its use of SLOs, with over 800 services using the VALET framework. The VALET Dashboard facilitated this scale by allowing easy SLO reporting and trend analysis, which helped solidify SLO practices across the organization.

**Applying VALET to Batch Applications and Using VALET in Testing**  
The VALET framework was adapted for batch processes, measuring metrics like processing volume and latency for scheduled jobs. Additionally, VALET supported chaos engineering in staging environments, allowing THD to monitor system resilience under controlled stress testing.

**Future Aspirations**  
THD aims to integrate an error budget culture, pausing new feature releases when SLOs are breached. The company plans to fine-tune reporting timeframes to balance service quality and development speed, ensuring that SLOs continue to drive reliability improvements.

#### Conclusion
Both Evernote and THD successfully implemented SLO-centric models, enhancing collaboration and system reliability. Evernote’s journey highlighted the importance of internal and external alignment, while THD’s comprehensive cultural shift showed how large-scale SLO adoption can benefit organizations.