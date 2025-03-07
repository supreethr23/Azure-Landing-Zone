# Azure Landing Zones

## Exercise 1: Introduction to Azure Landing Zone.

### Task 1: Understanding Azure Landing Zone (ALZ) Concepts 

An Azure Landing Zone (ALZ) is a structured environment in Azure that follows best practices t     - support application migration, modernization, and scalability. It organizes resources int     - Application Landing Zones (for hosting workloads) and Platform Landing Zones (for shared services like security, networking, and monitoring). The Enterprise-Scale ALZ, based on the Microsoft Cloud Adoption Framework (CAF), provides strong governance, security, and scalability.

- **Key Features**

  - Modular & Scalable → Supports multiple teams and workloads.

  - Secure by Design → Implements RBAC, Azure Policies, and Network Security.

  - Management Groups → Organizes subscriptions for better governance.

  - Compliance & Automation → Enforces policies and governance frameworks.

- **Architecture Overview**

  1. Management Groups & Subscriptions

     - Organizes workloads int     - categories:

        - Identity → Azure AD, PIM.
        - Connectivity → Networking, Firewalls.
        - Landing Zones → Workloads & Applications.

  2. Networking (Hub-Spoke Model)

        - Hub → Centralized security & networking (Firewall, ExpressRoute).
        - Spokes → Isolated environments for applications and workloads.

  3. Security & Governance

        - Azure Policies → Enforce compliance (e.g., restrict VM sizes, ensure encryption, enable Defender for Cloud).
        - Defender for Cloud → Monitors security risks and threats.

- **Role of Management Groups, Policies, and Subscriptions**

  1. Management Groups (MGs)

     - Organize subscriptions hierarchically for better governance.
     - Inherit policies and RBAC roles.

  2. Azure Policies

     - Enforce security, compliance, and governance.

     - Examples:

        - Restricting VM locations.
        - Enforcing tagging for cost management.
        - Enabling Defender for Cloud.

  3. Subscriptions

     - Used for billing, security, and workload separation.

     - Best practices include separate subscriptions for:

        - Landing Zones (Workloads).
        - Connectivity (Networking, ExpressRoute).
        - Identity & Management.

- **Governance and Automation Benefits**

  1. Governance Benefits

     - Centralized security and compliance.

     - Enforces standardized architecture.

     - Supports cost management and monitoring.

  2. Automation Benefits

     - Enables scalable and repeatable deployments.

     - Reduces manual errors using Infrastructure as Code (IaC).

     - Supports CI/CD for infrastructure to enhance efficiency.
