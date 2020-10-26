## Exercise 4: Create a purchase requisition workflow

>   The Finance and Operations app that you're working in determines the type of
>   workflow that you can create. You need either Internet Explorer or Microsoft
>   Edge to create the type of workflow and open the workflow editor. In this
>   exercise, you will create a purchase requisition workflow in USMF. Before a
>   purchase requisition can be submitted for review, you must configure a
>   workflow.

### Instructions

#### Create and set up workflows

1.  Navigate to **Procurement and sourcing \> Setup** \> **Procurement and
    sourcing workflows**.

2.  On the list page that appears, select **New** on the **Action Pane**..

3.  On the **Create workflow** page, select the **Purchase requisition line
    review.**

4.  For the first time, the browser will show a dialog box to open the
    **Microsoft.Dynamics.AX.Framework.WorkflowEditorHost.application** form.

5.  Select **Open**.

6.  Select **Run**. The workflow editor takes a few minutes to download. When it
    is finished, the workflow editor automatically opens the **Sign in** dialog
    box.

7.  **Enter** your credentials and password.

8.  The **workflow editor** appears.

#### Drag workflow elements onto the canvas

>   To connect one workflow element to another, hold the pointer over an element
>   until connection points appear. Select a connection point and drag it to
>   another element. Be sure to connect all the elements.

1.  The **Workflow elements** area of the workflow editor contains elements that
    you can add to your workflow.

2.  To add elements to the workflow, drag **Review purchase requisitions** and
    **Approve purchase requisitions** onto the canvas.

3.  Connect **Start** to **Review purchase requisitions.**

4.  Connect **Review purchase requisitions** to **Approve purchase
    requisitions.**

5.  Connect **Approve purchase requisitions** to **End.**

#### Configure workflow properties

1.  Select **Review purchase requisitions**

2.  From the action pane, select **Properties** to open the **Properties** page.

3.  Enter a value in the **Name** field.

4.  Enter a value in the **Work item subject** field. Alternatively, you can
    also include placeholder and concatenate the text with the placeholder.

5.  Select the **Yellow** bar. This will navigate to the assignment type.

6.  Select **User** and select the **User** tab.

7.  Select a user and add it to the **Selected users** section.

8.  Select **Close**.

9.  Double-click on the **Approve purchase requisitions** from the action pane.

10. Select **Step 1**.

11. Select **Properties** to open the **Properties** page.

12. Enter a value in the **Name** field.

13. Enter a value in the **Work item subject** field. Alternatively, you can
    also include placeholder and concatenate the text with the place holder.

14. Select the **Yellow** bar. This will navigate to the assignment type.

15. Select **User** and select the **User** tab.

16. Select a user and add it to the **Selected users** section.

17. Select **Close**.

18. Select **Save and close**.

19. Specify a version description.

20. Select **OK**.

21. Select **Activate the new version**.

22. Select **OK**. It may take a few minutes for the workflow editor to finish
    its activation process, and it will close automatically.

23. Navigate to **Procurement and sourcing\>Setup \> Procurement and sourcing
    workflows**.

24. Refresh the page if you do not see your new workflow.
