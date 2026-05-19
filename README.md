# 🚀 Standardized Corporate AI Developer Sandbox Website

This repository hosts the public, customer-facing product landing page for the **Corporate AI Developer Sandbox** offering. Deployed globally via GitHub Pages, this high-contrast, light-themed responsive sales asset targets small and medium enterprises (SMEs) across the UK, addressing compliance vulnerabilities related to "Shadow AI" and local laptop model engineering.

🌐 **Live URL:** [https://github.io](https://github.io)

---

## 🏗️ Architectural Topology of the Product

The underlying solution architecture marketed on this landing page transforms raw cloud building blocks into an audited corporate environment. The configuration consists of:

### 1. Compute & Performance Profiles
* **Instance Family:** Cost-optimized AMD EPYC `t3a.xlarge` nodes (4 vCPUs, 16 GB RAM) for testing, seamlessly scaling up to NVIDIA-accelerated `g4dn.xlarge` (T4 GPU) or `g5.xlarge` (A10G GPU) infrastructure for active production tuning.
* **Region Strategy:** Native positioning inside local server perimeters (e.g., AWS London `eu-west-2` or AWS Mumbai `ap-south-1`) to easily satisfy localized data localization and data sovereignty requirements.

### 2. Isolated 3-Disk Storage Fabric
To guarantee operational isolation and eliminate root storage disk thrashing, the system utilizes a custom, decoupled filesystem block structure:
* **Volume 1 (OS Boot):** 200 GB `gp3` SSD drive handling baseline system daemons, core logging architectures, and Linux runtime components.
* **Volume 2 (Developer Utilities):** 200 GB `gp3` SSD drive hosting the isolated Python Miniconda distribution, Git frameworks, and token-secured JupyterLab reverse-proxy systems.
* **Volume 3 (AI Workload Cache):** 400 GB high-performance `gp3` SSD drive maxed out to **500 MB/s throughput** and **6,000 IOPS**. It maps environmental overrides (`HF_HOME`) to isolate Hugging Face weight downloads, text datasets, and local vector indices (ChromaDB) from the rest of the file system.

### 3. Corporate Security Boundaries
* **Egress Filtering:** Strict AWS Security Group controls block outbound file tracking to mitigate data extraction risks.
* **Cost Controls:** Automated CloudWatch alarms monitor processor metrics, triggering an immediate system shutdown if left idle for over 60 minutes.
* **Data Shielding:** Native integration via the AWS SDK to serverless foundation gates like **Amazon Bedrock**, ensuring prompt inputs never train public third-party models.

---

## 🛠️ Repository File Structures

```text
├── index.html         # Bright corporate light-theme sales landing page
└── README.md          # Core architecture, catalog properties, and operational workflows
```

---

## 📞 Business Operations & Order Fulfillment

All consumer queries, custom architecture discussions, and onboarding triggers funnel directly through verified manual communication channels to ensure a personalized, high-trust B2B delivery experience:

* **Principal Consultant:** Jaikant S Rao (35 Years Data Center & Cloud Services Industry Experience)
* **📬 Business Intake Email:** [jaikantsrao@gmail.com](mailto:jaikantsrao@gmail.com)
* **💬 Corporate WhatsApp:** [+91-9900725080](https://wa.me)
* **⚡ Service Level Agreement (SLA):** Complete hands-free remote delivery inside the client's private AWS account via secure, cross-account IAM role handshakes in under 48 hours.
