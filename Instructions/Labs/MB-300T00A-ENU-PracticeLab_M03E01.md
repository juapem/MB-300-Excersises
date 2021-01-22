---
lab:
    title: 'Exercise 01: Work with templates in the Data management workspace'
    module: 'Module 03: Manage Dynamics 365 Finance and Operation data'
---
## Exercise 1: Work with templates in the Data management workspace

>   The goal of the lab exercise is to apply the knowledge we have learned
>   regarding the Data management workspace.

>   Instructions:

1.  Go to **Workspaces \> Data management**.

2.  If the dialog box “The entity list is being refreshed. You may continue your
    work while this happens. The completion status of this operation can be
    found in the message center.” appeared, click **Close**.

3.  Click **Enhanced view** button in the top left of the screen.

4.  Select the **Templates** tile.

5.  Refresh the page or press **Shift+F5**. (There is a refresh arrow near the
    top right of the Dynamics screen.) Note if there are any templates
    available.

6.  Select **Load default templates**.

7.  Select **Load all**. This may take a while.

8.  In the list, find and select the desired template, such as **020 - GL
    Shared**.

9.  View available entities for General ledger shared template.

10. In the list, find and select the desired record, such as **Supply chain
    management** by using the filter

11. View available entities for Supply chain management template.

12. Expand the **Template details** section.

13. In the list, find and select the desired record, such as **Barcode setup**.

14. Select **Discover dependencies**. It takes a few minutes, then shows all
    dependencies of the selected entity. This may take a while.

15. View entities that **Barcode setup** entity has dependency with.

16. Close the **Discover dependencies** page.

17. Close the **Templates** page.

18. Select **Data entities** tile. View the available Finance and Operations
    apps entities.

19. Select any of the entities of your choice, such as **Accountants**.

20. Select **Entity structure** button to see the data source. Here you can
    enable or disable running the business logic in your project. For instance,
    for data migration, you may have modified the settings of certain
    configurations to meet the customer requirements, however the legacy data
    would violate the new rule, so you may need to make the decision to turn off
    the rule for historical data.

21. Select the **Target fields** button. View and edit the target fields, such
    as enabling or disabling the table configuration key status.

22. Close the **Target fields** page.

23. Close the **Entity structure** page.

24. Select the **Entity model view** button. It allows you to have better
    visibility by grouping entities per category and subcategory of nodes
    representing the module, and the models of the entities.

25. In the tree, expand **All\\AccountsPayable**. View available entities.

26. In the tree, select **All\\AccountsPayable\\Transaction**. View available
    entities.

27. In the tree, expand **All\\GeneralLedger**. View available entities.

28. In the tree, select **All\\GeneralLedger\\Document**. View available
    entities.

29. Close the **Entity model view** page.

30. Select **Entity category view** button.

31. In the tree, expand **All\\Configuration**. View available entities

32. In the tree, select **All\\Configuration\\SystemAdministration**. View
    available entities

33. In the tree, expand **All\\Reference**. View available entities

34. In the tree, select **All\\Reference\\AccountsReceivable**. View available
    entities

35. Close the **Entity category view** page.

36. Close the **Data entities** page**.**

37. Select the **Staging cleanup** tile.

38. In the **Entity** field, enter or select a value such as **1099 fields**.

39. Select **OK**.

40. Select the **Data task automation** tile.

41. Select **Load default tasks** to open the **Load default tasks** dialog.

42. From the drop-down, enter or select a value such as
    **MS_Sample_Regression_DMFManifest**.

43. Click **Select**.

44. Select **Load**. This dialog allows you to load multiple data task
    automation.

45. Select **Cancel**.

46. View available tasks.

47. Close the **Data task automation** page.

48. Select the **Configure data source** tile. Here you can view, edit, and
    create data types such as CSV, Excel, and Package.

49. Close all pages.
