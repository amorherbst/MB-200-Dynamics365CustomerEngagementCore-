---
lab:
    title: 'Lab: Outlook integration'
    module: 'Module 11: Introduction to Integration'
---

Module 11: Introduction to Integration
=====================================

Lesson 6: Practice Lab – Outlook integration

Scenario
--------

As a functional consultant at Contoso, you are tasked with configuring Outlook
integration for your client Fabrikam. In this lab, you will review security
roles, enable and use the App for Outlook. Then you will enable activities for
the knowledge assessment entity created in previous lessons and customer the App
for Outlook.

**Important Note:** This lab will provide you with an actual Office 365 tenant
and licenses for the Power Platform applications you will be using in this
course. You will only be provided with one tenant for the practice labs in this
course. The settings and actions you take within this tenant do not roll-back or
reset, whereas the virtual machine you are provided with does reset each time
you close the lab session. Please be aware that Office 365 is evolving all the time. The
instructions in this document may be different from what you experience in your
actual Office 365 tenant. It is also possible to experience a delay of several
minutes before the virtual machine has network connectivity to begin the labs.

Exercise 1 - Acquire Tenant Information and Connect
---------------------------------------------------

**Note:** If you have already completed a practice recently, the virtual machine
might pick up where you left off and you will not need to login again.  In that
case you can skip ahead to exercise two and resume.

### Task 1 – Connect to the Power platform administration portal

1.  On Virtual machine MB200-Dynamics_Lab, sign in as Admin with the password
    Pa55w.rd if you are not already logged in.

2.  Outside the VM in the online lab interface click Files and choose D365
    Credentials. This will allocate an Office 365 tenant for you to use in these
    labs.  It will display the admin email and password for your tenant.  You
    should copy this information to notepad or similar for your reference.

3.  In MB200-Dynamics_Lab launch Microsoft Edge from the taskbar. By default,
    the browser opens Office 365. Use the O365 credentials you just acquired in
    the previous step to login.

