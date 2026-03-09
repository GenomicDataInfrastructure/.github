# Welcome to the Genomic Data Infrastructure (GDI)
## About the Project
The Genomic Data Infrastructure (GDI) is a European project, co-funded under the Digital Europe Programme, designed to realize the ambition of the 1+ Million Genomes (1+MG) initiative.

Our primary goal is to establish a federated, sustainable, and secure infrastructure to enable cross-border access to human genomic, phenotypic, and clinical data across Europe. By providing this infrastructure, we aim to unlock the potential of genomic data to drive breakthroughs in medical research, advance personalized healthcare, and inform public health policymaking.

## Deployed Environments
GDI operates on a federated model consisting of central (European-level) and local (node-level) components. Individual national nodes are responsible to deploy and integrate their services into the central services. The catalogue below lists the environments where end-users can use the central services.

| Environment | URL | Purpose |
| --- | --- | --- |
| Staging | https://portal.staging.gdi.lu/ | It can be used for demonstration and integration testing between local and central services. |
| Production | https://portal.gdi.lu/ | It is the production environment central services. |

## Navigating Our Repositories
Our organization is structured around several core components and themes. Here is a guide to our most critical repositories:

### 1. Architecture, Standards, and SOPs

| Repository | Description |
| --- | --- |
| [Reference Architecture](https://github.com/GenomicDataInfrastructure/oneplusmg-reference-architecture)  | Defines the federation-wide business capabilities, cross-border processes, and shared interoperability/security requirements. |
| [Standard Operating Procedures](https://github.com/GenomicDataInfrastructure/standard-operating-procedures) | The central hub for SOPs to standardize and harmonize operational procedures across all GDI nodes. |
| [API Specifications](https://github.com/GenomicDataInfrastructure/api-links) | A reference directory linking to specifications and documentation for all APIs used within the GDI ecosystem. |

### 2. The Starter Kit & Node Implementations

| Repository | Description |
| --- | --- |
| [Starterkit and service description](https://github.com/GenomicDataInfrastructure/starter-kit?tab=readme-ov-file#readme) | The main entry point. It contains a collection of software applications based on Global Alliance for Genomics and Health (GA4GH) standards (like Beacon, REMS, and htsget) to help national nodes deploy local infrastructure. |
| [Deployment Guide](https://github.com/GenomicDataInfrastructure/starter-kit/blob/main/deployment-guide.md) | The deployment guide for nodes. |

### 3. The GDI User Portal      
The User Portal serves as the primary interface for data discovery and access authorization across the federated network.

| Repository | Description |
| --- | --- |
| [Frontend](https://github.com/GenomicDataInfrastructure/gdi-userportal-frontend) | NextJS-based frontend interface. |
| [Access Management Service](https://github.com/GenomicDataInfrastructure/gdi-userportal-access-management-service) | Receives access requests and forwards them to the Data Authorities. |
| [Dataset Discovery Service](https://github.com/GenomicDataInfrastructure/gdi-userportal-dataset-discovery-service) | Integrates the User Portal with the Dataset Catalogue and Beacon Network. |
| [Dataset Catalogue / CKAN](https://github.com/GenomicDataInfrastructure/gdi-userportal-ckan-docker) | Dataset Catalogue of GDI, based on CKAN |
| [REMS Synchronizer](https://github.com/GenomicDataInfrastructure/gdi-userportal-rems-synchronizer) | Synchronizes the REMS database with the GDI Dataset Catalogue. |
| [Deployment](https://github.com/GenomicDataInfrastructure/gdi-userportal-deployment) | Example of how to deploy User Portal components using Docker Compose. |
| [CKAN extension for GDI User Portal](https://github.com/GenomicDataInfrastructure/gdi-userportal-ckanext-gdi-userportal) | CKAN extension for GDI User Portal, that implements the metadata model of GDI, based on HealthDCAT-AP. |
| [DCAT CKAN extension](https://github.com/GenomicDataInfrastructure/gdi-userportal-ckanext-dcat) | A fork of the DCAT CKAN extension, that implements new features for GDI. |
| [FAIR Data Point CKAN extension](https://github.com/GenomicDataInfrastructure/gdi-userportal-ckanext-fairdatapoint) | The CKAN extension implementation of the FAIR Data Point protocol, that adds new harvesting endpoints to CKAN. |
| [Dataset Series CKAN extension](https://github.com/GenomicDataInfrastructure/gdi-userportal-ckanext-dataset-series) | A fork of the dataset series CKAN extension, that implements new features for GDI. |

### 4. Development and Deployment Tracking
The development and deployment of GDI is tracked using GitHub Projects. Below, one can find links to the development and deployment boards.

| Board | Description |
| --- | --- |
| [Development](https://github.com/orgs/GenomicDataInfrastructure/projects/6/views/1) | Development tracking of GDI. |
| [Deployment](https://github.com/orgs/GenomicDataInfrastructure/projects/8/views/1) | Deployment tracking of GDI. |
