## Exercise 9: Use Excel workbook designer

You need to use the Excel workbook designer page to create an Open in Excel
experience for an entity.

### Instructions

1.  Switch to the **USMF** legal entity.

2.  Go to **Fleet Management \> Setup \> Fleet Setup**

3.  In the **Data setup** tab, click **Create.**

4.  In the Sample data created dialog box, click **Close**.

5.  Close the page.

6.  Navigate to **Common \> Common \> Office integration \> Excel workbook
    designer**.

7.  Select the **FleetCustomer** entity. You may use the filter to save time.

8.  Add all fields in the list of available fields to the list of selected
    fields.

9.  Select **Create workbook**. You may safely ignore a SharePoint informational
    message.

10. **Download** and **Open** the workbook that is generated.

11. If the office activation appears click close.

12. If necessary, select **Enable editing** to enable the Excel Data Connector
    App to load. Customer data is read from the OData service on the server and
    added to the table.

13. Click **Trust this add-in**.

14. This workbook contains the Excel Data Connector App, a binding to the Fleet
    Management Customer entity, and a pointer to the server that the workbook
    was generated from.

15. Click sign in and use the alias you are using to connect to Dynamics 365
    Finance.

16. Click **Yes** to stay connected.

17. Insert a blank row above the table and enter **Fleet Customers** as the
    title.

18. Rename the worksheet **FleetCustomers**.

19. Rearrange some of the fields in the table.

20. Select **Design** to open the design experience.

21. Next to the FleetCustomer data source, there are buttons for editing and
    deleting the data source. Select **Edit** to see the field list.

22. Select fields and move them as you require.

23. Set the order for the first three fields to **FirstName**, **LastName**, and
    **DriverLicense**.

24. Select **Update**. Note that the field order is changed.

25. Select **Done**.

26. Select the **Settings**.

27. Select **Clear binding data** so that the workbook contains no bound data.

28. Select **OK**.

29. Save the workbook as FleetCustomersBasic.xlsx.

30. In an internet browser, navigate to **Common \> Common \> Office integration
    \> Document templates**.

31. Select **New**.

32. Browse to the file that you just saved.

33. Select **OK**. The template is added as a line in the templates table.

34. In the **FleetCustomersBasic** row, clear the apply current record filter
    check box, so that an unfiltered list of customers will be loaded after the
    template is opened.

35. Change the **Template display name** value to Fleet Customers Basic.

36. Navigate to **Fleet Management \> Customers \> Customer**.

37. Select **Open** in Microsoft Office. Note that Fleet Customers Basic is now
    an option in the Open in Excel section. Select that option.

38. Open the workbook that is generated.

39. Select **Enable editing** to enable the Excel Data Connector App to load.
    Customer data is read from the OData service on the server and added to the
    table binding that you created.
