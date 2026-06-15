# Azure Data Factory ETL Pipeline: Superstore Analytics

## Overview
This repository contains the documentation and implementation details for an end-to-end cloud data pipeline built on Microsoft Azure. The project demonstrates core data engineering principles by extracting the Superstore sales dataset from a source storage container, validating its metadata, and securely loading it into a destination container using Azure Data Factory (ADF). 

This mini-project serves as a practical implementation of cloud infrastructure setup, role-based access control (RBAC), and automated data movement.

## Technology Stack
* **Cloud Platform:** Microsoft Azure
* **Orchestration:** Azure Data Factory (ADF)
* **Storage:** Azure Blob Storage (Locally-redundant storage)
* **Security & IAM:** System Assigned Managed Identity, Role-Based Access Control (RBAC)
* **Data Format:** CSV

## Architecture & Workflow

1. **Infrastructure Setup:** * Provisioned an Azure Resource Group to logically manage all project assets.
   * Created an Azure Storage Account with two distinct Blob containers: `source-data` and `destination-data`.
2. **Security & Authentication:**
   * Configured a System Assigned Managed Identity for the Azure Data Factory.
   * Granted the `Storage Blob Data Contributor` IAM role to the Data Factory, allowing secure, keyless access to the Storage Account.
3. **Pipeline Development:**
   * **Linked Services:** Established secure connections between ADF and Blob Storage.
   * **Datasets:** Defined schema and file path configurations for both the source CSV and the target destination.
   * **Activities:** * `Get Metadata`: Validated the presence and attributes of the source file.
     * `Copy Data`: Executed the movement of the Superstore dataset from the source container to the destination container upon successful metadata validation.

## Execution Results
The pipeline was successfully debugged and executed within the Azure Data Factory studio. The activities succeeded in sequentially validating the dataset parameters and copying the data securely across containers without manual intervention.

## Author
**Parth Gehlot**