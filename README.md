# Microsoft Entra ID Permissions

## Project Overview
This lab explores role-based access control (RBAC) in Microsoft Entra ID by assigning different permission levels and observing their effects. By completing this lab, I aim to gain a deeper understanding of how different roles impact access to resources at various levels: tenant, subscription, and resource group.

## Technologies Used
- Microsoft Entra ID
- Microsoft Azure Portal
- Azure Subscription
- Resource Groups (Azure)
- Role-Based Access Control (RBAC)

## Lab Steps

### 1. Configure and Observe Tenant-Level Global Reader
#### Steps:
1. Create a user in Microsoft Entra ID with the username `globalreaderjac`.
2. Assign the **Tenant-Level Global Reader** role to `globalreaderjac`.
3. Open a new browser or incognito window and log in as `globalreaderjac`.
4. Observe the permissions granted by the **Global Reader** role at the tenant level

---

### 2. Configure and Observe Subscription Reader
#### Steps:
1. In the main browser, create another user in Microsoft Entra ID with the username `subreaderpaysinger`.
2. Assign the **Subscription-Level Reader** role to `subreaderpaysinger`.
3. Open a new browser or incognito window and log in as `subreaderpaysinger`.
4. Observe the permissions granted by the **Subscription Reader** role.

---

### 3. Configure and Observe Resource Group Contributor
#### Steps:
1. In the main browser, create another user in Microsoft Entra ID with the username `rgcontributorjp`.
2. Create a new resource group named **Permissions-Tester**.
3. Assign the **Resource Group Contributor** role to `rgcontributorjp` at the **Permissions-Tester** resource group level.
4. For an additional test, assign `rgcontributorjp` the **Contributor** role for an existing resource group named **RG-Cyber-Lab**.
5. Open a new browser or incognito window and log in as `rgcontributorjp`.
6. Observe the results of being a **Resource Group Contributor**.
7. Observe that `rgcontributorjp` has no permissions beyond the assigned resource group.


## Takeaways
This lab demonstrated the effect of different permission levels in Microsoft Entra ID. By assigning and testing **Global Reader, Subscription Reader, and Resource Group Contributor** roles, I was able to see firsthand how RBAC controls access at different levels within an Azure environment. Understanding these roles is crucial for properly managing permissions and securing cloud resources.
