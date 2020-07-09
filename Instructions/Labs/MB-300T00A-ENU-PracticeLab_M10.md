---
lab:
    title: 'MB-300.0 Practice Lab: Module 10'
    module: 'Module 10'
---

# Exercise 1: Use office integration


You need to use and build office integration that involves Excel, Word, Document management, and email in Finance and Operations.


## Load the Fleet data set


1. Go to **Fleet Management** > **Setup** > **Fleet** **setup**.

2. Select **Create**.


## Static Export to Excel


1. Go to **Fleet Management** > **Customers** > **Customer**.

2. Select **Open in** **Microsoft Office** > **Export to Excel** > **Customers**.

3. Download and open the workbook that is generated. Note that the columns in the workbook match the columns in the grid.

4. Select the first two rows by clicking in the left edge of the row, below the Select all check mark.

5. Right-click the grid header to open the shortcut menu. Note that both **Export all rows** and **Export marked rows** are available as commands.

6. Select **Export marked rows**. Note that the columns in the workbook match the columns in the grid, and that the rows that are exported match the rows that you selected.


## Generated Open in Excel


1. Go to **Fleet Management** > **Customers** > **Customer**.

2. Select **Open in** **Microsoft Office** > **Open in Excel** > **Fleet Management Customers (unfiltered)**.

3. Download and open the workbook that is generated. This workbook contains the Excel Data Connector App, a binding to the Fleet Management Customer entity, and a pointer to the server that the workbook was generated from.

4. Select **Enable editing** to enable the Excel Data Connector App to load. Customer data is read from the OData service on the server and added to the table.

5. In an internet browser, on the **Customer** page, select **Edit** (or press F2) and change the email address of one of the customers.

6. In Excel, select **Refresh**. Note that the new email address is shown in Excel.

7. In Excel, change the email address of one of the customers.

8. In the Excel app, select **Publish**.

9. In an internet browser, select **Refresh** in the upper right of the page (or press Shift+F5). Note that the new email address is shown on the **Customer** page.

10. In Excel, select the **Settings** (gear) button in the lower-right corner of the Excel app. You can use the dialog box that appears to adjust the settings in the current workbook. Note that the **Server URL** value matches the start of the URL that is shown in an internet browser. Also note that the data refresh and data publish operations are listed.

11. Select **Cancel** to close the **Settings** dialog box.

12. Select the **Message Center** (flag) button in the lower-right corner of the Excel app. The message center dialog box that appears provides information about what is occurring in the Excel app.


## Add and remove table columns from an existing table data source in the Excel app


1. To get a workbook that has an existing table data source, such as Fleet management customers, go to **Fleet Management** > **Customers** > **Customer**.

2. Select **Open in Microsoft Office** > **Open in Excel** > **Fleet Management Customers (unfiltered)**.

3. Download and open the workbook that is generated. This workbook contains the Excel Data Connector App, a binding to the Fleet Management Customer entity, and a pointer to the server that the workbook was generated from.

4. Select **Enable editing** to enable the Excel Data Connector App to load. Customer data is read from the OData service on the server and added to the table.

5. Open the data source for editing. In Excel, select **Design**. A list of table and field data sources appears.

6. Select the **Edit** (pencil) button next to the existing table data source. The data source details are shown.

7. Remove fields. In the **Selected** list, double-click a field. Alternatively, click a field, and then select **Remove**. To select multiple fields, hold down the Ctrl key while you click the fields. To select all fields, press Ctrl+A.

8. Add fields. In the **Available** list, double-click a field. Alternatively, click a field, and then select **Add**. To select multiple fields, hold down the Ctrl key while you click the fields. To select all fields, press Ctrl+A.

9. Change the field order. In the **Selected** list, click a field, and then select **Up** or **Down**.

10. Change a field label. In the **Selected** list, click a field, and then select the **Column label** field below the list. You can change the label to either a static string or a label identifier that will be translated to the active language (for example, **@SYS129977**).

11. To apply the changes that you made to data source fields, select **Update** to return to the data source list.

12. Select **Refresh** to make sure that any new fields are filled with data.


## Open in Excel Online


