<div align="center">

# Arshaan Sindhwani

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=16&pause=1000&color=2E8B57&center=true&vCenter=true&width=520&lines=Software+Engineer;Cloud+%26+Platform+Engineering;Backend+Systems+%26+Infrastructure+as+Code" alt="Typing SVG" />

Building reliable backend systems, cloud infrastructure, and data-driven platforms, with a focus on automation, scalability, and clean architecture.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/arshaan-sindhwani)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArshaanSindhwani)

</div>

---

> **Currently:** Open to new opportunities in cloud computing, platform engineering, software engineering, data analytics, and systems architecture.

---

## About Me

Software engineer trained through La Fosse Academy's Technology Training programme, covering software engineering, cloud infrastructure, DevOps, and data engineering. I build full-stack applications and cloud-based systems using JavaScript, Node.js, PostgreSQL, React Native, Firebase, Docker, Terraform, and AWS. Previously led high-throughput, regulated laboratory operations, which sharpened my root cause analysis and structured problem-solving, skills I now apply to debugging and infrastructure reliability.

<p align="center">
  <img src="https://img.shields.io/github/followers/ArshaanSindhwani?label=Followers&style=for-the-badge&color=2E8B57" height="32"/>
  <img src="https://img.shields.io/github/stars/ArshaanSindhwani?label=Stars&style=for-the-badge&color=2E8B57" height="32"/>
  <img src="https://img.shields.io/badge/Actively%20Job%20Hunting-Open%20to%20Work-2E8B57?style=for-the-badge" height="32"/>
</p>

---

## Tech Stack

**Languages**
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Cloud, Infrastructure &amp; DevOps**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure%20DevOps-0078D7?style=flat-square&logo=azuredevops&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=white)

