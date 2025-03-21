## Exercise 3: Adding a Subscription in the App Landing Zone MG
### Task 1: Adding a Subscription to App LZ Management Group

1. Sign in to the Azure Portal at https://portal.azure.com and search for **Management Groups** in the top search bar.

1. Locate the top-level Tenant Root Group and find the Platform and Landing Zones Management Groups.

1. Click on the App Landing Zone Management Group to view its current details and structure.

1. Review any existing subscriptions already in the App Landing Zone Management Group and note the inherited policies.

1. From the Management Groups page, click on the App Landing Zone Management Group.

1. Click **Add** or **Add subscription** button and **Select** the subscription you want to add from the dropdown list.

1. Click **Save** to add the subscription to the Management Group and wait for the operation to complete.

1. Refresh the Management Group view to confirm that the subscription now appears under the App Landing Zone Management Group.

1. Navigate to the newly added subscription by searching for **Subscriptions** in the search bar and selecting your subscription.

1. Select **Access control (IAM)** from the left menu and click **+ Add** then **Add role assignment.**

1. Choose the appropriate role such as **Contributor** for application teams, **Security Reader** for security teams, or **Network Contributor** for operations teams.

1. Select the appropriate user, group, or service principal to assign the role to and click **Review + assign** to finalize.

1. Verify the RBAC assignments by checking the **Role assignments** tab in the Access control (IAM) page.

### Task 2: Governance and Security for the New Subscription

1. From your subscription page, select **Policy** from the left menu and click **+ Assign policy** to create a new policy assignment.

1. Search for and select the **Require a tag** policy, then enter the required tag name like **Department** or **Environment** in the Parameters field.

1. Enable **Create a remediation task** if you want to apply the policy to existing resources, then click **Review + create** and **Create.**

1. Navigate to **Resource groups** from your subscription page and create new resource groups named according to your convention like **rg-app-prod-001.**

1. Verify policy compliance by selecting **Policy** from the subscription menu and clicking on **Compliance** to view the status.

1. From your subscription page, select **Security** from the left menu, click on **Security policy,** and assign the Azure Security Benchmark policy.

1. Navigate to **Microsoft Defender for Cloud** from your subscription page, click **Environment settings,** select your subscription, and enable the recommended Defender plans.

1. Return to the **Policy** page and assign additional security policies like **Audit VMs that do not use managed disks** or **Storage accounts should restrict network access.**

1. Review security recommendations by selecting **Microsoft Defender for Cloud** and clicking **Recommendations** to see the list for your subscription.