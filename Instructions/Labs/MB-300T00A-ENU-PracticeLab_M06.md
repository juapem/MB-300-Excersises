# Exercise - Create a purchase requisition workflow

The Finance and Operations module that you're working in determines the types of workflow that you can create.

In this exercise, you will create a purchase requisition workflow. Before a purchase requisition can be submitted for review, you need to configure the workflow.

## Create and set up workflows

1. Go to **Procurement and sourcing** **&gt; Setup** **&gt;** **Procurement and sourcing workflows**.

2. On the list page that appears, on the Action Pane, select **New**.

3. On the **Create workflow** page, select the **Purchase requisition line review**.

4. For the first time, the browser will show a dialog box to open the **Microsoft.Dynamics.AX.Framework.WorkflowEditorHost.application** page.

5. Select **Open**.

6. Select **Run**. It takes a few minutes for the workflow editor to be downloaded. When it has finished the download, it automatically opens the **Sign in** dialog box.

7. Enter your credentials and password.

8. The workflow editor appears.


## Drag workflow elements onto the canvas

1. To connect one workflow element to another, hold the pointer over an element until connection points appear.

2. Click a connection point and drag it to another element. Be sure to connect all the elements.

3. The **Workflow elements** area of the workflow editor contains the elements that you can add to your workflow.

4. To add elements to the workflow, drag **Review purchase requisitions** and **Approve purchase requisitions** onto the canvas.

5. Connect **Start** to **Review purchase requisitions**.

6. Connect **Review purchase requisitions** to **Approve purchase requisitions**.

7. Connect **Approve purchase requisitions** to **End**.


## Configure workflow properties

1. Select **Review purchase requisitions** and, from the Action Pane, select **Properties** to open the **Properties** page.

2. Enter a value in the **Name** field.

3. Enter a value in the **Work item subject** field. Alternatively, you can also include a place holder and concatenate the text with the place holder.

4. Select the **Yellow** bar. This will navigate to the assignment type.

5. Select **User** and select the **User** tab.

6. Select a user and add it to the **Selected users** section.

7. Select **Close**.

8. Select **Save and close**.

9. Specify a version description.

10. Select **OK**.

11. Select **Activate the new version**.

12. Click **OK**. It might take a few minutes for the workflow editor to finish its activation process, and then it will close automatically.

13. Go to **Procurement and sourcing &gt; Setup &gt; Procurement and sourcing workflows**.

14. Refresh the page if you do not see your new workflow.