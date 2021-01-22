---
lab:
    title: 'Exercise 03: Copy configuration data between legal entities'
    module: 'Module 03: Manage Dynamics 365 Finance and Operation data'
---
## Exercise 3: Copy configuration data between legal entities

In this exercise, you will copy configuration data from legal entity **USMF**
into a new company called Woodgrove Bank (WOB).

>   **Note**: You need to complete Exercise 1

1.  Go to **Workspaces \> Data management**.

2.  Select the **Copy into legal entity** tile.

3.  In the **Group name** field, enter **Copy to LE**.

4.  In the **Description** field, enter **WOB**.

5.  In the **Data project operation type** field, select **Copy into legal
    entity**.

6.  Select **Create legal entities** to open the **New legal entity** dialog
    box.

7.  In the **Name** field, enter **Woodgrove Bank**.

8.  In the **Company** field, enter **WOB**.

9.  In the **Country/region** field, enter **USA**.

10. Select **OK**.

11. Select **Add template** to open the **Add template** dialog box.

12. In the **Copy from template** field, enter or select **010 - System Setup**

13. Select **OK**.

14. Select **Yes** in the **Copy number sequences** field.

15. Select **Copy into legal entity** button.

16. The dialog box appears with the following text “Copy into legal entity job
    scheduled. Please refresh the form to see current status”. Select **Close**.

17. Select **Refresh** button. Continue until the job is finished.

18. This process may take a while.

19. When the job is finished, switch to **WOB** company and test your newly
    created legal entity.
