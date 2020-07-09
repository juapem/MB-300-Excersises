---
lab:
    title: 'MB-300.0 Practice Lab: Module 04'
    module: 'Module 04'
---

# Exercise 1: Generate and explore a financial report

You need to generate and explore an existing default financial report. 

This report includes all accounts and contains account properties (attributes) for the accounts. 

You'll be drilling into transaction detail, applying dimension filters, and changing the currency on the report. 

 
**Before you begin**

To get the most out of this exercise and the other exercises that are included with this module, we recommend that you have the standard sample data available in Finance and Operations that is installed using Lifecycle services (LCS).  


First, we'll update the display order of dimensions for financial reporting. This allows you to select how the dimensions display 


1. Go to **Financial dimension configuration for integrating applications** under the **Dimensions of Chart of Accounts** in **General ledger**. 

	![Screenshot of defining financial dimension formats for data entities](../media/mb-300-t-000-a-enu-practicelab-m-004-01.png) 


2. Arrange the dimensions so that the **Main Account** is first on the list. 

3. Arrange the dimensions so that the **Business Unit** is second on the list  

4. Arrange the dimensions so that the **Cost Center** is third on the list 

5. Arrange the dimensions so that the **Department** is forth on the list 

6. Save the dimension configuration.  


**Generate a report and explore the data in the report.** 

1. Go to **Financial reports** under **Inquiries and reports** in **General ledger**. 

2. Select the row for the report named **GL Detail – Default**. 

3. Click **Edit**. 

4. You'll be prompted to download the click-once report designer and to log in.  

5. Use your credentials to log in. 

6. Change the base year to 2012 and select **Generate**.  

7. When a report is generated from the report designer, it will open in a new browser tab.  

8. You can either explorer the report in the new browser tab or go to your original browser tab and open the report from there by selecting it from the **Financial reports** list. 

9. In the opened report, select one of the amounts to drill into the account detail for the report. 

10. Once in account detail, select an account with data and click **drill to report transaction level**.  

11. At the report transaction level, you can see the properties (attributes) that are included in the design of this report. Depending on the transaction and account, some or all the attributes may be displayed. 

12. Close the report transaction level. 

13. Select the same or a different account and click **open voucher transactions**. Voucher transactions are filtered to the period, year and account and dimension combination of the account selected. From **Voucher transactions**, you can select to explore other information about the transaction. 

14. Close the **Voucher transactions** page. Within a financial report, you can select to view the data either for a different period and year, or with different attributes and dimensions applied. This is done by using **Report options**. 

15. Select **Report options**. 

16. Select **Add a dimension filter** and type ‘001’ in the **Business unit** field. 

17. Click **OK**.  

18. The report now displays only the data for the 001 Business Unit. This is a personalized view of the report and isn't available for others to view. 

19. Close the filtered report. Financial reports can be displayed in any currency that has been added to Finance and Operations. 

20. Select **Currency**, then select **EUR**. The report now displays in Euros. Any currency codes or currency symbols included in the report design now display in the applied currency. If no currency symbol is defined for a currency, the currency symbol is not displayed. 

21. Close the **GL Detail** report. 

22. Close the **Report designer**. 


# Exercise 2: Add additional account properties to a report design

Now you will update a row definition to include all accounts, and the column definition to contain account attributes. Once the updates are complete, you'll generate the newly created report and explore the report. 


1. Go to **Financial reports** under **Inquiries and reports** in the **General ledger** module. 

2. Select the row for the report named **Summary Trial Balance – Default**. 

3. Select **Edit**. **Summary Trial Balance – Default** to open the Report designer. 

4. Select **File**, then **Save As** and name the report ’Detailed trial balance with attributes’. 

5. Any time a new report is created in the Report designer, the financial reports list is updated in Finance and Operations. 

6. From the report definition, select the **Row definition** icon to open the **Trial Balance – Default row definition**. 

7. Save the row definition as ‘Detailed trial balance with attributes’. 

8. With the cursor on row 50, select **Edit**, then **Insert Rows from Dimensions**. Insert rows from dimensions allows you to choose which dimensions you'd like to have in your row definition.  

9. You are going to build the row definition using Main account. 

10. Make sure **Main account** contains all ampersands and select **OK**. The row definition now contains all the main accounts for legal entity USMF. 

11. Scroll down to row 11110 and delete row 11110. 

12. In row 11080, select **--- (Underscore amounts)**. 

13. In row 11140, type ‘Total of all accounts’ in column B. 

