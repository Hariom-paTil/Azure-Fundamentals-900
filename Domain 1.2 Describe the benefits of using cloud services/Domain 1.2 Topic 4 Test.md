# Domain 1.2: Describe the Benefits of Using Cloud Services — Practice Test

This practice test covers all key topics from **Domain 1.2** and fundamental cloud concepts for the **AZ-900: Microsoft Azure Fundamentals** exam.

> 📝 **How to take this test:**
> 1. Try answering all 24 questions on your own first.
> 2. You can click on the **"👁️ Click to Reveal Answer & Explanation"** drop-down under each question to check your answer immediately, **OR**
> 3. Scroll to the bottom to view the **Complete Answer Key & Score Tracker**.
> 4. *(Bonus)* Open the companion [`Domain 1.2 Interactive Test.html`](file:///d:/Azure/Azure-Fundamentals-900/Domain%201.2%20Describe%20the%20benefits%20of%20using%20cloud%20services/Domain%201.2%20Interactive%20Test.html) in your browser for a live interactive test with a "Submit & Score" button!

---

### Q1.
A company has an application running on Azure. During a festival, the number of users increases from 10,000 to 500,000. After the festival, traffic returns to normal.

Which capability is most useful?

- [ ] A. Governance
- [ ] B. Scalability
- [ ] C. Private cloud
- [ ] D. CapEx

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Scalability**
>
> **Explanation:**  
> **Scalability** (specifically elasticity / horizontal scaling) allows an application to automatically increase computing resources during traffic spikes (from 10k to 500k users) and scale back down when demand normalizes.
</details>

---

### Q2.
A company wants to use its existing VMware workloads but move them to Azure with minimal changes.

Which Azure solution should it consider?

- [ ] A. Azure Arc
- [ ] B. Azure VMware Solution
- [ ] C. Azure SQL Database
- [ ] D. Azure Blob Storage

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Azure VMware Solution**
>
> **Explanation:**  
> **Azure VMware Solution (AVS)** provides private cloud clusters containing VMware vSphere environments running directly on dedicated bare-metal Azure infrastructure, allowing seamless migration of existing VMware workloads without refactoring.
</details>

---

### Q3.
A company buys physical servers, networking equipment, and cooling systems for its own data center.

Which type of expenditure is this?

- [ ] A. OpEx
- [ ] B. SaaS
- [ ] C. CapEx
- [ ] D. Consumption-based

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. CapEx**
>
> **Explanation:**  
> **Capital Expenditure (CapEx)** refers to upfront spending on physical hardware, equipment, and on-premises datacenter facilities that are deducted as depreciation over time.
</details>

---

### Q4.
An organization wants its cloud environment to automatically identify resources that don't follow company policies.

Which capability is most relevant?

- [ ] A. Auditing
- [ ] B. Horizontal scaling
- [ ] C. Load balancing
- [ ] D. Virtualization

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Auditing**
>
> **Explanation:**  
> **Auditing** (using tools like **Azure Policy** compliance evaluation and Activity Logs) automatically scans resources, identifies non-compliant configurations (e.g., missing encryption or wrong region), and flags violations.
</details>

---

### Q5.
A company hosts its application in Azure but wants to keep its sensitive database in its own data center.

Which cloud model best describes this environment?

- [ ] A. Public
- [ ] B. Private
- [ ] C. Hybrid
- [ ] D. Multicloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. Hybrid**
>
> **Explanation:**  
> A **Hybrid Cloud** environment connects a public cloud provider (Azure) with an on-premises private datacenter, allowing data and apps to be shared securely between them.
</details>

---

### Q6.
An application is running on an Azure VM with 4 CPUs and 8 GB RAM. The CPU is constantly overloaded. The company increases the VM to 16 CPUs and 32 GB RAM.

What has happened?

- [ ] A. Scale out
- [ ] B. Scale in
- [ ] C. Vertical scaling
- [ ] D. Horizontal scaling

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. Vertical scaling**
>
> **Explanation:**  
> **Vertical Scaling (Scale Up)** means upgrading the hardware specs (CPU cores, RAM, disk speed) of an **existing single server/VM**. Horizontal scaling would mean adding *more* VM instances.
</details>

---

### Q7.
A company wants developers to deploy an ASP.NET Core API without managing the underlying operating system or physical servers.

Which option is most appropriate?

- [ ] A. Azure Virtual Machines
- [ ] B. Azure App Service
- [ ] C. Physical data center
- [ ] D. VMware

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Azure App Service**
>
> **Explanation:**  
> **Azure App Service** is a **Platform as a Service (PaaS)** offering that allows developers to deploy web applications and APIs without managing the OS, patching, or physical servers.
</details>

---

### Q8.
A company uses Azure for its API, another public cloud provider for analytics, and a third provider for storage.

What type of environment is this?

- [ ] A. Hybrid cloud
- [ ] B. Private cloud
- [ ] C. Multicloud
- [ ] D. On-premises

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. Multicloud**
>
> **Explanation:**  
> A **Multicloud** environment uses services across **two or more distinct public cloud providers** (such as Azure, AWS, and GCP).
</details>

---

### Q9.
A company's application must continue operating even if an entire Azure region becomes unavailable.

What should the organization consider?

- [ ] A. Deploying the application across multiple regions
- [ ] B. Increasing the RAM of one VM
- [ ] C. Buying physical servers
- [ ] D. Using only one VM

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Deploying the application across multiple regions**
>
> **Explanation:**  
> Deploying across **multiple Azure regions (Multi-Region Disaster Recovery)** ensures that if one entire geographical region suffers an outage or natural disaster, traffic is redirected to another active region.
</details>

---

### Q10.
A company wants to estimate the potential cost of running a workload in Azure before deploying it.

Which tool is most suitable?

- [ ] A. Azure Pricing Calculator
- [ ] B. Azure Arc
- [ ] C. Azure VMware Solution
- [ ] D. Azure Monitor only

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Azure Pricing Calculator**
>
> **Explanation:**  
> The **Azure Pricing Calculator** is a free web-based tool used to configure and estimate expected cloud spending **before** deploying any resources into Azure.
</details>

---

### Q11.
A company has 1,000 Azure resources. It wants every production resource to follow the same required configuration.

Which approach would help maintain consistency?

- [ ] A. Templates
- [ ] B. Buying more servers
- [ ] C. Vertical scaling
- [ ] D. Multicloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Templates**
>
> **Explanation:**  
> **Templates** (ARM Templates, Azure Bicep, Terraform) implement **Infrastructure as Code (IaC)**, ensuring that every deployment follows identical, pre-approved configuration standards.
</details>

---

### Q12.
A company wants to run an application but does not want to purchase physical servers or maintain a data center.

What cloud characteristic provides this benefit?

- [ ] A. Consumption-based cloud model
- [ ] B. Private cloud only
- [ ] C. CapEx
- [ ] D. On-premises computing

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Consumption-based cloud model**
>
> **Explanation:**  
> The **Consumption-based model** (OpEx) allows companies to rent cloud infrastructure on demand and only pay for what they consume, completely avoiding server purchases and datacenter maintenance.
</details>

---

### Q13.
An online banking application needs to remain available even if one server fails.

Which architecture would best support this requirement?

- [ ] A. One powerful server only
- [ ] B. Multiple application instances
- [ ] C. One physical computer
- [ ] D. One VM with maximum RAM

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Multiple application instances**
>
> **Explanation:**  
> Running **multiple redundant instances** behind a load balancer ensures **High Availability (HA)**. If one instance fails, user requests are immediately routed to healthy instances with zero downtime.
</details>

---

### Q14.
A company uses a cloud service where the provider manages the application, operating system, infrastructure, and most maintenance. The company mainly manages users, settings, and its data.

Which model is this?

- [ ] A. IaaS
- [ ] B. PaaS
- [ ] C. SaaS
- [ ] D. Private cloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. SaaS**
>
> **Explanation:**  
> In **Software as a Service (SaaS)** (e.g., Microsoft 365), the vendor delivers a fully managed end-user application. The customer is only responsible for user access, settings, and data.
</details>

---

### Q15.
A company wants maximum control over the operating system and installed software running on its Azure workload.

Which model gives it the most control?

- [ ] A. SaaS
- [ ] B. PaaS
- [ ] C. IaaS
- [ ] D. Public cloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **C. IaaS**
>
> **Explanation:**  
> **Infrastructure as a Service (IaaS)** (e.g., Azure Virtual Machines) provides the highest level of administrative control over the OS, networking, storage, and software configuration.
</details>

---

### Q16.
A company's website normally uses two VMs. During a major event, it automatically creates eight additional VMs and removes them when traffic decreases.

Which capability is being demonstrated?

- [ ] A. Governance
- [ ] B. Autoscaling
- [ ] C. CapEx
- [ ] D. Private cloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Autoscaling**
>
> **Explanation:**  
> **Autoscaling** (Horizontal Elasticity / Scale Sets) automatically provisions extra VM instances when traffic spikes and deprovisions them when traffic subsides to save money.
</details>

---

### Q17.
A company has resources running in Azure, its own data center, and another cloud provider. It wants to manage these resources using Azure management capabilities.

Which technology is designed for this purpose?

- [ ] A. Azure Arc
- [ ] B. Azure VMware Solution
- [ ] C. Azure App Service
- [ ] D. Azure Virtual Machines

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Azure Arc**
>
> **Explanation:**  
> **Azure Arc** extends Azure management, governance policies, and Azure services across on-premises environments, edge devices, and multicloud platforms.
</details>

---

### Q18.
An organization wants to protect its application from a large amount of malicious network traffic designed to make the service unavailable.

What type of attack is this?

- [ ] A. DDoS
- [ ] B. Scaling
- [ ] C. Governance
- [ ] D. Virtualization

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. DDoS**
>
> **Explanation:**  
> A **Distributed Denial of Service (DDoS)** attack attempts to overwhelm a target server with massive amounts of malicious traffic. Azure provides **Azure DDoS Protection** to absorb and scrub this traffic.
</details>

---

### Q19.
A company has a server that is powerful enough for its workload, but the number of incoming requests has become too large for one server.

What is the most appropriate scaling approach?

- [ ] A. Add CPU to the same server only
- [ ] B. Add more application instances
- [ ] C. Reduce RAM
- [ ] D. Move to CapEx

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Add more application instances**
>
> **Explanation:**  
> When the request volume exceeds what a single server can process, **Horizontal Scaling (Scale Out)** by adding more identical server instances distributes the incoming load across multiple nodes.
</details>

---

### Q20.
A company is responsible for its application data and user access, while Microsoft manages the physical data center, power, cooling, and physical network.

Which concept does this describe?

- [ ] A. Consumption-based model
- [ ] B. Shared responsibility model
- [ ] C. Multicloud model
- [ ] D. Vertical scaling

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Shared responsibility model**
>
> **Explanation:**  
> The **Shared Responsibility Model** defines which security and maintenance tasks belong to the cloud customer and which tasks belong to the cloud provider (Microsoft).
</details>

---

### Q21.
A company wants to reduce its cloud costs when application traffic decreases.

What should it do?

- [ ] A. Keep all resources running at maximum capacity
- [ ] B. Scale down resources when demand decreases
- [ ] C. Purchase additional physical servers
- [ ] D. Move everything to private cloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **B. Scale down resources when demand decreases**
>
> **Explanation:**  
> **Scaling in / down** (reducing VM instances or down-tiering compute specs) when demand drops minimizes resource consumption, directly lowering cloud billing costs.
</details>

---

### Q22.
A company creates a policy that only authorized employees can access production resources.

What area does this primarily relate to?

- [ ] A. Governance and access control
- [ ] B. Vertical scaling
- [ ] C. CapEx
- [ ] D. Multicloud

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Governance and access control**
>
> **Explanation:**  
> Controlling who can view or manage production resources is part of **Governance and Access Control** (enforced via **Azure Role-Based Access Control (RBAC)** and Conditional Access).
</details>

---

### Q23.
An Azure service has an availability commitment describing the expected level of uptime.

What does this commitment represent?

- [ ] A. SLA
- [ ] B. CapEx
- [ ] C. VM
- [ ] D. DDoS

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. SLA**
>
> **Explanation:**  
> A **Service Level Agreement (SLA)** is Microsoft’s formal contractual commitment guaranteeing specific availability, uptime, and performance metrics (e.g., 99.9% or 99.99%).
</details>

---

### Q24.
A company wants to avoid purchasing hardware that may remain unused for most of the year. It wants to increase resources during busy periods and reduce them afterward.

Which cloud concept best matches this requirement?

- [ ] A. Consumption-based model
- [ ] B. Private cloud
- [ ] C. CapEx
- [ ] D. On-premises model

<details>
<summary><b>👁️ Click to Reveal Answer & Explanation</b></summary>

> **Correct Answer:** **A. Consumption-based model**
>
> **Explanation:**  
> In a **Consumption-based model**, you pay only for the compute and storage resources you actively use. You avoid idle hardware waste by scaling up during peaks and deallocating resources during lulls.
</details>

---

## 📊 Complete Answer Key Table

| Question | Correct Option | Core Concept Tested |
| :---: | :---: | :--- |
| **Q1** | **B** | Scalability & Elasticity |
| **Q2** | **B** | Azure VMware Solution (AVS) |
| **Q3** | **C** | Capital Expenditure (CapEx) |
| **Q4** | **A** | Auditing & Compliance (Azure Policy) |
| **Q5** | **C** | Hybrid Cloud Model |
| **Q6** | **C** | Vertical Scaling (Scale Up) |
| **Q7** | **B** | Azure App Service (PaaS) |
| **Q8** | **C** | Multicloud Model |
| **Q9** | **A** | Multi-Region High Availability & Disaster Recovery |
| **Q10** | **A** | Azure Pricing Calculator |
| **Q11** | **A** | Infrastructure as Code / Templates |
| **Q12** | **A** | Consumption-Based Model |
| **Q13** | **B** | Redundant Application Instances |
| **Q14** | **C** | Software as a Service (SaaS) |
| **Q15** | **C** | Infrastructure as a Service (IaaS) |
| **Q16** | **B** | Autoscaling (Horizontal Elasticity) |
| **Q17** | **A** | Azure Arc (Multicloud & On-Premises Management) |
| **Q18** | **A** | DDoS (Distributed Denial of Service) Attack |
| **Q19** | **B** | Horizontal Scaling (Scale Out) |
| **Q20** | **B** | Shared Responsibility Model |
| **Q21** | **B** | Cost Optimization via Scaling Down |
| **Q22** | **A** | Governance & Access Control (Azure RBAC) |
| **Q23** | **A** | Service Level Agreement (SLA) |
| **Q24** | **A** | Consumption-Based Cloud Model |

---

## 🎯 Score Calculation Breakdown

* **22 – 24 Correct:** 🌟 **Mastery (Pass with Distinction)** – You have a thorough understanding of Domain 1.2!
* **18 – 21 Correct:** ✅ **Pass (Solid Foundation)** – Ready for exam questions on cloud benefits.
* **14 – 17 Correct:** ⚠️ **Review Recommended** – Revisit Topics 1, 2, and 3 for reinforcement.
* **Below 14:** 🔄 **Retake Required** – Review the Shared Responsibility Model, Scaling, and Cloud Models.
