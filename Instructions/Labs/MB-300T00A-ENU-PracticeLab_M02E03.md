---
lab:
    title: 'Exercise 03: Run a security report and analyze the output'
    module: 'Module 02: Configure security, processes, and options'
---
## Exercise 3: Run a security report and analyze the output

>   Finance and Operations apps security reports can be found under **System
>   administration \> Inquiries \> Security**. Let’s run and analyze some of
>   these security reports.

### User role assignments

>   The **User role assignments** report generates a view of the current user
>   role assignments in your system. By default, the report includes all users
>   with roles assigned. You can limit the report to a specific set of users by
>   entering them when generating the report.

1.  Navigate to **System administration \> Inquiries \> Security \> User role
    assignments.**

2.  On the **User role assignments** report parameters pane, navigate to
    **Records to include** \> **Filter.**

3.  From there, you can add or remove filters to the list of users. A list of
    roles is provided for each user in the report, along with any restrictions
    at the legal entity or organization level.

4.  Select **OK**.

5.  View the results.

### Role to user assignments

>   The **Role to user assignment** report provides an aggregation of role
>   assignments. Expanding a role in the report shows the list of users assigned
>   to the role, and expanding the user name shows any restrictions the role has
>   applied. You can apply the same method for filtering the set of users to
>   this report as described for the **User role assignments** report.

1.  Navigate to **System administration \> Inquiries \> Security \> Role to user
    assignments.**

2.  On the report parameters pane, navigate to **Records to include** \>
    **Filter.**

3.  From there, you filter by User ID.

4.  Select **OK**.

5.  View the results.

### Security role access

>   The **Security role access** report provides a view of the effective
>   permissions for each security role. This report provides a flattened list of
>   permissions grouped by type across all sub-roles, duties, and privileges
>   contained in the role.

>   This report may take some time to run, since its data set backing can be
>   very large. If it is the first time the report has run, or there could be
>   changes to the role definitions, the **Rebuild collection** option should be
>   set to **Yes**. You can limit the roles included in the report by adding a
>   filter under **Records to include**.

1.  Navigate to **System administration \> Inquiries \> Security \> Security
    role access.**

2.  On the report parameters pane, navigate to Records to include \> Filter.

3.  From there, you can filter by security role or other fields.

4.  Select **OK**.

5.  View the results.

    Expanding a role shows the category of objects the role has access to.
    Expanding one of the object types will show a detailed list of each object
    of that type included in the role.

### Security duty assignments

>   The **Security duty assignments** report provides a view of all the duties
>   contained within a role. This report can be configured to run on any
>   collection of roles, which ensures that segregation of duties is maintained
>   between roles. By default, the report will include each role. To limit the
>   roles included, use the filtering provided in the **Records to include**
>   section.

1.  Navigate to **System administration \> Inquiries \> Security \> Security
    duty assignments.**

2.  On the report parameters pane, navigate to Records to include \> Filter.

3.  From there, you can filter by fields in various tables.

4.  Select **OK**.

5.  View the results.

    Expanding a role in the **Security duty assignments** report will show each
    duty assigned to the role, along with details of the duty.
