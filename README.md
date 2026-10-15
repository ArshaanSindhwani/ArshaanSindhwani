
<div align="center">

# Arshaan Sindhwani

**Software Engineering | Data Engineering | Cloud and Platform Engineering**

Building applications, data pipelines and cloud infrastructure.

London, UK · Open to on-site, hybrid and remote opportunities

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/arshaan-sindhwani)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArshaanSindhwani)

</div>

---

## About

I build software and cloud-based systems, from REST APIs and relational databases to automated data pipelines and infrastructure provisioned with Terraform.

Through La Fosse Academy and technical projects, I have developed practical experience with JavaScript, Node.js, Python, PostgreSQL, AWS, Azure, Docker and CI/CD. My work includes a serverless AWS image-processing pipeline, an Azure environment managed through Terraform, automated weather data collection, and backend services with automated testing.

My earlier experience in IT infrastructure, laboratory operations and consultancy has also given me experience in troubleshooting, technical documentation, data quality and structured problem-solving.

I am looking for early-career opportunities across software engineering, data engineering, cloud engineering and platform engineering.

## Technical Skills

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Cloud, Infrastructure and Automation**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azuredevops&logoColor=white)

**Software and Data**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

**Testing and Development Tools**

![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Supertest](https://img.shields.io/badge/Supertest-333333?style=flat-square)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)

---

## Featured Projects

### 1. Azure Terraform Platform Demo

[View Repository](https://github.com/ArshaanSindhwani/azure-terraform-project)

An Azure environment provisioned with Terraform, covering networking, storage, container hosting, identity and automated deployment.

**Engineering highlights**

- Defined Azure infrastructure as code, including a resource group, virtual network, subnet, network security group, storage account and Azure Container App.
- Configured a system-assigned managed identity with storage-scoped `Storage Blob Data Reader` permissions.
- Built an Azure DevOps pipeline with separate Validate, Plan and Apply stages.
- Published a saved Terraform plan as a pipeline artefact so that Apply uses the reviewed plan.
- Configured remote Terraform state in Azure Storage and included an alternative GitHub Actions workflow.

**Verified result:** A recorded Azure DevOps pipeline completed all three stages in 1 minute 23 seconds.

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/azure-devops-pipeline-success.png" alt="Successful Azure DevOps Validate, Plan and Apply pipeline" width="75%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/container-app-overview.png" alt="Azure Container App overview" width="45%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/azure-terraform-project/main/docs/screenshots/storage-rbac-assignment.png" alt="Azure Storage role-based access control assignment" width="45%" />
</p>

**Technologies:** Terraform, Microsoft Azure, Azure Container Apps, Azure Storage, Azure DevOps, GitHub Actions, RBAC.

The Azure subscription has expired, so the environment is no longer deployed. The Container Apps environment is not VNet-integrated, and the sample application does not yet read from Blob Storage.

### 2. AWS Terraform and Lambda Assessment

**Serverless processing, infrastructure as code and access control**

An AWS solution that processes JPEG images uploaded to Amazon S3. An S3 object creation event invokes a Python Lambda function, which removes EXIF metadata and saves the processed image to a second bucket.

**Engineering highlights**

- Provisioned 18 AWS resources with Terraform, including two S3 buckets, a Lambda function, IAM policies and event notifications.
- Implemented metadata removal without decoding or recompressing the image.
- Configured separate bucket permissions for two IAM users and a dedicated Lambda execution role.
- Added six pytest unit tests and GitHub Actions checks for testing, Terraform formatting and validation.
- Reduced measured Lambda processing time from approximately 3.9 seconds to 2.5 to 2.6 seconds by improving the scan-data parsing loop.

**Verified result:** Tested the deployed function with a 3 MB photograph, checked that camera, GPS and original date metadata had been removed, then destroyed all 18 resources.

**Technologies:** AWS, S3, Lambda, IAM, Python, Terraform, pytest, GitHub Actions.

### 3. Weather DataOps Pipeline

[View Repository](https://github.com/ArshaanSindhwani/Weather-DataOps-Pipeline)

An automated pipeline that collects weather data, stores current and historical readings, and presents the results through an interactive dashboard.

**Engineering highlights**

- Integrated the OpenWeather API for scheduled data collection.
- Stored current readings in JSON and appended historical readings to CSV.
- Built an Express API and Plotly dashboard for exploring weather data.
- Containerised the application with Docker and configured deployment to Render.
- Automated data collection, testing, version control and deployment triggers through GitHub Actions.

**Measured Docker improvements**

| Measure | Before | After |
|---|---:|---:|
| Image content size | 108 MB | 82.8 MB |
| Disk usage | 496 MB | 343 MB |
| Build time without cache | 22.5 seconds | 7.8 seconds |

These improvements came from excluding unnecessary files from the Docker build context and installing production dependencies only.

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/Weather-DataOps-Pipeline/main/screenshots/dashboard-overview.png" alt="Weather DataOps dashboard overview" width="80%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/Weather-DataOps-Pipeline/main/screenshots/temperature-chart.png" alt="Historical temperature trend visualisation" width="48%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/Weather-DataOps-Pipeline/main/screenshots/api-weather-endpoint.png" alt="Current weather API response" width="48%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/Weather-DataOps-Pipeline/main/screenshots/api-weather-log.png" alt="Historical weather log API response" width="70%" />
</p>

**Technologies:** JavaScript, Node.js, Express, OpenWeather API, JSON, CSV, Plotly.js, Docker, GitHub Actions, Render.

### 4. AgroSense

[View Repository](https://github.com/ArshaanSindhwani/AgroSense)

A mobile agriculture platform for recording field observations, mapping fields, viewing weather information and generating AI-assisted farming recommendations. Developed within a five-person Agile team at La Fosse Academy.

**Engineering highlights**

- Implemented local persistence using AsyncStorage and a connectivity-aware synchronisation queue.
- Integrated Firebase Authentication and Firestore for authentication and cloud data storage.
- Connected external weather, mapping and AI services.
- Added fallback handling for unavailable weather and map data.
- Contributed to debugging, dashboard behaviour, synchronisation documentation and technical presentation.

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/login.jpg" alt="AgroSense login screen" width="30%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/dashboard.jpg" alt="AgroSense farm and weather dashboard" width="30%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/fields.jpg" alt="AgroSense field management screen" width="30%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/observations.jpg" alt="AgroSense field observation recording" width="30%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/recommendations.jpg" alt="AgroSense AI-assisted recommendations" width="30%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/AgroSense/main/screenshots/offline-compatible.jpg" alt="AgroSense offline-compatible functionality" width="30%" />
</p>

**Technologies:** JavaScript, React Native, Expo, Firebase, Firestore, AsyncStorage, Gemini API, Open-Meteo, OpenStreetMap.

### 5. MovieApp

[View Repository](https://github.com/ArshaanSindhwani/MovieApp)

A collaborative movie tracking application with a JavaScript frontend, Express backend and PostgreSQL database. Users can manage watched films, record ratings and retrieve movie information from TMDB.

**Engineering highlights**

- Built backend functionality with Node.js and Express.
- Implemented JWT authentication and protected routes.
- Designed relational database tables, foreign keys and constraints.
- Integrated TMDB for movie details, posters and ratings.
- Developed a separate Flask recommendation endpoint using Google Gemini.
- Configured Docker Compose for the backend and resolved reported dependency vulnerabilities.

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/MovieApp/main/screenshots/login.png" alt="MovieApp login screen" width="45%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/MovieApp/main/screenshots/register.png" alt="MovieApp registration screen" width="45%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/MovieApp/main/screenshots/homepage.png" alt="MovieApp homepage" width="45%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/MovieApp/main/screenshots/my-list.png" alt="MovieApp personal film list" width="45%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/MovieApp/main/screenshots/add-movie.png" alt="MovieApp add movie screen" width="60%" />
</p>

**Technologies:** JavaScript, Node.js, Express, Python, Flask, PostgreSQL, JWT, TMDB API, Google Gemini, Docker.

### 6. EduFun

[View Repository](https://github.com/ArshaanSindhwani/EduFun)

An educational gaming platform with a REST API, PostgreSQL database and interactive learning challenges. Students can complete quizzes and review their scores and progress.

**Engineering highlights**

- Developed backend functionality using Express and an MVC structure.
- Implemented registration, login and JWT issuance.
- Integrated PostgreSQL for users, challenges, questions, answers and results.
- Wrote unit tests and API tests using Jest and Supertest.
- Replaced an empty integration test stub with five working API tests and improved test coverage reporting.

**Verified testing results**

| Metric | Result |
|---|---:|
| Backend tests passing | 37 |
| Test suites | 7 |
| Line coverage | 87.71% |
| API routes | 9 |
| Database tables | 9 |

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/EduFun/main/screenshots/login.png" alt="EduFun login screen" width="45%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/EduFun/main/screenshots/register.png" alt="EduFun registration screen" width="45%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/EduFun/main/screenshots/home.png" alt="EduFun learning dashboard" width="45%" />
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/EduFun/main/screenshots/game.png" alt="EduFun interactive educational challenge" width="45%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ArshaanSindhwani/EduFun/main/screenshots/results.png" alt="EduFun results and progress screen" width="70%" />
</p>

**Technologies:** JavaScript, Node.js, Express, PostgreSQL, bcrypt, JWT, Jest, Supertest.

---

## Experience

**Technology Trainee | La Fosse Academy**  
April 2026 to June 2026

Completed technical training across software engineering, cloud infrastructure, DevOps and data engineering. Built applications and deployment workflows using JavaScript, Node.js, PostgreSQL, AWS, Docker, Terraform and GitHub Actions.

**Associate Consultant | CPL Life Sciences**  
October 2023 to October 2025

Managed recruitment pipelines, maintained candidate data and built Excel and Power BI dashboards for KPI tracking. Developed experience in data quality, reporting and stakeholder communication.

**Senior Scientist | Cignpost Diagnostics**  
October 2021 to October 2022

Led a team of 10 in an ISO 15189 laboratory processing up to 10,000 diagnostic samples daily. Used root cause analysis and corrective and preventive actions to reduce repeat deviations by 25%.

**Earlier experience:** Laboratory Associate Practitioner at Prenetics and IT Engineer at iTech Services, including infrastructure support and migrations for enterprise clients.

For further employment details, see my [LinkedIn profile](https://www.linkedin.com/in/arshaan-sindhwani).

## Education

**MSc Genomic Medicine, Merit**  
University of Sheffield, 2020

**BSc Biomedical Sciences, First Class Honours**  
University of Roehampton, 2019  
IBMS-accredited degree.

## Engineering Focus

- **Application development:** REST APIs, relational databases, authentication and backend architecture.
- **Cloud infrastructure:** Terraform, AWS, Azure, identity and access management.
- **Automation:** GitHub Actions, Azure DevOps, scheduled pipelines and deployment workflows.
- **Testing and troubleshooting:** Automated tests, API testing, coverage reporting and investigation of failures.
- **Data engineering:** API ingestion, structured data storage, JSON, CSV and dashboard development.
- **Operational discipline:** Technical documentation, data quality, root cause analysis and experience in regulated environments.

## Contact

I am open to early-career opportunities in software engineering, backend development, data engineering, cloud engineering and platform engineering across London and beyond, including on-site, hybrid and remote positions.

<p align="center">
  <a href="https://www.linkedin.com/in/arshaan-sindhwani">LinkedIn</a> ·
  <a href="https://github.com/ArshaanSindhwani">GitHub</a>
</p>
