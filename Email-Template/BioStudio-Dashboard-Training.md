## Dashboard training 

**What is a Dashboard in BioStudio?**

```R
The BioStudio web administrator page serves as a centralized hub for managing the various components of the application, allowing authorized individuals to keep the site running smoothly and securely.

Dashboard is a place where administrators can perform all administrative tasks.
```

**How to login with Dashboard?**

```R
BioStudio admin portal can be opened by adding /dashboard to domain name in URL.

https://<Domain Name>/dashboard.
```

<img alt="Protocol" src="https://cdn.bioturing.com/documentation/emailtemp-pic/dash.png" class="lazy" width="100%"> 



**What is a Account Registration?**

```R
The admin user must register the account first to have admin login and admin privileges. It can only be performed by a superuser who has root admin credentials. It will create an admin user on the BioStudio system.

Note: You cannot create multiple Super Admin user’s accounts. It can only have one super admin user in the BioStudio system. It is only a one-time activity. Then you can create multiple admin users based on their roles.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar.png" class="lazy" width="100%">

**Create Admin Account.**

- Root Password : This is the password we used to provide during installation.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar1.png" class="lazy" width="100%">

**What is inside dashboard?**

Admin dashboard can view and perform activities below.

- **Overview**: provides a comprehensive view of all activities in your BioStudio system.

- **SSO**: displays all current Single Sign-On (SSO) protocols supported in your BioStudio system. You can also add new SSO protocols to expand your options.

- **Users**: allows you to manage all users in your BioStudio system. When you enter this tab, you will see a table displaying the details of each user.

- **Admin**: contains all accounts set as administrators. New accounts can be added to this tab to grant administrative privileges. Additionally, you can assign specific roles to each admin account, such as super administrator or content, user, technique, or security roles.

- **Machines**: shows all servers currently in use by your BioStudio system with detailed information such as machine names, IP addresses, and status.

- **Forward Port**: allows you to configure port forwarding for your BioStudio system.

- **Settings**: enables you to access and modify your BioStudio system’s settings. License information is also stored in this tab, along with other system-wide configurations.

- **Help Center**: If you face any troubles while managing the system, you can send system log files to BioTuring for the purpose of debugging the application. Your data will be kept secure and confidential.

**Note:** Some of setting, we already performed during installation and should not do any changes.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/menuf.png" class="lazy" width="100%">

**Admin Tab:**

```R
It used to create multiple admin user accounts based on their roles.
They can login to the dashboard with limited rights.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/adminp.png" class="lazy" width="100%">

**How to activate and deactivate accounts?**

```R
Super admin can enable or disable that button to change status. A super admin can edit and delete the accounts.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/status.png" class="lazy" width="100%">


**BioStudio usage and activities:**

```R
BioStudio usage and activity graphs can be deployed automatically based on usage and activities. CPU, RAM, DISK, PROCESS resources, and USER ACTIVITY are all included.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/acti.png" class="lazy" width="100%">

**BioStudio usage and activities:**

```R
A graph will help users see the activities and take appropriate actions.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ua.png" class="lazy" width="100%">

**BioStudio usage and activities:**

```R
Clicking on the dot will give more information about user activities.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/acti1.png" class="lazy" width="100%">

**BioStudio System Setting:**

```R
BioStudio provides super admin control and actions related to the system under the System Setting tab.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/systemset.png" class="lazy" width="100%">

:low_brightness: **Email SMTP**

```R
It used to set up a client SMTP email server, and this facility used to send an email based on process or task completion.
```

:low_brightness: **Restart BioStudio**

```R
When we execute processes that take longer, it's possible that they hold resources for a long time and create zombie processes. It used to clean the hold process and start the BioStudio application.
```

:low_brightness: **Release Notes**

```R
We keep improving, updating BioStudio, and releasing new versions. Clients can review the release notes to see what has changed with the new release.
```
:low_brightness: **Check BioStudio**

```R
It used to check the BioStudio websocket status.
```

**BioStudio login:**

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/lgin.png" class="lazy" width="100%">

*For every successful login, BioStudio automatically creates a user entry on the Users tab to maintain their usage and status. A user's account can be activated or deactivated by changing its status.*

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ustat121.png" class="lazy" width="100%">
<br>
<br>

For more information, please contact us at support@bioturing.com.