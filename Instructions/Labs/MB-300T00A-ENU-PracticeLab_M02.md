---
lab:
    title: 'MB-300.0 Practice Lab: Module 02'
    module: 'Module 02'
---

# Exercise 1: Create a task recording

In this exercise, you will:
- Create a recording using Task recorder.

- Save the recording.

- Edit a recording.

## Create a recording

1. Open Finance and Operations and sign in. It's a good practice to refresh the browser before each new recording. This creates a new user session and restarts Task recorder, providing the most stable recording experience.

2. Select the company that you want to use while recording. If this is your first-time using Task recorder, you can follow along as this exercise creates a sample recording based on a Fleet Management business process. You will need to load the Fleet demo data to follow along.

3. In the Navigation Pane, go to **Modules &gt; Fleet Management &gt; Setup &gt; Fleet Setup.**

4. Under Data Setup tab, Click **Create** sample data.

5. When the data is finished loading, click **Close**.

6. Go to the **Dashboard** by clicking **Finance and Operations** in the navigation bar.

7. Go to **Settings &gt; Task recorder**.  
   ![Settings is the gear in the top right and under it you will find task recorder](media/mb-300-t-000-a-enu-practicelab-m-002-01.png)

8. The **Task recorder** pane opens. You can click the "**X**" in the upper-right corner to close the **Task recorder** pane before beginning a new recording. The pane can be reopened by following the previous steps.

9. Click **Create a new recording**.

10. Enter a name for the recording and click **Start**. Recording begins the moment **Start** is clicked. For the Fleet example in this exercise, you'll use the name "Create a new rental reservation."

11. During recording, clicking the "**X**" in the upper-right corner will hide the pane without stopping the recording. The pane can be re-opened by clicking the **Task recorder** menu button that appears at the top of the screen. This icon only appears while recording is in progress.

12. The **Task recorder** enters **Recording Mode**. The pane now shows information and controls related to the process of recording.

13. In the **Task recorder** pane, click **Start sub-task**.

14. Set **Name** to "Create a new rental customer". Leave the **Comment** field blank.

15. Click **OK**.

16. The task is added to the **Steps list**.

17. In the navigation pane, go to **Dashboard &gt; Fleet Management &gt; Reservation Management**.

18. Go to **All customers** under the **Summary** tab.

19. In the Action Pane, click **New**.

20. Enter a first and last name for the customer.


## Save a recording
1. Click **Save**.

2. In the **Task recorder** pane, click **End task**.

3. To save the recording to your PC, select **Save to this PC**. Choose a location and save the file.

4. To save the recording to Lifecycle Services, select **Save to Lifecycle Services**. Note that you must have a BPM library in your LCS project.

5. To save the recording as a Word document, select **Export as a Word document**.

6. To save as a developer recording, select **Save as developer recording**.

7. Click **Return to main menu**.


## Edit recording

1. Click **Edit Recording**.

2. Click **Open from this PC** and click **Browse** to load a recording from the location where you saved the file. The extension of this file ends with (.axtr).

3. Click **Start** and Task recorder begins recording in Maintenance mode.

4. Here you can insert, delete, and move steps with a task.

5. Click **Done editing** to finish editing.

6. To save the recording to your PC select **Save to this PC**. Select a location and save the file.

7. Click **Return to main menu**.



# Exercise 2: Create a business process model

### Scenario

You want to import a global business process library to your Lifecycle Services (LCS) project and modify the library to introduce new processes for order to cash, procure to pay, and core financials. To do this, you must:


- Copy a business process library.

- Create your own business process library.


## Copy a business process library

1. Go to the LCS portal ([https://lcs.dynamics.com/v2](https://lcs.dynamics.com/v2/?azure-portal=true) ) and sign in to your Finance and Operations LCS project using your alias.

2. Click on your project that you created in the cloud environment that has been deployed on your Azure Pass subscription.

3. On the **Project details** page, go to the **More tools** section, and click the **Business Process** tile, or use the menu icon and select “Business process modeler”. **NOTE** Depending on the type of LCS project, the **Business process modeler** menu can be accessed either from the Tools section (partner oriented) or from the menu icon.

4. Click **View this page in the updated BPM experience**.

5. Click the ellipsis (…) for the **(March 2018 - All languages) APQC Unified Library for Microsoft Dynamics 365 for Finance and Operations (Cross industry)** library and click Copy.

6. Rename the library and **Create**.

7. Your BPM library will be available in the **Project libraries** section, ready to be used in your LCS project.

8. Select your new library.

9. Review available processes.


## Create your own business process library

1. Click **New Library**.

2. Assign a name and click **Create**

3. Click your new library tile.

4. Select **Sample Core Business process**, and then click **Edit Mode** to make a change to the library.

5. In the right panel, change the name of the process to **Order to Cash**, click **Save**.

6. Click **Add Process** and select **As Sibling**. Click **Edit Mode** and change the name to ‘Procure to Pay’.

7. Repeat the previous step for ‘Core Financials’ and ‘Procure to Pay’.

8. Select **Order to Cash** and add a child-level process.

9. Click **Add Process As Child** > **Edit Mode** and change the name to “Free Text Invoice”, and then click **Save**.

10. Add the next process under **Order to Cash** for ‘Receipt Journal’.

11. You can change the sequence by selecting the option to move process.

12. Repeat the previous steps to add child processes to the other process as follows:

| **Process**| **Child process** |
| - | - |
| Order to Cash| Receipt journal, Free Text invoice |
| Procure to Pay| Purchase order, Vendor invoice, Vendor payment |
| Core Financials| General journal, Run Financial reports, Period end |
 

# Exercise 3: Create a support incident

### Scenario

You will use the project environment that you created on the Azure subscription and log a support incident directly from Finance and Operations. You will be able to view the incident in Lifecycle Services (LCS) and Azure DevOps (also known as Visual Studio Team Services or VSTS), and view the associated environment health data.


## Connect the environment to Lifecycle Services

1. From the LCS portal ([https://lcs.dynamics.com/v2](https://lcs.dynamics.com/v2/?azure-portal=true) ), go to the details of your environment and start the environment if it is not already started.

2. Sign in on to Finance and Operations. Go to **System administration &gt; Setup &gt; System parameters**.

3. Go to the **Help** tab. You may get a notification to connect to Lifecycle Services.

4. Click the link in the message, **Click here to connect to Lifecycle services**. In a new tab, a message appears indicating **Success**.

5. Return to the previous tab and click **OK** in the confirmation message.

6. On the **Support contact** tab, note that the LCS project used in this workshop is selected.

7. Click **Save**.


## Create a support incident

1. Sign in to Finance and Operations

2. Click the ? icon in the upper-right corner and select **Support**.

3. In the lower-right corner, click **Create**.

4. Enter a value in the **Issue** field.

5. Enter a value in the **Description** field.

6. Enter a date in the **Time when issue occurred** field.

7. Answer if this issue stopping you from working.

8. Answer if this issue has a potential to create a company-wide work stoppage.

9. Alternatively, you can attach a task recording.

10. Answer if you want to share your email address. This must be set to Yes to allow you to submit an incident.

11. Click **Submit**.

12. You can now click **Close**.


## View your support incident in LCS

1. Sign in to LCS and open your project.

2. Select **Support** from the menu.

3. This list shows all the active issues logged within your project. From this screen you can add new issues, submit issues to Microsoft, or use Issue search.

4. Click incident title for your incident to open the Azure DevOps work item. Azure DevOps can be used to manage the assignment, status, and attachments of a support incident.

5. Scroll down to review the **Discussion** attached to the incident.
