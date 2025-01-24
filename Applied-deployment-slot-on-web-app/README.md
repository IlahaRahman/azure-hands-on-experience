Deployment slots are a powerful feature of Azure App Services that enable seamless testing, staging, and production workflows. Below, you’ll find the steps I followed and the outcomes of my tasks, along with references to screenshots captured during the process.

---


### **Task 2: Create and Configure a Deployment Slot**
1. **Objective**: Create a staging deployment slot for testing changes before going live.
2. **Steps**:
   - Opened the Web App blade in the Azure portal.
   - On the Web App **Overview** blade, clicked on the **Default domain** link to view the initial app screen.

	![Step 1](Screenshots/deployment_slot1.png)
     - Observed the default "Your App Service app is up and running" message in the browser.

	![Step 2](Screenshots/deployment_slot2.png)
   - Returned to the Azure portal and clicked **Deployment slots** under the Deployment section.

	![Step 3](Screenshots/deployment_slot3.png)
   - **Upgraded the Web App to the Premium tier to enable deployment slots.**

	![Step 4](Screenshots/deployment_slot4.png)
	![Step 5](Screenshots/deployment_slot5.png)

   - Selected **Add slot** with the following settings:
     - **Name**: `staging`
     - **Clone settings from**: `Do not clone settings`
   - Verified the staging slot was created with a unique URL.
	![Step 6](Screenshots/deployment_slot6.png)

3. **Outcome**: Successfully created a staging slot for pre-production testing.

---

### **Task 3: Configure Web App Deployment Settings**
1. **Objective**: Configure the deployment settings to enable continuous deployment from an external Git repository.
2. **Steps**:
   - Navigated to the **staging slot** blade.

	![Step 7](Screenshots/deployment_slot7.png)
   - Accessed **Deployment Center** > **Settings**.
   - Configured the following:
     - **Source**: External Git

	![Step 8](Screenshots/deployment_slot8.png)
     - **Repository URL**: `https://github.com/Azure-Samples/php-docs-hello-world`
     - **Branch**: `master`

	![Step 9](Screenshots/deployment_slot9.png)
   - Saved the settings and verified deployment in the staging slot.

	![Step 10	](Screenshots/deployment_slot10.png)

   - Opened the staging slot's **Default domain** URL to confirm the "Hello World!" application was deployed.
	![Step 11](Screenshots/deployment_slot11.png)
3. **Outcome**: Continuous deployment was successfully configured for the staging slot.

---

### **Task 4: Swap Deployment Slots**
1. **Objective**: Swap the staging slot with the production slot to make the tested code live.
2. **Steps**:
   - Navigated to the **Deployment slots** blade.
   - Selected **Swap** to exchange the `staging` and `production` slots.
	![Step 12](Screenshots/deployment_slot12.png)
	![Step 13](Screenshots/deployment_slot13.png)

   - Reviewed and confirmed the default settings before starting the swap.
   - Verified the production slot displayed the "Hello World!" page using the **Default domain** URL.
	![Step 14](Screenshots/deployment_slot14.png)

2. **Outcome**: Successfully swapped the staging slot with the production slot.



