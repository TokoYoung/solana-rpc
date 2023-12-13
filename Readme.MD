# IAC for ETL-Core infrastructure 

## Overview
This repository contains the necessary infrastructure as code to set up a Solana RPC node and RabbitMQ for an ETL (Extract, Transform, Load) project. It is designed to provision and configure a secure environment on Google Cloud Platform (GCP) for running a Solana node, along with RabbitMQ for efficient data handling and processing.

## Structure
- `init/`: Contains Terraform scripts for enabling required APIs in the GCP environment.
- `main/`: Houses the main Terraform configuration for provisioning the GCP environment. This includes setting up firewalls, VPC, and all prerequisites to securely run a Solana node.
- `scripts/`: Includes shell scripts for configuring disks, downloading, and running the Solana RPC node, as well as setting up RabbitMQ configuration automatically.

## Usage
1. **API Initialization**: 
   - Navigate to the `init/` directory.
   - Run the Terraform scripts to enable the necessary APIs in your GCP project.

2. **Environment Provisioning**:
   - Move to the `main/` directory.
   - Execute the Terraform scripts to provision the GCP environment, including firewalls, VPC, and other required infrastructure components.

3. **Solana Node and RabbitMQ Configuration**:
   - After provisioning the infrastructure, download and run the scripts located in the `scripts/` directory on the Solana node and RabbitMQ server.
   - These scripts will handle disk configuration, Solana RPC node setup, and RabbitMQ configuration.

## Prerequisites
- A Google Cloud Platform account.
- Terraform installed on your local machine.
- Basic knowledge of GCP, Terraform, and shell scripting.
