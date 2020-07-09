---
lab:
    title: 'MB-300.0 Practice Lab: Module 08'
    module: 'Module 08'
---

# Exercise 1: Create a new user and assign a security role


The HR department at USMF has requested access to Finance and Operations for a new employee who was hired as an accounts payable clerk.

You need to create a new user ID for the employee in Finance and Operations. After that, you need to assign the default company to USMF and then associate the account to the accounts payable clerk role.

1. Go to **System administration &gt; Users &gt; Users**.

2. Select **New**.

3. In the **User ID** field, enter a unique identifier for the user. A **user ID** is required.

4. In the **User name** field, enter the user's name.

5. In the **Domain** field, enter the user's domain.

6. In the **Alias** field, enter the user's alias.

7. In the **Company** field, click the drop-down button to open the lookup.

8. In the list, select **USMF**.

9. Click **Assign roles**.

10. In the list, find and select “accounts payable clerk.”

11. Click **OK**.

12. Click **Save**.


 

 

# Exercise 2: Import a user and assign a security role


The HR department at USMF has requested access to Finance and Operations for a new employee who has been hired as an accounts receivable clerk. The Azure Active Directory user account has already been created as part of the onboarding process.

You need to import a new employee into Finance and Operations. After that you need to assign USMF as the default company and then associate the account to the accounts receivable clerk role.

1. Go to **System administration &gt; Users &gt; Users**.

2. Click **Import users**.

3. From the list of aliases, select the alias that you want to import.

4. Click **Import users**.

5. Click **Close**.

6. On the **Users** list page, verify that the new user has been imported successfully.

7. Click the **User ID** link.

8. Click **Assign roles**.

9. In the list, find and select accounts receivable clerk.

10. Click **OK**.

11. Click **Save**.


 

 

# Exercise 3: Import users in bulk as a batch job


The HR department at USMF is hiring new employees for different roles. The Azure Active Directory user accounts will be created as part of the onboarding process. You must import multiple users from Azure Active Directory into Finance and Operations.

1. Go to **System administration &gt; Users &gt; Users**.

2. Click **Batch import**.

3. Expand the **Run in the background** section.

4. Select **Yes** in the **Batch processing** field.

5. In the **Task description** field, type a value.

6. In the **Batch group** field, enter or select a value.

7. Select **Yes** in the **Private** field.

8. Select **Yes** in the **Critical** **Job** field.

9. In the **Monitoring** **category** field, select an option.

10. Click **OK**.

11. After the batch job is completed, all new users from Azure Active Directory will be imported to Finance and Operations.


 

 

# Exercise 4: Assign users to security roles dynamically


The HR department at USMF has requested to dynamically assign users to the accounting supervisor role based on rules defined by the HR department. You need to associate the accounting supervisor role to the rules defined by the HR department for the selected employees.

1. Go to **System administration &gt; Security &gt; Assign users to roles**.

2. In the tree, select **Accounting supervisor**.

3. Click **Add rule** to open the drop-down menu.

4. In the list, find and select a query rule.

5. In the list, click the link in the selected row.

6. Click **Edit query**. You can change the query if needed.

7. Click **OK**.

8. Close the page.


 

 

# Exercise 5: Exclude users from a role assignment


The HR department at USMF has an employee who is changing their role. You need to exclude the accounts receivable clerk role for the employee in Finance and Operations

1. Go to **System administration &gt; Security &gt; Assign users to roles**.

2. In the tree, select **Accounts receivable clerk**.

3. Click **Manually assign / exclude users**.

4. In the list, select a user.

5. Click **Exclude from role** to exclude the selected users from the role.

6. To remove exclusions, select the users that you want to remove exclusions for, and then click **Reset status**.


 

 

# Exercise 6: Set up segregation of duties


The HR department at USMF has requested a rule for segregation of duties for the **Access benefits** workspace and the **Approve production** journal. You need to create this rule in Finance and Operations

The following procedure shows how to create a rule. You must be a system administrator to complete the procedure. The demo data company used to create this procedure is DAT.

1. Go to **System administration &gt; Security &gt; Segregation of duties &gt; Segregation of duties rules**.

2. Click **New**.

3. In the **Name** field, enter a name for the rule.

4. In the **First duty** field, click the drop-down button to open the lookup.

5. In the list, find and select the first duty that is controlled by the rule.

6. In the list, click the link in the selected row.

7. In the **Second duty** field, click the drop-down button to open the lookup.

8. In the list, find and select the second duty that is controlled by the rule.

9. In the list, click the link in the selected row.

10. In the **Severity** field, select the severity of the risk that occurs when the same user or role performs both duties.

11. In the **Security risk** field, enter a description of the security risk.

12. In the **Security mitigation** field, type a value.

13. Enter a description of the actions that you take to mitigate the security risk.  
‎‎For example, you can mitigate the risk by conducting more detailed reviews of the process, by conducting a monthly managerial review, or by sharing resources with other departments.

14. Click **Save**.


 

 

# Exercise 7: Work with batch jobs and add an alert


You’ve been asked to work with some batch jobs and alerts. To do this, you must perform these tasks:

- Create a batch job.

- Create a recurrence.

- Add alerts.

- Copy a batch job.

- Enable the batch job.

- Set up active periods for a batch job.

- Assign active periods to a batch job.

- Assign the Batch manager role to a user.


## Create a batch job

1. Go to **System administration &gt; Inquiries &gt; Batch jobs.**

2. Click **New.**

3. In the **Job description** field, type a value.

4. In the **Scheduled start date/time** field, enter a date and time.

5. Click **Save.**


## Create a recurrence

1. On the **Action Pane**, click **Batch job.**

2. Click **Recurrence** and use the options to enter a range and pattern for the recurrence.

3. Click **OK**.


## Add alerts

1. On the **Action Pane**, click **Batch job**.

2. Click **Alerts**. Indicate if you want alert messages sent when the batch job ends, has an error, or is canceled. Then specify if you want the alerts to be displayed as pop-up messages.

3. Click **OK**.


## Copy a batch job

1. Click **System administration** > **Inquiries** > **Batch jobs**.

2. Select the job that you want to copy, and on the **Action Pane**, click **Batch Job** > **Copy batch job**.

3. Enter or add any changes. If you set **View tasks** to **Yes**, when you click **OK** you will go directly to the **Batch tasks** page for the copied job.


The copied batch job will be created with a **Withhold** status, so you will need to enable it. The **Run by** user can also be set to give this user the privilege to run the job without being a System administrator.


## Enable the batch job

1. On the **Batch job** page, on the Action Pane, click **Batch job** > **Change status**.

2. Select the **Waiting** status, and then click **OK**.


## Set up active periods for batch jobs

1. Go to **System administration** > **Setup** > **Active periods for batch jobs**.

2. Enter the name of the batch job and specify start and end dates that the batch job is active.

3. Click **Save**.


## Assign active periods to batch jobs

1. Go to **System administration** > **Inquiries** > **Batch jobs**.

2. Select the batch job that you want to assign a **Period to** and click **Edit**.

3. In the **Active period** field, select the active period that you want to assign, and then click **Save**.


## Assign the Batch manager role to a user

1. Click **System administration** > **Security** > **Assign users to roles**.

2. Click **Batch Job Manager**, and on the left pane, click **Manually assign/exclude user**.

3. Select a user from the list, and then click **Assign to role**.

4. Close the page.


 
