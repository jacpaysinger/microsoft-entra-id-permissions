# Microsoft Entra ID Permissions

## Project Overview
This lab explores role-based access control (RBAC) in Microsoft Entra ID by assigning different permission levels and observing their effects. By completing this lab, I aim to gain a deeper understanding of how different roles impact access to resources at various levels: tenant, subscription, and resource group.

## Objectives

- Understand and implement **Role-Based Access Control (RBAC)** in Microsoft Entra ID.
- Configure and observe effects of **Tenant-Level Global Reader**, **Subscription-Level Reader**, and **Resource Group Contributor** roles.
- Identify the scope and limitations of each assigned role within **Microsoft Entra ID**.
- Analyze and document access permissions at **tenant, subscription, and resource group levels**.

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
<img width="1618" alt="Screenshot 2025-02-23 at 10 24 20 PM" src="https://github.com/user-attachments/assets/82b6d833-2c2e-41f8-be99-81d0a220c7ec" />
<img width="1618" alt="Screenshot 2025-02-23 at 10 40 11 PM" src="https://github.com/user-attachments/assets/52f7596c-1ed5-4b3d-8de4-f109edca5329" />


---

### 2. Configure and Observe Subscription Reader
#### Steps:
1. In the main browser, create another user in Microsoft Entra ID with the username `subreaderpaysinger`.
2. Assign the **Subscription-Level Reader** role to `subreaderpaysinger`.
3. Open a new browser or incognito window and log in as `subreaderpaysinger`.
4. Observe the permissions granted by the **Subscription Reader** role.
<img width="1618" alt="Screenshot 2025-02-23 at 10 47 37 PM" src="https://github.com/user-attachments/assets/86916782-275c-42a6-bc2f-ebef8df248eb" />
<img width="1618" alt="Screenshot 2025-02-23 at 10 50 45 PM" src="https://github.com/user-attachments/assets/9592272d-d13a-4c26-9b0c-4f109c06b48f" />
<img width="1618" alt="Screenshot 2025-02-23 at 10 56 19 PM" src="https://github.com/user-attachments/assets/96036b2b-4b46-4346-b6d4-add282c20da4" />


---

### 3. Configure and Observe Resource Group Contributor
#### Steps:
1. In the main browser, create another user in Microsoft Entra ID with the username `rgcontributorjp`.
2. Create a new resource group named **Permissions-Tester**.
3. Assign the **Resource Group Contributor** role to `rgcontributorjp` at the **Permissions-Tester** resource group level.
4. Open a new browser or incognito window and log in as `rgcontributorjp`.
5. Observe the results of being a **Resource Group Contributor**.
6. Observe that `rgcontributorjp` has no permissions beyond the assigned resource group.
<img width="1618" alt="Screenshot 2025-02-23 at 11 13 45 PM" src="https://github.com/user-attachments/assets/aeb6f62f-e7d0-4228-94d7-090c9900b021" />
<img width="1618" alt="Screenshot 2025-02-23 at 11 14 12 PM" src="https://github.com/user-attachments/assets/917c764e-404a-42ec-b4bc-69380650a430" />
<img width="1603" alt="Screenshot 2025-02-23 at 11 16 34 PM" src="https://github.com/user-attachments/assets/bc7631c1-7b45-4ba0-93f8-a4dfa225fd37" />
<img width="1603" alt="Screenshot 2025-02-23 at 11 20 09 PM" src="https://github.com/user-attachments/assets/057bd400-0b79-4349-8bd3-534c407837e5" />
<img width="1617" alt="Screenshot 2025-02-23 at 11 23 10 PM" src="https://github.com/user-attachments/assets/c8548751-815e-486f-b5a1-9e0a60130312" />




## Takeaways
This lab demonstrated the effect of different permission levels in Microsoft Entra ID. By assigning and testing **Global Reader, Subscription Reader, and Resource Group Contributor** roles, I was able to see firsthand how RBAC controls access at different levels within an Azure environment. Understanding these roles is crucial for properly managing permissions and securing cloud resources.
