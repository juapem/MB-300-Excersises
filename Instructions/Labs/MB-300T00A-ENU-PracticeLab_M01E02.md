## Exercise 2: Prepare, enable, and use Business document management

>   **Scenario**: You must import [Sample ER
>   configurations](https://mbs.microsoft.com/customersource/Global/AX/downloads/hot-fixes/365optelecrepeg),
>   into your current instance of Dynamics 365 Finance, the ER configurations
>   that contain the business document templates that can be edited by using
>   Business document management. Download, and then locally store the following
>   files to complete this procedure.

>   In this exercise you will import the ER *data model* configuration of each
>   ER solution from the following list before you import the corresponding ER
>   *format* configuration;

>   **Important**: Click on the hyper link to download the data model and save
>   it in the **Download** folder on your VM running an instance of **Dynamics
>   365 Finance**.

-   **Sample ER customer invoicing solution**

    -   [Customer invoicing
        model.version.2.xml](https://mbs.microsoft.com/files/public/CS/AX/Customerinvoicingmodelversion2.xml)

    -   [Customer FTI report
        (GER).version.2.3.xml](https://mbs.microsoft.com/files/public/CS/AX/CustomerFTIreportGERversion23.xml)

-   **Sample ER payment checks solution**

    -   Model for cheques.version.10.xml

    -   [Cheques printing
        format.version.10.9.xml](https://mbs.microsoft.com/files/public/CS/AX/Chequesprintingformatversion109.xml)

-   **Sample ER foreign trade solution**

    -   [Intrastat
        model.version.1.xml](https://mbs.microsoft.com/files/public/CS/AX/Intrastatmodelversion1.xml)

    -   [Intrastat
        report.version.1.9.xml](https://mbs.microsoft.com/files/public/CS/AX/Intrastatreportversion19.xml)

Each ER configuration will refer to the provider as the author of the
configuration. In this example, you will create a configuration provider for
sample company, **Litware, Inc.** These steps can be performed in any company as
ER configuration providers are shared among all companies.

### Create a provider

1.  Go to the **navigation pane** in the upper left corner and select
    **Organization administration**.

2.  Go to **Workspaces \> Electronic reporting**.

3.  Go to **Related links \> Configuration providers**.

4.  Select **New**.

5.  In the Name field, type Litware, Inc**.**

6.  In the Internet address field, type http://www.litwareinc.com/

7.  Select **Save**.

8.  Close the page.

### Select as an active provider

1.  Select the **Litware, Inc.** provider.

2.  Click **…** drop down.

3.  Select **Set active**.

### Import ER solutions

Import the ER *data model* configuration of each ER solution in the tables above
before you import the corresponding ER *format* configuration.

1.  Select the **Organization administration** \> **Electronic reporting** \>
    **Reporting Configurations** tile.

2.  On the top of the page, select **Exchange**.

3.  Select **Load from XML file**.

4.  Select **Browse** to load the required XML file.

5.  Select **Customerinvoicingmodelversion2**

6.  Select **OK** to confirm configuration's import.

7.  Repeat step 2 through 4

8.  Select **CustomerFTIreportGERversion23**

9.  Select **OK** to confirm configuration's import.

10. On the top of the page, select **Exchange**.

11. Select **Load from XML file**.

12. Select **Browse** to load the required XML file.

13. Select **Intrastatmodelversion1**

14. Select **OK** to confirm configuration's import.

15. Select **Intrastat model**

16. Repeat step 10 through 12

17. Select **Intrastatreportversion19**

18. Select **OK** to confirm configuration's import.

19. Expand Electronic ledger accounting model MX node

20. Select Auxiliary Ledger XML MX

21. Click Delete

22. Click Ok.

23. Select Chart of Account XML MX

24. Click Delete

25. Click Ok.

26. Select Journals XML MX

27. Click Delete

28. Click Ok.

29. Select Trial Balance XML MX

30. Click Delete

31. Click Ok.

32. Select Electronic ledger accounting model MX node

33. On the top of the page, select **Exchange**.

34. Select **Load from XML file**.

35. Select **Browse** to load the required XML file.

36. Select **Modelforchequesversion10**

37. Select **OK** to confirm configuration's import.

38. Repeat step 33 through 35

39. Select **Modelforchequesversion10**

40. Select **OK** to confirm configuration's import.

41. Select **Model for cheques**

42. On the top of the page, select **Exchange**.

43. Select **Load from XML file**.

44. Select **Browse** to load the required XML file.

45. Select **Chequesprintingformatversion109**

46. Select **OK** to confirm configuration's import.

47. Close the page.

### Enable Business document management

To start Business document management, you need to open the **Feature
management** workspace and enable the **Business document management** feature.

1.  Open the **Feature management** workspace.

2.  Make sure the **Business document management** feature is enabled.

### Configure access permissions

By default, when access to Business document management permissions is not
enabled, every user with access to the Business document management workspace
will see all of the ER solution templates that are available.

The Business document management workspace will show only those templates that
reside in ER format configurations and that are marked by a **Business document
type** tag.

1.  Go to **Organization administration** \> **Electronic reporting** \>
    **Business document management** \> **Manage access permissions**.

2.  Click **Access permission settings**

3.  Select **Yes**.

4.  Click **Ok**.

5.  Click **Add.**

6.  Select **Accounts receivable manager.**

7.  Click **Ok**.

8.  Under the **Access permission per tags of configuration**, click **New.**

9.  Select **Functional area** in the **Tag type** field.

10. Select **invoicing** in the **Id** field.

11. Under the **Access permission per configuration** section, click **New.**

12. Select **Customer FTI report (GER)** in the **Name** field.

13. Click **Save**.

### Business document management Workspace

1.  Go to Business document management workspace

2.  Click **New document** button.

3.  Select **Invoicing**.

4.  In order to create a template you can click **Create document.**

5.  Close all pages.
