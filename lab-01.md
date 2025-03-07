Azure Landing Zones

Exercise 1: Introduction to Azure Landing Zone and Deployment Options

Task 1: Understanding Azure Landing Zone (ALZ) Concepts An Azure Landing Zone (ALZ) is a structured environment in Azure that follows best practices to support application migration, modernization, and scalability. It organizes resources into Application Landing Zones (for hosting workloads) and Platform Landing Zones (for shared services like security, networking, and monitoring). The Enterprise-Scale ALZ, based on the Microsoft Cloud Adoption Framework (CAF), provides strong governance, security, and scalability.

Key Features

1. Modular & Scalable → Supports multiple teams and workloads.

2. Secure by Design → Implements RBAC, Azure Policies, and Network Security.

3. Management Groups → Organizes subscriptions for better governance.

4. Compliance & Automation → Enforces policies and governance frameworks.

Architecture Overview

1. Management Groups & Subscriptions

o Organizes workloads into categories:

§ Identity → Azure AD, PIM.

§ Connectivity → Networking, Firewalls.

§ Landing Zones → Workloads & Applications.

2. Networking (Hub-Spoke Model)

o Hub → Centralized security & networking (Firewall, ExpressRoute).

o Spokes → Isolated environments for applications and workloads.

3. Security & Governance

o Azure Policies → Enforce compliance (e.g., restrict VM sizes, ensure encryption, enable Defender for Cloud).

o Defender for Cloud → Monitors security risks and threats.

Role of Management Groups, Policies, and Subscriptions

1. Management Groups (MGs)

o Organize subscriptions hierarchically for better governance.

o Inherit policies and RBAC roles.

2. Azure Policies

o Enforce security, compliance, and governance.

o Examples:

§ Restricting VM locations.

§ Enforcing tagging for cost management.

§ Enabling Defender for Cloud.

3. Subscriptions

o Used for billing, security, and workload separation.

o Best practices include separate subscriptions for:

§ Landing Zones (Workloads).

§ Connectivity (Networking, ExpressRoute).

§ Identity & Management.

Governance and Automation Benefits

1. Governance Benefits

o Centralized security and compliance.

o Enforces standardized architecture.

o Supports cost management and monitoring.

2. Automation Benefits

o Enables scalable and repeatable deployments.

o Reduces manual errors using Infrastructure as Code (IaC).

o Supports CI/CD for infrastructure to enhance efficiency.
