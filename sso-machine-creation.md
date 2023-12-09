Dear,

Happy to follow next step to setup SSO and Machine.

## BioStudio SSO and Machine Configuration

**SSO:**

**1]** Login to the admin Dashboard using admin credentials.
 Please refer to the link below.

```R
http://<Your BioStudio URL>/dashboard
https://<Your BioStudio URL>/dashboard
```

**2]** Do the **account registration** for Admin login.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar.png" class="lazy" width="100%">


**3]** Create an Admin Account by clicking on **Account Registration**.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ar1.png" class="lazy" width="100%">


**4]** Login to the dashboard using the Admin account that we registered via the create admin account step.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/lg.png" class="lazy" width="100%">

**5]** Admin portal setting will appear on the **left hand side menu**. Please click on **SSO**. Then select **+ Add New SSO**.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ans.png" class="lazy" width="100%">

**6] SSO** set up.

Select the protocol that you wish to set up and add some **dummy** values to the **mandatory** field. That we will change once we have the correct values after setting up the **callback** URL with **Idp**. Copy the callback URL and click on "Submit.

**NOTE:** SSO configuration should be saved by clicking the **Submit** button, as its value would be changed each time. Once clicked,  add a new SSO.

- You can have two callback URLs. I hope the SSL certificate is already setup for the BioStudio domain and the HTTPS callback URL can be used. Copy the callback URL based on configuration and set it up with IDP.

- BioStudio supports three types of protocols (SAML, OPENID, and OAUTH2) with all types of service providers.

[SSO Set up](https://studio.bioturing.com/document/installation#p-stylecolor-000080-sso-set-up-p)


<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/sso.png" class="lazy" width="100%">

**7]** Update SSO setting.

Once set up the Callback URL with IDP. Get all mandatory values and update SSO settings. 
<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/usso.png" class="lazy" width="100%">

```R
     --> Login to admin dashboard. https://<Your Domain>/dashboard
     --> Select SSO and click on three dots on Action tab.
     --> Click on Update SSO.
     --> Replace dummy values with correct values and set up other values like Allow 
```
SSO domains and save the configuration.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ssco.png" class="lazy" width="100%">


## Machine Creation:

Machine Creation: In order to create workspace for the user and save data. We need to create machine and volume. Detail are in link below.

https://studio.bioturing.com/document/installation#machine-creation

**1]** Log to the admin dashboard.

```R
– Click on Machine settings on the left hand side menu.
– We can give any name to the machine 
– IP address: this is a private IP of the server. You can get this from the command below.
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/crm.png" class="lazy" width="100%">

```R
docker exec bioproxy cat /etc/hosts
```

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/h.png" class="lazy" width="100%">

**2]** fill all mandatory Make it **Available** by enabling it. Click on **Submit** button to save this setting.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/crm2.png" class="lazy" width="100%">

**3]** Volume creation.

**Volume Creation:**

– Once machine creation is completed. Click on **+ plus** sign of volume tab to create volume.
– We can use any name for Volume name.
– Volume path would be **/home**
– Make it **Available** by enabling it.
– Click on **Submit** button to save this configuration.

<img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/adv1.png" class="lazy" width="100%">

**Testing**

User Testing:
Below is the user credential for testing. It will work without SSO configuration.


User Name: tester@bioturing.com
Password: XXXXXXXXXXXX

Thank you so much for your continued support for us in this setup. Feel free to contact us if you need any support or have any questions for us.

Best regards,