14. In column C, select **TOT** from the drop down. 

15. Type ‘50:11080’ in column D. 

16. **Save** the row definition.  

17. The row definition now contains all the accounts plus a total row to add all the accounts together.    
‎ 

**Update the column definition to include additional account attributes** 

1. From the **Detailed trial balance with attributes** report definition, select the column definition icon to open the **Summary Trial Balance – Default** column definition. 

2. Save the column definition as ‘Detailed trial balance with attributes’.  

3. The column definition contains financial data columns, a description column and calculation columns.  

4. Add the **Journal description** attribute columns to the column definition to provide additional detail about the accounts. 

5. Add the **Transaction date** attribute columns to the column definition. 

6. Add the **Created by** attribute columns to the column definition. 

7. Add the **Last modified by** attribute columns to the column definition. 

8. In column I, select **ATTR** as the column type.  

9. Select **Journal number** as the attribute category. 

10. Continue adding columns for the remaining attributes. 

11. In the **Header 2** row, add descriptions for each of the new columns that have been added. 

12. Save the column definition. Now that the row definition and column definition have been updated, we'll need to add them to the report definition. 

13. From the **Detailed trial balance with attributes** report definition, select **Detailed trial balance with attributes** for both the row definition and column definition. 

14. Change the base year to ‘2012’. 

15. **Save** the report definition and then click **Generate**. When the report opens, you can explore the report as you did in the first exercise.  

16. Drill down on different accounts to see how the additional attributes are displayed. 

17. Close the **Detailed trial balance with attributes** report. 

18. Close the **Report designer**. 


# Exercise 3: Create a multidimensional report using a reporting tree

You need to modify an existing default report.  You will create a reporting tree and add to a report definition to produce a Cost center/divisional income statement. When the updates are complete, you'll generate the Cost center/divisional income statement and explore the report using the reporting tree. 


1. Go to **Financial reports** under **Inquiries and reports** in the **General ledger** module. 

2. Select the row for the report named **Income Statement – Default**. 

3. Select **Edit**. **Income statement – default** will open in Report designer. 

4. On the **File** menu, point to **New**, and then click **Reporting tree definition**. 

5. On the **Edit** menu, click **Insert reporting units from dimensions**. 

6. Clear check boxes for all dimensions, except **Cost center**. 

7. Click the **From dimension** field for the Cost center dimension, type ‘007’, and then press the **Tab** key.  

8. In the **To dimension** field, type ‘018’. 

9. **Save** the resulting tree with the name ‘Cost centers by division’.  


Now that the reporting tree is created, you'll modify the reporting tree to contain three new rollup units; **Marketing**, **Operations** and **Retail**. 


10. On the **Window** menu, click **Cost centers by division**.  

11. If the reporting tree has been closed, select it from the **Reporting tree definitions** in the Navigation pane. 

12. Click unit number two, **Trade shows**, and click the **Insert reporting unit** icon. 

13. Double-click the entity column on the blank row and select **USMF**. 

14. Type **Marketing** in columns B and C. 

15. Click unit number five, **Service operations**, and right-click.  

16. Select **Insert reporting unit**. 

17. On the **Window** menu, click **Cost centers by division**.  

18. Type **Operations** in columns B and C. 

19. Click unit number twelve, **Outlet**, and right-click.  

20. Select **Insert reporting unit**. 

21. On the **Window** menu, click **Cost centers by division**.  

22. Type **Retail** in columns B and C. Notice the **Marketing**, **Operations** and **Retail** units display at the same level as the current rollup units.  

23. The new units are organized next. Reporting units are organized through the right-click options; promote and demote, or by drag and drop. 

24. Verify unit three, **Trade shows**, is active and right-click. 

25. Select **Demote reporting unit**. Notice the unit now displays as a child of **Marketing**. 

26. Click unit four, **Marketing campaign**, and right-click. 

27. Select **Demote reporting unit**. 

28. Click **Service operations** in the graphical display. Press and hold down the left mouse button while dragging the unit up to **Operations**.  

29. Release the left mouse to drop the unit into Operation's rollup. Repeat for **Production, Quality Control, Logistics, Procurement** and **Administration**. 

30. Make **Outlet**, **Super**, **Mall**, and **Online** children of **Retail** by either demoting them or dragging and dropping them. 

31. Save the resulting re-organization. Now that we have the reporting tree created and organized, it can be added to the report definition. 

32. On the **Window** menu, select **Income statement – Default** to open the report definition. 

33. Click the **Tree type** drop-down arrow and select **Reporting tree**. 

