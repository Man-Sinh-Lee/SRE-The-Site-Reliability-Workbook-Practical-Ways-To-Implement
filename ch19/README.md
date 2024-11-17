### Chapter 19: SRE: Reaching Beyond Your Walls

#### **Truths We Hold to Be Self-Evident**

1. **Reliability Is the Most Important Feature**:
   - Reliability underpins user trust, engagement, and the overall value of a system. If a system is unreliable, users will avoid it, diminishing its network effects and usefulness.

2. **Your Users, Not Your Monitoring, Decide Your Reliability**:
   - User perception determines reliability. Systems that appear stable to monitoring but are experienced as unstable by users will still lose trust. Monitoring should preemptively identify issues before users notice.

3. **If You Run a Platform, Then Reliability Is a Partnership**:
   - Platform reliability depends on both the provider and the user’s system. For instance, if a user’s application built on a highly available platform is poorly configured, their perceived reliability will still be low.

4. **Everything Important Eventually Becomes a Platform**:
   - Systems evolve to expose APIs as other services integrate with them. Even without formal APIs, users may create their own integrations, pushing systems toward platformization.

5. **When Your Customers Have a Hard Time, You Have to Slow Down**:
   - Customer struggles consume developer resources through support and fixes. This creates toil and limits innovation. Proactively addressing customer needs reduces friction.

6. **You Will Need to Practice SRE with Your Customers**:
   - Teaching customers SRE principles like SLOs and error budgets ensures they design reliable systems on your platform. This applies to external and internal customers.

---

#### **How to: SRE with Your Customers**

1. **Step 1: SLOs and SLIs Are How You Speak**:
   - SLOs and SLIs standardize communication about reliability. Defining these metrics with customers prevents misunderstandings and reduces unproductive conversations.

2. **Step 2: Audit the Monitoring and Build Shared Dashboards**:
   - Collaborate on monitoring setups and dashboards that highlight meaningful metrics. Shared dashboards improve transparency and streamline problem resolution.

3. **Step 3: Measure and Renegotiate**:
   - After defining SLOs, measure performance to align expectations with reality. Misaligned assumptions, such as unrealistic "five nines" availability, can be corrected.

4. **Step 4: Design Reviews and Risk Analysis**:
   - Conduct reviews to identify issues like single points of failure (SPOFs). Help customers prioritize fixes to optimize reliability.

5. **Step 5: Practice, Practice, Practice**:
   - Simulate incidents to build trust and operational readiness. Joint postmortems deepen collaboration and improve incident handling.

6. **Be Thoughtful and Disciplined**:
   - Engage only with a manageable subset of customers, such as high-revenue or feature-critical users. This ensures sustainable support.

---

#### **Conclusion**
SRE principles increasingly extend beyond internal systems to customer-facing platforms. By adopting a collaborative approach with customers—rooted in SLOs, shared metrics, and joint practices—SRE teams can foster reliability across ecosystems. This approach strengthens relationships and enhances trust while preparing platforms for future challenges.