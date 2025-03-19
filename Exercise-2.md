## Exercise 2: Reviewing the Deployed ALZ Foundation

### **Task 1: Exploring the Management Group (MG) Hierarchy and Subscriptions**  
### **Step 1: Validate the Created Management Groups**

1. In the [Azure Portal](https://portal.azure.com), search for **Management Groups** in the search bar and select it.  

1. Expand the **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>** under the Root Management Group nto verify the management groups like **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-decommissioned**, **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-landingzones**, 
**managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-platform**, and **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-sandboxes**.

1. Each of these management groups have different functions which are listed below
    - **Tenant Root Group** – The top-level management group that contains all subscriptions in the tenant.
    - **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>** – A parent management group organizing all child groups under the tenant.
    - **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-decommissioned** – Holds resources or subscriptions that are no longer in active use.
    - **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-landingzones** – Manages enterprise workloads and landing zones for production and development.
    - **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-platform** – Contains shared services like identity, networking, and management resources.
    - **managementgroup<inject key="DeploymentID" enableCopy="false"></inject>-sandboxes** – Isolates non-production environments for testing and experimentation.
 
1. Click on each **Management Group** and check **Subscriptions** assigned under them.

1. Verify that inherited policies from parent management groups are correctly applied. 
 
1. In the **Management Groups** page, select a management group (e.g., **Platform** or **LandingZones**). 

1. Navigate to the **Policy** section:  
   - Click on **Policy** in the left menu.  
   - Select **Assignments** to view policies applied at that level.  

1. Identify built-in Azure Policies.  

1. Click on **Compliance** to check if the applied policies are compliant.

## **Task 2: Validating Azure Policies and Security Controls**  

1. In the **Azure Portal**, search for **Policy** in the search bar.  
2. Click on **Policy** under **Governance**.  
3. In the **Policy | Assignments** tab:  
   - Review policy assignments applied to subscriptions and management groups.  
   - Check the **Scope** (i.e., where the policy is enforced).  

1. Go to **Policy → Compliance**.  
2. Review the **Security Benchmark compliance** (e.g., **Azure Security Benchmark** policy).  
3. Identify non-compliant policies and click on them to view affected resources.  
4. For any **non-compliant policy**, take note of:  
   - The reason for non-compliance.  
   - Recommended remediation steps.  

1. Check how policies are enforced across multiple subscriptions:  
   - In **Policy → Assignments**, filter by subscription.  
   - Identify any missing policy assignments at the subscription level. 

2. Verify if **Deny, Audit, or Enforce** policies are correctly applied to prevent non-compliance. 
 
3. If needed, assign a new policy:  
   - Click **Assign Policy** → Choose a built-in or custom policy.  
   - Select the **Scope** (Management Group or Subscription).  
   - Choose **Effect** (Audit, Deny, Append, Modify).  
   - Click **Assign**.  