**Application &amp; Backend**
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![React Native](https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

**Data &amp; Testing**
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Featured Projects

### Azure Terraform Platform Demo

🔗 **[github.com/ArshaanSindhwani/azure-terraform-project](https://github.com/ArshaanSindhwani/azure-terraform-project)**

A small, end-to-end Azure platform environment provisioned entirely with Terraform: resource group, VNet, subnet and NSG, a private blob storage account, and an Azure Container App running under a **system-assigned managed identity** with a least-privilege `Storage Blob Data Reader` role, so the workload can access storage without a stored key.

The Azure DevOps pipeline runs **Validate → Plan → Apply** as separate stages, publishing a saved Terraform plan as a pipeline artefact so Apply executes exactly what was reviewed, rather than re-planning on deployment. State is stored remotely in Azure Storage, and an equivalent GitHub Actions workflow is included as an alternative CI/CD path.

**Tech used:** Terraform · Microsoft Azure · Azure Container Apps · Azure DevOps · GitHub Actions · RBAC and Managed Identity · Azure Blob Storage

<table>
<tr>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/azure-devops-pipeline-success.png" alt="Successful Azure DevOps pipeline run" width="260" /><br/><sub>Validate → Plan → Apply pipeline run</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/container-app-overview.png" alt="Container App overview" width="260" /><br/><sub>Container App overview</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/storage-rbac-assignment.png" alt="Storage RBAC assignment" width="260" /><br/><sub>Storage RBAC role assignment</sub></td>
</tr>
</table>

<details>
<summary><b>Architecture and design detail</b></summary>

- Resource group, VNet (`10.0.0.0/16`), application subnet, and NSG permitting inbound HTTPS only
- Standard LRS storage account (TLS 1.2 minimum) with a private `app-data` blob container
- Container Apps environment with a public Container App and a system-assigned managed identity
- `Storage Blob Data Reader` RBAC role scoped to the storage account, no keys or connection strings in the app config
- Three-stage Azure DevOps pipeline using a saved plan artefact to separate review from deployment
- The VNet and NSG are foundation resources for a future VNet-integrated deployment; the Container App is not yet VNet-integrated, and the sample image does not yet read from Blob Storage. The identity and role assignment exist so a real application can add that integration later without introducing a storage secret.

</details>

---

### AgroSense — Agriculture Intelligence Platform

🔗 **[github.com/ArshaanSindhwani/AgroSense](https://github.com/ArshaanSindhwani/AgroSense)**

Full-stack mobile platform for field data capture, mapping, and AI-assisted recommendations, which I architected and led within a 5-person Agile team at La Fosse Academy.

- **Offline-first architecture:** local persistence via AsyncStorage with a connectivity-aware synchronisation queue, syncing deferred updates to Firebase Firestore once connectivity returns
- **Cloud backend:** Firebase Authentication with Firestore as the centralised data store, and event-driven UI updates based on connectivity state
- **Third-party integration:** Gemini API for contextual AI recommendations, OpenWeather for weather intelligence, and OpenStreetMap for geospatial field visualisation

**Tech used:** React Native · Expo · Firebase (Auth &amp; Firestore) · Gemini API · OpenStreetMap · OpenWeather API

<div align="center">
<table width="100%">
<tr>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/login.jpg" alt="AgroSense login screen" width="140" /><br/><sub>Firebase Authentication login</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/dashboard.jpg" alt="AgroSense dashboard" width="140" /><br/><sub>Farm and weather dashboard</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/fields.jpg" alt="AgroSense fields screen" width="140" /><br/><sub>Field and crop management</sub></td>
</tr>
<tr>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/observations.jpg" alt="AgroSense observations screen" width="140" /><br/><sub>Field observation recording</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/recommendations.jpg" alt="AgroSense AI recommendations screen" width="140" /><br/><sub>Gemini AI recommendations</sub></td>
<td width="33%" align="center"><img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/offline-compatible.jpg" alt="AgroSense offline mode" width="140" /><br/><sub>Offline-compatible sync state</sub></td>
</tr>
</table>
</div>

<details>
<summary><b>Architecture and design detail</b></summary>

- Hybrid offline-compatible model combining local persistence with cloud synchronisation
- Queue-based synchronisation system for deferred network operations, rather than blocking on connectivity
- Firestore as the single source of truth once synced, with local storage acting as a durable write buffer
- Event-driven state updates tied to connectivity changes, keeping the UI responsive on unreliable networks

</details>

---

## Other Projects

| Project | Description | Stack |
|---|---|---|
| **[MovieApp](https://github.com/ArshaanSindhwani/MovieApp)** | Multi-service, containerised movie tracking app with TMDB API enrichment, JWT-authenticated REST APIs, and a Docker deployment pipeline. | Node.js · Flask · PostgreSQL · Docker |
| **[EduFun](https://github.com/ArshaanSindhwani/EduFun)** | REST API-based learning platform with a relational schema for users, quizzes, and progress, plus JWT auth and Jest/Supertest test coverage. | Node.js · Express · PostgreSQL · Jest |
| **[Weather DataOps Pipeline](https://github.com/ArshaanSindhwani/Weather-DataOps-Pipeline)** | Dockerised, scheduled ingestion pipeline pulling from the OpenWeather API, with CI/CD deployment triggers via Render. | Node.js · Docker · GitHub Actions · Render |

Each repository has its own README with full architecture detail.

---

## Experience

**Technology Trainee** · La Fosse Academy · Apr 2026 – Jun 2026
Built full-stack applications and cloud deployment workflows (Node.js, PostgreSQL, AWS, Docker, Terraform, GitHub Actions) within a 5-person Agile team; led AgroSense's architecture and offline sync design.

**Associate Consultant** · CPL Life Sciences · Oct 2023 – Oct 2025
Managed recruitment pipelines of 40+ candidates, built Power BI/Excel dashboards for KPI tracking, and drove a 15% increase in client acquisition.

**Senior Scientist** · Cignpost Diagnostics · Oct 2021 – Oct 2022
Led a team of 10 processing up to 10,000 diagnostic samples daily in an ISO 15189 lab; reduced repeat deviations by 25% through CAPA-led root cause analysis.

**Earlier experience:** Laboratory Associate Practitioner at Prenetics (2020–2021) and IT Engineer at iTech Services (2015–2018), delivering infrastructure migrations for clients including Amazon, BBC, and Microsoft. 

**Full employment details on** [LinkedIn](https://www.linkedin.com/in/arshaan-sindhwani)

---

## Education

- **MSc Genomic Medicine**, University of Sheffield, 2020 — Merit, Course Representative
- **BSc Biomedical Sciences (IBMS Accredited)**, University of Roehampton, 2019 — First Class Honours

---

## Contact Me

<div align="center">

**Cloud Platforms • Infrastructure as Code • Platform Engineering • Backend Scalability • Data Pipelines**

I'm actively looking for new opportunities in cloud, platform engineering, and software engineering. Feel free to reach out.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/arshaan-sindhwani)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArshaanSindhwani)

</div>
