# Topic 4.1: Cloud Service Models (IaaS, PaaS, SaaS)

In the **Shared Responsibility Model**, cloud services are categorized into three main service types: **IaaS**, **PaaS**, and **SaaS**. As you move from IaaS to SaaS, Azure takes away more of your operational workload.

---

## ☁️ 2. IaaS — Infrastructure as a Service

### Overview
**IaaS** means Azure provides the basic computing infrastructure (physical datacenter, physical servers, networking, and storage), while you manage much of the software environment. You are responsible for configuring the virtual machines, operating system, applications, and data.

### When is it used?
* When you need maximum control over the server and operating system.
* When running legacy software that requires specific OS settings or custom server configurations.
* When migrating existing on-premises workloads to the cloud with minimal changes (Lift and Shift).

### 🏦 Real-Life Example
> **Legacy Windows Application:**  
> A enterprise needs a Windows Server to run a specialized legacy app. Instead of purchasing physical server hardware, the IT team provisions an **Azure Virtual Machine (VM)**. Microsoft handles the physical datacenter and hardware, while the internal IT team installs Windows updates, configures firewalls, and maintains the application.

### 📋 Responsibilities Breakdown

| Layer | Managed By | Description |
| :--- | :---: | :--- |
| 🏭 **Physical Infrastructure** | **Azure** | Data center physical security, power, cooling, physical servers, and physical cables. |
| 💻 **Virtual Machine (VM)** | **You** | Selecting VM sizes, attached disks, and virtual network configuration. |
| 💿 **Operating System (OS)** | **You** | Installing OS security patches, updates, and configuration settings. |
| 📱 **Applications** | **You** | Installing, updating, and maintaining application code inside the VM. |
| 🔐 **Data & Access** | **You** | Securing application data, setting permissions, and managing database backups. |

### 📐 IaaS Diagram

```text
☁️ AZURE PLATFORM
    │
    ├── 🏢 Data Center       → Azure
    ├── 🖥️ Physical Server   → Azure
    ├── ⚡ Power + Cooling    → Azure
    └── 🌐 Physical Network  → Azure
              │
              ↓
        💻 YOUR VIRTUAL MACHINE
              │
        ├── 💿 Operating System → You
        ├── 📱 Applications    → You
        └── 🔐 Data & Access    → You
```

---

## ☁️ 3. PaaS — Platform as a Service

### Overview
**PaaS** means Azure manages both the physical infrastructure **and** the underlying operating system and runtime platform for you. Developers can focus entirely on writing application code, building APIs, and managing data without worrying about server provisioning or OS patching.

### When is it used?
* When developers want to build, test, and deploy applications rapidly.
* When you want to eliminate OS administration and server maintenance overhead.
* When building modern web apps, microservices, or APIs.

### 💻 Real-Life Example
> **Web API Deployment:**  
> A software team builds an ASP.NET Core Web API. Instead of manually creating VMs, installing Windows Server, and configuring IIS web server software, they deploy directly to **Azure App Service**. Azure automatically handles OS patches, server scaling, and framework updates.

### 📋 Responsibilities Breakdown

| Layer | Managed By | Description |
| :--- | :---: | :--- |
| 🏭 **Physical Infrastructure** | **Azure** | Datacenters, physical servers, power, cooling, and hardware maintenance. |
| 💿 **Operating System & Runtime** | **Azure** | OS installation, security patching, runtime engine (.NET, Node.js, Python). |
| ⚙️ **Platform & Scaling** | **Azure** | Load balancing, auto-scaling, OS updates, and framework security. |
| 📱 **Application** | **You** | Writing, deploying, configuring, and updating your application code. |
| 🔐 **Data & Access** | **You** | Data protection, database backups, user authentication, and API access rules. |

### 📐 PaaS Diagram

```text
☁️ AZURE PLATFORM
    │
    ├── 🏢 Data Center       → Azure
    ├── 🖥️ Servers           → Azure
    ├── 💿 Operating System  → Azure
    └── ⚙️ Platform Runtime   → Azure
              │
              ↓
        👨‍💻 YOUR APPLICATION
              │
        ├── 📱 ASP.NET / Node App → You
        └── 🔐 Application Data   → You
```

---

## ☁️ 4. SaaS — Software as a Service

### Overview
**SaaS** is a complete, fully managed software application provided over the internet. The cloud provider manages the physical infrastructure, operating system, network, database, and application code. Your primary responsibilities are managing user accounts, access permissions, and your data.

### When is it used?
* When you want ready-to-use software applications without building or hosting them yourself.
* For standard enterprise tools like email, collaboration software, CRM, and cloud storage.

### 💼 Real-Life Example
> **Enterprise Email & Collaboration:**  
> A company uses **Microsoft 365** (Outlook, Teams, SharePoint) for daily business operations. Microsoft hosts the servers, patches software, and ensures 99.9% uptime. The company’s IT team simply manages employee accounts, passwords, and permissions.

### 📋 Responsibilities Breakdown

| Layer | Managed By | Description |
| :--- | :---: | :--- |
| 🏭 **Physical Infrastructure** | **Microsoft** | Datacenters, physical host servers, power, and physical network connections. |
| 💿 **OS & Server Stack** | **Microsoft** | All server operating systems, databases, and network virtualizations. |
| ⚙️ **Software Application** | **Microsoft** | Feature development, bug fixes, software updates, and security patching. |
| 👥 **Users & Access** | **You** | Managing user identities, multi-factor authentication (MFA), and permissions. |
| 📄 **Data** | **You** | Managing and classifying company documents, emails, and sensitive files. |

### 📐 SaaS Diagram

```text
☁️ MICROSOFT PLATFORM
    │
    ├── 🏢 Data Center       → Microsoft
    ├── 🖥️ Physical Servers  → Microsoft
    ├── 💿 Operating System  → Microsoft
    ├── ⚙️ Application Code  → Microsoft
    └── 🔧 Maintenance       → Microsoft
              │
              ↓
        👨‍💻 YOUR ORGANIZATION
              │
        ├── 👥 User Accounts → You
        ├── 🔐 Access & MFA  → You
        └── 📄 Company Data  → You
```

---

## 🔑 The Main Difference

Think of cloud service types on a spectrum of control vs. convenience:

```text
More Responsibility for YOU (Maximum Control)
                 │
          🏢 On-Premises
                 │
              ☁️ IaaS
                 │
              ☁️ PaaS
                 │
              ☁️ SaaS
                 │
More Responsibility for CLOUD PROVIDER (Maximum Convenience)
```

### 📊 Quick Comparison Matrix

| Service Model | Physical Infrastructure | Operating System | Application Code | User Data & Access |
| :--- | :---: | :---: | :---: | :---: |
| 🏢 **On-Premises** | You | You | You | You |
| ☁️ **IaaS** | Azure | **You** | **You** | **You** |
| ☁️ **PaaS** | Azure | Azure | **You** | **You** |
| ☁️ **SaaS** | Microsoft | Microsoft | Microsoft | **You** |