34. Click the **Tree** drop-down arrow and select **Cost centers by division**. 

35. Change the base year to ‘2012’, save the changes and click **Generate**. When the report opens, you can explore the report. 

36. Select the **Reporting tree** drop-down to view the reporting units.  

37. Or, you can drill down on a row of the report to see all the balances for all units of the reporting tree. 

38. Close **Income statement – default**. 

39. Close **Report designer**. 


# Exercise 4: Create a consolidated report using an organization hierarchy

You need to add an organization hierarchy in the report definition to produce a consolidated income statement and balance sheet. When the updates are complete, you'll generate the consolidated report and explore the report using the reporting tree. 

1. Go to **Financial reports** under **Inquiries and reports** in the **General ledger** module. 

2. Select the row for the report named **Balance sheet and Income statement side by side – default**. 

3. Select **Edit**. The **Balance sheet and income statement side by side – default** report will open in the Report designer. 

4. Select **File** > **Save as** and name the report ‘Consolidated balance sheet and income statement side by side’. 

5. Change the base year to ‘2012’. 

6. Click the **Tree type** drop-down arrow and select **Organization hierarchies**. 

7. Click the **Tree** drop-down arrow and select **Contoso holdings**. 

8. Save the changes and generate the report.  

9. If prompted, select all reporting units. When the report opens, you can explore the report. 

10. Select **Report options**. 

11. Select **Add a dimension filter** and then type ‘022’ in the **Department** field 

12. Click **OK**. 

13. Close the filtered report. 

14. Select the **Reporting tree** drop down to view the reporting units.  

15. Or, you can drill down on a row of the report to see all the balances for all units of the reporting tree. 

16. Close the **Consolidated balance sheet and income statement side by side** report. 

17. Close the **Report designer**. 


# Exercise 5: Create a side-by-side departmental report

You need to create a new side-by-side departmental income statement report. You'll use an existing row definition, but create a new report definition and a new column definition that uses dimension filters. 

**Instructions** 
1. Navigate to **Financial reports** under Inquiries and reports in **General ledger**. 

2. Select **New**.  

3. Report designer will open with a blank report definition open.  

**Creating the column definition** 

4. Create a new column definition by clicking **File**, then **New**, and then **Column Definition**. 

5. In **Column A**, select **DESC** for the column type. 

6. In **Column B**, select **FD** for the column type. 

7. Double click in **the Dimension Filter** field. 

8. In the **Dimension** window, double click the **Department** column. 

9. In the Individual or range section of the dialog, click the **ellipsis** for the **From** field to display a list of departments. 

10. Select department **022**, **Sales &amp; Marketing** and then click **OK**. 

11. Repeat steps 4 to 10 for Departments 023-025. 

12. On the **Header 2** row for each **FD** column, you need to type the department descriptions for Column **B** – **Sales and Marketing**. 

13. On the **Header 2** row for each **FD** column, you need to type the department descriptions for Column **C – Operations**. 

14. On the Header 2 row for each FD column, you need to type the department descriptions for Column **D – Finance**. 

15. On the Header 2 row for each FD column, you need to type the department descriptions for Column **E – IT**. 

16. **Save** the column definition as Side by Side Departments.  

17. Since we are using an existing row definition, the report definition can now be modified to have use the newly created column definition and the existing row definition. 

18. On the **Window** menu, select **New Report Definition** to open the report definition. 

19. Select **Income Statement – Default** as the row definition and **Side by Side Departments** as the column definition. 

20. Save the report definition as **Side by Side Departmental Income Statement**. 

21. Change the base year to **2012**. 

22. Change the detail level to **Financial, Account and Transaction**. 

23. **Save** your changes and **generate**.  

24. Once the report completes generating and opens, you can explore the report. 


# Exercise 6: Customer and vendor account statements

You need to print accounts statements for customers and vendors that display information for a time period that you select for FRSI legal entity based on France. 

**Instructions** 
1. Navigate to **Accounts receivable &gt; Inquiries and reports &gt; Customers &gt; Customer account statement report - France**. 

2. In the **From** date field, enter a date. 

3. In the **To** date field, enter a date. 

4. In the **Assessment date** field, enter a date. 

5. Click **OK**. 

6. Navigate to **Accounts payable &gt; Inquiries and reports &gt; Vendor reports &gt; Account statement**. 

7. In the **From** date field, enter a date. 

8. In the **To** date field, enter a date. 

9. In the **Assessment date** field, enter a date. 

10. Click OK. 