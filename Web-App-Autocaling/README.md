# Web App Autoscaling

Autoscaling ensures optimal performance by dynamically adjusting resources based on app traffic and metrics such as CPU usage, memory, or bandwidth. Below, you’ll find the steps I followed and the outcomes of the task, along with references to screenshots captured during the process.

---


### **Task 5: Configure and Test Autoscaling of the Azure Web App**
1. **Objective**: Configure autoscaling for the production slot of an Azure Web App and test its performance under load.
2. **Steps**:
   - Navigated to the Web App blade in the Azure portal.
   - Selected **Scale out (App Service plan)** under the **Settings** section.
	![Step 1](Screenshots/scale_out1.png)

   - Configured the following settings:
     - **Scaling Mode**: Automatic
     - **Maximum burst**: 2
	![Step 2](Screenshots/scale_out2.png)
   - Saved the autoscaling configuration.

3. **Load Testing**:
   - Selected **Diagnose and solve problems** from the left pane.
	![Step 3](Screenshots/scale_out3.png)

   - In the **Load Test your App** box, selected **Create Load Test**.
	![Step 4](Screenshots/scale_out4.png)

   - Created a new load test with the following steps:
     - Selected **+ Create**, provided a unique name for the load test, and clicked **Review + create** and **Create**.
	![Step 5](Screenshots/scale_out5.png)

     - Waited for the load test resource to deploy and navigated to the resource.
	![Step 6](Screenshots/scale_out6.png)
	![Step 7](Screenshots/scale_out7.png)

   - From the **Overview | Add HTTP requests** section:
	![Step 8](Screenshots/scale_out8.png)
	![Step 9](Screenshots/scale_out9.png)
	
     - Clicked **Create**.
     - On the **Test plan** tab, added a new HTTP request:
       - **URL**: Pasted the **Default domain URL** of the production slot (ensured proper format starting with `https://`).
     - Selected **Review + create** and clicked **Create**.
	![Step 10](Screenshots/scale_out10.png)
	![Step 11](Screenshots/scale_out11.png)

   - After creation, reviewed test results including:
     - **Virtual Users**: The number of simulated users accessing the app.
     - **Response Time**: Average time for the app to respond.
     - **Requests/sec**: Number of requests the app handled per second.
	
	![Step 13](Screenshots/scale_out13.png)
	![Step 14](Screenshots/scale_out14.png)
	![Step 14](Screenshots/scale_out14.png)
	![Step 16](Screenshots/scale_out16.png)

   - Stopped the test manually without waiting for completion to verify autoscaling behavior.

3. **Outcome**:
   - Successfully configured autoscaling and confirmed the app’s ability to scale based on load.
   - Load test results provided insights into performance metrics under stress.


 