4.  Navigate in the browser to the Power platform admin portal at
    [https://admin.Powerplatform.microsoft.com](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.Powerplatform.microsoft.com&data=02%7C01%7Cv-juya%40microsoft.com%7C4be5a28c6f1e41eefee808d687ae2dc7%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636845580068684293&sdata=cLrD%2FhTDb5sRbajtFR9RrztfyTDCo0xGS4k8FSxTaIc%3D&reserved=0)

Exercise 2 – Outlook Integration
--------------------------------

### Task 1 – Review Security Roles for Users

In this task, you will check if your Users have security roles with Outlook
enabled.

1.  Navigate to <https://admin.powerplatform.microsoft.com/>

2.  Select **Environments**.

3.  Select your environment and click **Settings**.

4.  Go to the **Users + Permissions** section and click **Users**.

5.  Click to open the **Test User**.

6.  Click **Manage Roles**.

7.  Make sure the selected **Roles** include the **Salesperson** role and click
    **OK**.

8.  Close the **User** form editor.

9.  Click to open the user you are logged in as.

10. Click **Manage Roles**.

11. Make sure the selected **Roles** include the **System Administrator** role
    and click **OK**.

12. Close the **User** form.

13. Close the **Users** browser tab.

14. Go to the **Users + Permissions** section and click **Security Roles**.

15. Locate and open the **Salesperson** role.

16. Select the **Business Management** tab and scroll down to the **Privacy
    Related Privileges** section.

17. Make sure the **Use Dynamics 365 for Outlook** is set to **Organization**.
    Note: For custom security roles you would need to enable these privileges as
    we outlined in the Dynamics 365 App for Outlook topic.

18. Close the security role editor.

19. You may check what other security roles have **Dynamics 365 for Outlook**
    enabled.

20. Close the **Security Roles** browser tab.

### Task 2 – Enable App

In this task, you will enable Dynamics 365 App for Outlook, this will ensure new
users who are eligible will automatically get the app.

1.  Navigate to <https://admin.powerplatform.microsoft.com/>

2.  Select **Environments**.

3.  Select your environment and click **Open Environment**.

4.  Navigate to **Settings** and select **Dynamics 365 App for Outlook**.

5.  Go to the **Settings** section and check the **Automatically Add App to
    Outlook** checkbox and click **Save**.

6.  In the **All Eligible Users** grid, you should see both of your users.

7.  Click **Add App for All Eligible Users** button located on top of the grid.

8.  The status should change to **Pending**. It can take up to 15 minutes to
    complete and say Added to Outlook.

9.  Press the **Refresh** button located on the top right corner of the grid.
    You will see the **Added to Outlook status**.

### Task 3 – Use Dynamics 365 App for Outlook

In this task, you will be sending a test email and then using the Dynamics 365
App for Outlook to create the contact in Dynamics 365 and then associate the
email with an Opportunity you created. This is a common practice with a sales
organization that receives their initial inquiry email.

1.  Go to your personal email account, an email that is unrelated to your
    Dynamics 365.

2.  Send a test email to the admin user of your Dynamics 365.

3.  Navigate to <https://outlook.office.com> and make sure you are logged in as
    the admin user of your Dynamics 365.

4.  You should see the test email you sent from your personal email account.

5.  Click to select the test email.

6.  You should see **Dynamics 365** icon on the top right corner of the email.

7.  Click on the **Dynamics 365** icon.

8.  The Dynamics 365 pane will open, and it will show a message “Create contact
    first to avoid duplicates” this is because the email you sent from is not a
    contact in the current environment.

9.  Click on the **+** button located on bottom of the pane.

10. Select **Add as a Contact**.

11. Provide any other information you would like to include and click **Save and
    Close**.

12. The contact will be saved to Dynamics 365.

13. You will now add an **Opportunity**. Click on the **+ Add** button.

14. Notice that Assessment isn’t on this list. Select **Opportunity**.

15. Provide a **Topic** and select the Contact you just created as a
    **Contact**.

16. Click **Save and Close**.

17. Go to the email and click **Reply**.

18. Type some text in the reply body. Do not send the reply.

19. Click on the **Dynamics 365** icon located on the bottom right of the reply.

20. The Dynamics 365 pane will open. Notice it says **Not Tracked**.

21. Click on the Regarding textbox and select the Opportunity you created.

22. The message will change to **Track Pending**.

23. Go to the email and click **Send**.

24. Go to your personal email account.

25. Open the Reply form your **Dynamics 365** admin account.

26. Send a reply from your personal email account.

27. Go back to **Outlook** and open the new reply.

28. Click on the **Dynamics 365** icon.

29. The **Dynamics 365** pane will open and this time, the **Contact** and
    **Opportunity** will open.

30. Close the **Dynamics 365** pane.

### Task 4 – Enable Activities for Knowledge Assessment

In this task, you will be enabling a custom entity to be eligible to be set as a
regarding in the Dynamics 365 App for Outlook. In order to be eligible,
activities must be enabled.

1.  Navigate to <https://admin.powerplatform.microsoft.com/>

2.  Select **Solutions**.

3.  Click to open the **Knowledge Assessment Solution**.

4.  Click on the **…** button located in the command bar and select **Switch to
    Classic**.

5.  Expand **Entities** and select the **Knowledge Assessment** entity.

6.  Go to the **Communication & Collaboration** section and check the
    **Activities** checkbox.

7.  Click **Save**.

8.  Click **Publish** and wait for the publishing to complete.

9.  Close the solution explorer.

### Task 5 – Customize the Dynamics 365 App for Outlook

In this task, you will be customizing the app to include a custom entity and
removing Case, Competitor and Lead that you are not using.

1.  Navigate to <https://web.powerapps.com>

2.  In the upper right corner, review the Environment selector to make sure you
    are **NOT** in the **Default Environment**. You should have something like
    Contoso (crm2003) instead of Contoso(default). If you are set to default
    change the environment.

3.  Select **Apps**.

4.  Select **Dynamics 365 App for Outlook** and click **Edit**.

5.  Select the **Components** tab and click **Entities**.

6.  Uncheck the **Case**, **Competitor** and **Lead** entities, these entities
    don’t need to be part of this application.

7.  Locate the **Knowledge Assessment** custom entity and check it to include
    it.

8.  Click **Save**.

9.  Click **Publish**.

### Task 6 – Use the new customized app

In this task, you will be using the Dynamics 365 App for Outlook to review your
customizations.

1.  Go back to <https://outlook.office365.com> and refresh the browser.

2.  Select the email you had previously tracked.

3.  Click on the **Dynamics 365** icon.

4.  Locate the **Regarding** field and click **Search**.

5.  Click on the right arrow and the **Knowledge Assessment** entity should be
    available to you.

6.  Select the **Knowledge Assessment** entity and click **New**.

7.  Enter **Assessment from Outlook** for **Title**, select Today’s date for
    **Start Date**, select 10 days from today for **End Date** and click
    **Save**.

8.  Click on the back button.

9.  Click on the **Regarding** field and select the record you just created.

10. Close the **Dynamics 365** pane.

11. Navigate <https://web.powerapps.com/> and make sure you are not in the
    default environment.

12. Select Apps.

13. Select **Knowledge Admin** and click **Play**.

14. Click on the **Site Map** button and select **Assessments**.

15. The record you created in **Dynamics 365 App for Outlook** should be in this
    list.
