Exercise 2: Prepare, enable, and use Business document management
-----------------------------------------------------------------

**Scenario**: you need to demonstrate the usage of Business document management (BDM) in **USMF**. Depending on the VM you are using the preview option of Business document management may not be working properly due to restrictions on the VM applied by the hosting company.

**Note:** you will not have the preview issue if you are working with your own environment.

In this exercise you will import the data from a free text invoice into an excel template by using the ER *data model *configuration which is provided as part of this lab in XML format.

**Important**: Click on the hyper link to download the data model and save it in the **Download** folder on your VM running an instance of **Dynamics 365 Finance**.

-   **Sample ER customer invoicing solution**

    -  [Customer invoicing model.version.2.xml](https://github.com/MicrosoftLearning/MB-300-Microsoft-Dynamics-365-Core-Finance-and-Operations/tree/master/Allfiles/Labs) 

    -  [Customer FTI report (GER).version.2.3.xml](https://github.com/MicrosoftLearning/MB-300-Microsoft-Dynamics-365-Core-Finance-and-Operations/tree/master/Allfiles/Labs)

The ER configuration will refer to the provider as the author of the
configuration. In this example, you will create a configuration provider for
sample company, **Litware, Inc.** These steps can be performed in any company as
ER configuration providers are shared among all companies.

### Create a provider

1.  Go to the **navigation pane** in the upper left corner and
    select **Organization administration**.

2.  Go to **Workspaces > Electronic reporting**.

3.  Go to **Related links > Configuration providers**.

4.  Select **New**.

5.  In the Name field, type **Litware, Inc.**

6.  In the Internet address field, type **http://www.litwareinc.com/**

7.  Select **Save**.

8.  Close the page.

### Select as an active provider

1.  Select the **Litware, Inc.** provider.

2.  Click **…** drop down.

3.  Select **Set active**.

### Import ER solutions

Import the ER *data model* configuration of each ER solution in the tables above
before you import the corresponding ER *format* configuration.

1.  Select the **Organization administration** \> **Electronic
    reporting** \> **Reporting Configurations** tile.

2.  Select the first node on the top of the page,

3.  Select **Exchange** button.

4.  Select **Load from XML file**.

5.  Select **Browse** to load the required XML file.

6.  Select **Customerinvoicingmodelversion2.xml**

7.  Select **OK** to confirm configuration's import.

8.  This will create a new node “**Customer Invoicing model”**

9.  Select the “**Customer Invoicing model”** node.

10. Select **Exchange** button.

11. Select **Load from XML file**.

12. Select **Browse** to load the required XML file.

13. Select **CustomerFTIreportGERversion23**

14. Select **OK** to confirm configuration's import.

15. This will create a new sub-node “**Customer FTI report (GER)”**

16. Select “**Customer FTI report (GER)”**

17. Select **Designer** button.

18. Expand **Report**

19. Expand **Invoice**

20. Review the sub-nodes and the values of the **Format** tab on the right-hand
    side.

21. Select the **Mapping** tab and review the values.

22. Close the **Designer** form.

23. Close the **Reporting Configuration** form.

24. Click on the **Home** button.

### Verify Business document management feature is enabled

To start Business document management, you need to open the **Feature
management** workspace and enable the **Business document management** feature.

1.  Open the **Feature management** workspace.

2.  Select **All** tab.

3.  In the quick filter type **Business,** then press enter**.**

4.  Make sure the **Business document management** feature is enabled.

5.  Click **Home**.

### Configure access permissions

By default, when access to Business document management permissions is not
enabled, every user with access to the Business document management workspace
will see all of the ER solution templates that are available.

The Business document management workspace will show only those templates that
reside in ER format configurations and that are marked by a **Business document
type** tag.

1.  Go to **Organization administration** \> **Electronic
    reporting** \> **Business document management** \> **Manage access
    permissions**.

2.  Click **Access permission settings**

3.  Set the **Apply configured access permission**, to **Yes**.

4.  Click **Ok**.

5.  Click **Add.**

6.  Select **Accounts receivable manager.**

7.  Click **Ok**.

8.  Under the **Access permission per tags of configuration**, click **New.**

9.  Select **Functional area** in the **Tag type** field.

10. Select **invoicing** in the **Id** field.

11. Under the **Access permission per configuration** section, click **Add.**

12. Select **Customer FTI report (GER)** in the **Name** field.

13. Click **Save**.

14. Close the form.

### Business document management Workspace

1.  Go to **Business document management** workspace

2.  Click **New document** button.

3.  Select **Invoicing**.

4.  To create a template you can click **Create document** button**.**

5.  In the Name field type “**My Free Text Excel Business Document**”

6.  Select **OK**.

**Note:** If you are using VM hosted by vendors rather than your environment you
will receive an error message while previewing the excel document. Click **Ok**.

1.  Select **Check for issues** button.

2.  Select the **Open in Desktop App** button.

3.  Select **Save > Save As**. Choose download folder and click **Save**.

4.  Select **Open folder** button.

5.  Select the **Free Text Invoice Template**.

6.  Double **Open**.

7.  If the Office activation form appears, click **Close**.

8.  View the format.

9.  Close the workbook.

10. Navigate to **Business document management** workspace.

**Note**: if you see ‌an error message that service is not available is due to
not having a license of Office 365 online or have not logged on to the Office
365 services for editing the template. If you are using the VM hosted by a
vendor you will see this message.

1.  You can delete the document by selecting **Action >Delete**.

2.  You can publish your business document by selecting **Publish** button.

3.  Click **Publish** button.

4.  Click **Yes**.
