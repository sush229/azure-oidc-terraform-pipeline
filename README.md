# azure-oidc-terraform-pipeline
A zero-trust, secretless CI/CD pipeline deploying Azure infrastructure via Terraform, GitHub Actions, and Workload Identity Federation (OIDC).

This repository demonstrates a zero-trust, secretless CI/CD pipeline for deploying Azure infrastructure using Terraform, GitHub Actions, and OpenID Connect (OIDC).

Key Components:
The Main Terraform File (terraform/main.tf) provides:

Azure Provider Configuration: Sets up the Terraform provider for Azure Resource Manager (AzureRM) with version 4.0+
Basic Infrastructure as Code Template: Defines a reusable resource group that can be deployed to Azure
Parameterization: Uses variables for resource group name and location, making the configuration flexible and reusable
Primary Purpose:
The repository showcases how to:

Eliminate Secret Management: Uses Workload Identity Federation (OIDC) instead of storing secrets like connection strings or service principal credentials
Automate Azure Deployments: GitHub Actions workflows trigger automated infrastructure provisioning via Terraform
Implement Zero-Trust Security: Leverages OIDC for secure, token-based authentication between GitHub and Azure without persistent credentials
Infrastructure as Code: Manages Azure resources declaratively through Terraform's HCL language
Use Cases:
Learning: Understanding how to set up secretless authentication for cloud deployments
Template: A starting point for building more complex Azure infrastructure pipelines
Best Practices: Demonstrates modern CI/CD security patterns for infrastructure automation
The 100% HCL composition confirms this is a pure Terraform-based infrastructure project with no application code—it's purely focused on infrastructure provisioning and pipeline configuration.
