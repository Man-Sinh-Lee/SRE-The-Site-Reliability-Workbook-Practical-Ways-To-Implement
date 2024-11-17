### Chapter 21: Organizational Change Management in SRE

#### **SRE Embraces Change**
- SRE teams are positioned to balance rapid innovation with reliability in fast-paced environments. Error budgets provide a mechanism to balance the risks of change with service reliability.

---

#### **Introduction to Change Management**

1. **Lewin’s Three-Stage Model**:
   - A foundational model with three stages:
     - **Unfreeze**: Prepare the organization for change by addressing resistance.
     - **Change**: Implement the changes incrementally.
     - **Freeze**: Solidify new processes into the culture.

2. **McKinsey’s 7-S Model**:
   - Focuses on aligning seven organizational elements: structure, strategy, systems, skills, style, staff, and shared values. Useful for transitioning from traditional IT operations to SRE.

3. **Kotter’s Eight-Step Process for Leading Change**:
   - Includes steps like creating urgency, forming a vision, empowering teams, and institutionalizing changes. Suitable for structured, large-scale transformations.

4. **The Prosci ADKAR Model**:
   - Emphasizes the individual journey through Awareness, Desire, Knowledge, Ability, and Reinforcement. Applicable for distributed teams.

5. **Emotion-Based Models**:
   - Models like Kübler-Ross’s Change Curve address emotional responses to change, helping leaders anticipate team reactions and maintain morale.

6. **The Deming Cycle (PDCA)**:
   - Iterative approach for continuous improvement but less applicable for managing large organizational changes due to its mechanical focus.

---

#### **Case Study 1: Scaling Waze—From Ad Hoc to Planned Change**

1. **Background**:
   - Waze experienced scaling challenges post-acquisition, with SREs addressing critical messaging queue issues under high operational pressure.

2. **The Messaging Queue**:
   - Waze rebuilt its messaging queue to meet increased demands. The process involved a phased migration, collaborative development, and iterative improvements.

3. **The Next Cycle of Change**:
   - Improved deployment processes using lessons from the queue migration. Incremental changes and collaboration between SREs and developers enabled smoother transitions.

4. **Lessons Learned**:
   - Change management frameworks like Kotter’s can streamline ad hoc processes.
   - Cross-functional teams and executive support are critical for large technical changes.

---

#### **Case Study 2: Common Tooling Adoption in SRE**

1. **Background**:
   - SREs used disparate tools for monitoring, rollouts, and incident management. The lack of standardization led to inefficiencies.

2. **Problem Statement**:
   - Fragmentation of tools hindered operational efficiencies and scalability across teams.

3. **What We Decided to Do**:
   - Proposed a unified monitoring platform with minimal customization requirements. Engineers contributed through a virtual team structure.

4. **Design and Implementation**:
   - A zero-configuration dashboard was created to standardize monitoring. Iterative updates ensured adoption while minimizing migration costs.

5. **Lessons Learned**:
   - Migration costs must be outweighed by clear benefits.
   - Collaboration with users and addressing resistance are critical for adoption.

---

#### **Conclusion**
Change management is integral to SRE. While no single model applies universally, frameworks like Kotter’s Eight-Step Process and the ADKAR model provide valuable guidance for technical and organizational transformations. The importance of iterative change, collaboration, and structured planning are consistent themes across case studies.