---
lab:
    title: 'Exercise 02: Set up segregation of duties'
    module: 'Module 02: Configure security, processes, and options'
---
## Exercise 2: Set up segregation of duties

>   The HR department of USMF has requested a rule for segregation of duties for
>   **two duties: Access benefits workspace**  and **Approve production
>   journal**. As a system administrator, you need to create the rule in Finance
>   and Operations apps.

>   Complete the following procedure to create a rule. You must be a system
>   administrator to complete the procedure.

### Instructions:

1.  Go to **System administration \> Security \> Segregation of duties \>
    Segregation of duties rules**.

2.  Select **New**.

3.  In the **Name** field, enter a name for the rule such as ‘My Segregation of
    duties rule’.

4.  In the **First duty** field, select the drop-down button to open the lookup.

5.  In the list, find and select the first duty that is controlled by the rule
    (**Access benefits workspace**).

6.  In the **Second duty** field, select the drop-down button to open the
    lookup.

7.  In the list, find and select the second duty that is controlled by the rule
    (**Approve production journal**).

8.  In the **Severity** field, select **Medium**. The severity of the risk that
    occurs when the same user or role performs both duties.

9.  In the **Security risk** field, enter a description of the security risk
    such as ‘HR-Production’.

10. In the **Security mitigation** field, type a value such as ‘Managerial
    review is necessary’.

    Enter a description of the actions that you will take to mitigate the
    security risk. For example, you can mitigate the risk by conducting more
    detailed reviews of the process, by conducting a monthly managerial review,
    or by sharing resources with other departments.

11. Select **Save**.

12. Close the page.
