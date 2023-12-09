## Dashboard training 

**What is a Dashboard in BioStudio?**

The BioStudio web administrator page serves as a centralized hub for managing the various components of the application, allowing authorized individuals to keep the site running smoothly and securely.

Dashboard is a place where administrators can perform all administrative tasks.

**How to login with Dashboard?**

BioStudio admin portal can be opened by adding /dashboard to domain name in URL.

`https://<Domain Name>/dashboard`

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/emailtemp-pic/dash.png" class="lazy" width="100%"><br><br>

**What is a Account Registration?**

The admin user must register the account first to have admin login and admin privileges. It can only be performed by a superuser who has root admin credentials. It will create an admin user on the BioStudio system.

:bell: **Note**: You cannot create multiple Super Admin user’s accounts. It can only have one super admin user in the BioStudio system and it is only a one-time activity. Then you can create multiple admin users based on their roles.


<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar.png" class="lazy" width="100%"><br>

**Create Admin Account.**

- **Root Password** : This is the password we used to provide during installation.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar1.png" class="lazy" width="100%"><br>

**What is inside dashboard?**

Admin dashboard can view and perform activities below.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/admin_menu.png" class="lazy" width="30%"><br>

- **Overview**: provides a comprehensive view of all activities in your BioStudio system.

- **SSO**: displays all current Single Sign-On (SSO) protocols supported in your BioStudio system. You can also add new SSO protocols to expand your options.

- **Users**: allows you to manage all users in your BioStudio system. When you enter this tab, you will see a table displaying the details of each user.

- **Admin**: contains all accounts set as administrators. New accounts can be added to this tab to grant administrative privileges. Additionally, you can assign specific roles to each admin account, such as super administrator or content, user, technique, or security roles.

- **Machines**: shows all servers currently in use by your BioStudio system with detailed information such as machine names, IP addresses, and status.

- **Forward Port**: allows you to configure port forwarding for your BioStudio system.

- **System Settings**: enables you to access and modify your BioStudio system’s settings. License information is also stored in this tab, along with other system-wide configurations.

- **Help Center**: If you face any troubles while managing the system, you can send system log files to BioTuring for the purpose of debugging the application. Your data will be kept secure and confidential.

**Note:** Some of setting, we already performed during installation and should not do any changes.

**Admin Tab:**

It used to create multiple admin user accounts based on their roles. They can login to the dashboard with limited rights.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/adminp.png" class="lazy" width="100%"><br>

**How to activate and deactivate accounts?**

Super admin can enable or disable that button to change status. A super admin can edit and delete the accounts.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/status.png" class="lazy" width="100%"><br>


**BioStudio usage and activities:**

BioStudio usage and activity graphs can be deployed automatically based on usage and activities. CPU, RAM, DISK, PROCESS resources, and USER ACTIVITY are all included.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/acti.png" class="lazy" width="100%"><br>

**BioStudio usage and activities:**

A graph will help users see the activities and take appropriate actions.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ua.png" class="lazy" width="100%"><br>

**BioStudio usage and activities:**

Clicking on the dot will give more information about user activities.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/acti1.png" class="lazy" width="100%"><br>

**BioStudio System Setting:**

BioStudio provides super admin control and actions related to the system under the System Setting tab.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/systemset.png" class="lazy" width="100%"><br>

:low_brightness: **Email SMTP**

It used to set up a client SMTP email server, and this facility used to send an email based on process or task completion.

:low_brightness: **Restart BioStudio**

When we execute processes that take longer, it's possible that they hold resources for a long time and create zombie processes. It used to clean the hold process and start the BioStudio application.

:low_brightness: **Release Notes**

We keep improving, updating BioStudio, and releasing new versions. Clients can review the release notes to see what has changed with the new release.

:low_brightness: **Check BioStudio**

It used to check the BioStudio websocket status.

**BioStudio login:**

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/lgin.png" class="lazy" width="100%"><br>

*For every successful login, BioStudio automatically creates a user entry on the Users tab to maintain their usage and status. A user's account can be activated or deactivated by changing its status.*

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ustat121.png" class="lazy" width="100%"><br>
<br>
 
For more information, please contact us at support@bioturing.com.