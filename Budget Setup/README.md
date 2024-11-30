# Azure Budget and Action Setup

This folder contains the steps and documentation for setting up both a **budget** and an **action group** in **Azure**. 
Although budgeting isn't strictly required for a **Free Azure Account**, I set it up as part of my **hands-on experience** to demonstrate my ability to manage costs and configure notifications for resource usage. This showcases my proficiency with Azure's **Cost Management** and **Alerting** features.

## Why Budget and Action for a Free Account?
- **Azure Free Account**: My **Azure Free Student Account** provides me with $100 in credits, so I won't incur charges unless I upgrade to a **Pay-As-You-Go** subscription. Although setting a budget is optional, I chose to implement it to gain experience with Azure's **Cost Management** tools and to demonstrate my skills for potential real-world scenarios.
- **Action Setup**: I configured an **action group** to receive notifications via **email** when certain budget thresholds are exceeded, ensuring that I can monitor my resource usage effectively.

## Steps for Budget Creation (Resource Group Scope)
1. **Log into Azure Portal**
   - Navigate to the **Subscriptions** section in the Azure portal.

2. **Create a New Budget at Resource Group Scope**
   - In the Azure portal, select your **subscription**
   - Under the **Cost Management** section, select **Budgets** and click **+ Add** to create a new budget.
   - Set the **budget name**, the **amount** (e.g., $50), and the **time period** (e.g., Monthly). 
   - Set the **scope** to **Resource Group**, and specify the resource group you want the budget to apply to.
   - Configure the **alert thresholds** (50%(forecasted), 100%, and 100%) to notify you when you approach or exceed the budget.

3. **Configure Alerts for the Budget**
   - I set up **email alerts** so I would be notified via email when the budget thresholds are exceeded.

## Action Group Setup (Notification Action)
1. **Create Action Group**
   - After setting the budget, I created an **action group** that will trigger notifications whenever my budget thresholds are reached.
   - I chose **email notifications** for the action to receive alerts.

2. **Email Notification Action**
   - I configured the action to send **email notifications** to my registered email address. This ensures that I can monitor usage directly in my inbox and take action to prevent exceeding the budget.

## Screenshots
Here are the screenshots showing the **budget creation** and **action group setup** in the Azure portal:

- **Budget Overview**:  
 
  
- **Action Group Setup**:  