1. Go to **Fleet Management** > **Customers** > **Customer**.

2. Select **Open in Microsoft Office** > **Open in Excel** > **Fleet Management Customers**.

3. Select **SharePoint**.

4. Browse to the desired Microsoft SharePoint folder.

5. Select **Save**. The default behavior is to open the file after it's saved.

6. Note that the workbook opens in Excel Online. In Excel Online, capabilities of the Excel app, such as refresh and publish, and the design experience, should work just as they work in on-premises Excel instances.


## Lookups in the Excel app


1. Go to **Fleet Management** > **Rentals** > **Rental**.

2. Select **Open in** **Microsoft Office** > **Open in Excel** > **Fleet Management Rentals**.

3. Open the workbook that is generated.

4. Select **Enable editing** to enable the Excel Data Connector App to load and read in data.

5. Select a **Drivers license** value. Note that a relationship lookup now appears in the Excel app and shows a list of customers. Because relationship lookups are in their first generation, no filtering or sorting is currently supported.

6. Select another customer in the lookup and note that the **Drivers license** value changes. Because this field is part of the key, select the original **Drivers license** value to reset it. Note that the **Drivers license**, **First name**, and **Last name** fields form a multi-part key, but the Excel app doesn’t immediately change all parts of the multi-part key.

7. Select a **Start date** value. Note that a date picker now appears in the Excel app.

8. Select another date to change the **Start date** value.

9. Select **Design** and edit the FleetRental data source by adding the **Status** field as a column in the table binding.

10. When you've finished adding the **Status** column, select a **Status** value. Note that an enum list now appears in the Excel app.

11. While focus is in the **Status** column, move up and down the list of rentals to observe how quickly the enum list changes to reflect the current value. The whole enum list is shown so that the user can quickly view all the available values.

12. Select a different **Status** value to observe how an enum value can be changed by using a single click.


 

 

# Exercise 2: Use workbook designer


You need to use the **Excel workbook designer** page to create an Open in Excel experience for an entity.


1. Go to **Common** > **Common** > **Office integration** > **Excel workbook designer**.

2. Select the **FleetCustomer** entity.

3. Add all fields in the list of available fields to the list of selected fields.

4. Select **Create workbook**.

5. Open the workbook that is generated. This workbook contains the Excel Data Connector App, a binding to the Fleet Management Customer entity, and a pointer to the server that the workbook was generated from.

6. Select **Enable editing** to enable the Excel Data Connector App to load. Customer data is read from the OData service on the server and added to the table.

7. Insert a blank row above the table and enter **Fleet Customers** as the title.

8. Rename the worksheet **FleetCustomers**.

9. Rearrange some of the fields in the table. Select **Design** to open the designer experience.

10. Next to the **FleetCustomer** data source are buttons for editing and deleting the data source. Select **Edit** to see the field list.

11. Select fields and move them as you require. Set the order for the first three fields to **FirstName**, **LastName**, and **DriverLicense**.

12. Select **Update**. Note that the field order is changed.

13. Select **Done**.

14. Select the **Settings** (gear) button.

15. Select **Clear binding data** so that the workbook contains no bound data.

16. Select **OK**.

17. Save the workbook as **FleetCustomersBasic.xlsx**.

18. In an internet browser, go to **Common** > **Common** > **Office integration** > **Document templates**.

19. Select **New**.

20. Browse to the file that you just saved.

21. Select **OK**. The template is added as a line in the templates table.

22. In the **FleetCustomersBasic** row, clear the **Apply current record filter** check box, so that an unfiltered list of customers will be loaded after the template is opened.

23. Change the **Template display name** value to **Fleet Customers Basic**.

24. Go to **Fleet Management** > **Customers** > **Customer**.

25. Select **Open in Microsoft Office**. Note that Fleet Customers Basic is now an option in the **Open in Excel** section. Select that option.

26. Open the workbook that is generated.

27. Select **Enable editing** to enable the Excel Data Connector App to load. Customer data is read from the OData service on the server and added to the table binding that you created.

28. Bonus: Try using the designer experience in the Excel add-in to add another data source onto another worksheet.


 
