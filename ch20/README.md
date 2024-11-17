### Chapter 20: SRE Team Lifecycles

#### **SRE Practices Without SREs**
- Organizations can adopt foundational SRE practices without dedicated SRE teams by implementing **SLOs (Service Level Objectives)** with associated consequences.
- Error budgets, informed by SLOs, help teams balance reliability with velocity, guiding business decisions on prioritization and risk tolerance.

---

#### **Starting an SRE Role**

1. **Finding Your First SRE**:
   - Ideal candidates have expertise in operations, system architecture, monitoring, and production automation. They must balance reliability and velocity goals.
   
2. **Placing Your First SRE**:
   - Placement options include embedding in product development, operations, or a horizontal consulting role. The decision depends on organizational needs and challenges.

3. **Bootstrapping Your First SRE**:
   - Initial work includes improving monitoring, addressing postmortem action items, and automating toil reduction. Ensuring alignment with SLOs is critical.

4. **Distributed SREs**:
   - In the absence of a centralized team, distributed SREs require a supportive community to share practices and maintain consistency.

---

#### **Your First SRE Team**
- Teams evolve through Tuckman’s stages:
  1. **Forming**: Assemble members with expertise in reliability, automation, and system design. Seed with experienced internal transfers to build cohesion.
  2. **Storming**: Address team dynamics and challenges through collaborative forums and learning initiatives.
  3. **Norming**: Establish best practices like sustainable on-call rotations, SLO adherence, and error budgeting.
  4. **Performing**: Teams operate efficiently, focusing on impactful reliability projects while maintaining strong relationships with stakeholders.

---

#### **Making More SRE Teams**

1. **Service Complexity**:
   - As services grow, split teams along architectural, language, or geographical lines to manage complexity effectively.

2. **SRE Rollout**:
   - Prioritize high-impact or business-critical services for new SRE teams. Avoid engaging SREs in unreliable systems without addressing root causes first.

3. **Geographical Splits**:
   - Multisite teams improve reliability and reduce on-call stress. Maintain balanced workloads and foster collaboration across sites.

---

#### **Suggested Practices for Running Many Teams**

1. **Mission Control**:
   - Embed developers in SRE teams temporarily to enhance mutual understanding of reliability practices.
   
2. **SRE Exchange**:
   - Facilitate short-term rotations between SRE teams to share knowledge and practices.

3. **Training**:
   - Provide standardized training like Google’s SRE EDU to ensure consistent knowledge across teams.

4. **Horizontal Projects**:
   - Centralize solutions for common challenges like monitoring and automation to reduce duplicated efforts.

5. **Mobility and Travel**:
   - Encourage team transfers and in-person interactions to foster collaboration and retain talent.

6. **Launch Coordination Engineering Teams**:
   - Apply SRE principles to services without full SRE engagement, using automation and standard tooling.

---

#### **Conclusion**
This chapter provides a roadmap for evolving SRE practices from an unstaffed state to a robust, distributed organization. Establishing strong foundations with SLOs, scaling teams based on service complexity, and fostering cross-team collaboration ensures long-term reliability and operational excellence.