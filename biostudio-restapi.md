# BioStudio API

BioStudio is providing a great feature to test API calls with the BioStudio application.

## BioStudio Restful API for admin.

We are providing a Restful API for admins to test requests and responses.
There are a variety of checks that can be performed by admin, those are illustrated below.

:o: **Steps to open BioStudio API**

:one: Login to Admin dashboard. `https://<BioStudio Domain Name>/dashboard`
:two: click to System settings
:three: Click to `OpenAPI Configuration` :link: <strong style="color:skyblue;">View API Documentation</strong>

<br><img alt="rest api" src="/NEW_IMG/api-link.png" class="lazy" width="100%"><br>

<br><img alt="rest api" src="/NEW_IMG/restapi-home.png" class="lazy" width="100%"><br>

:bell: **Note** Please click on the `Try It Out` button to enable the input parameter field.

<br><img alt="rest api" src="/NEW_IMG/try-out.png" class="lazy" width="100%"><br>

**Admin API token :** This is a (mask) key that is available to be copied from the admin dashboard in the system settings.

<br><img alt="rest api" src="/NEW_IMG/rest-apikey.png" class="lazy" width="100%"><br>

:o: **SSO Setting**

It used to check get response with BioStudio Domain.
:small_blue_diamond: Click on the SSO setting: Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/exec.png" class="lazy" width="100%"><br>

Result:

<br><img alt="rest api" src="/NEW_IMG/sso-resp.png" class="lazy" width="100%"><br>

:o: System management

It is used to test the SMTP information setting response.

:small_blue_diamond: Click on the System management : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/smtp.png" class="lazy" width="100%"><br>

:o: Restart server API

It is used to restart sever using API.

:small_blue_diamond: Click on the Restart server : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/rserver.png" class="lazy" width="100%"><br>

Similarly, you can check the server status.

:o: **Group**

It used to get information related to group.

:small_blue_diamond: Click on the Groups : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/groups.png" class="lazy" width="100%"><br>

:o: **Machines**

It used to get information related to machine.

:small_blue_diamond: Click on the Machines : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/machine.png" class="lazy" width="100%"><br>

:o: **Summary**

It used to Get information about the number of users and the usage of notebooks.

:small_blue_diamond: Click on the Summary : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/summary.png" class="lazy" width="100%"><br>

:o: **Activities**

It used to Get information about service
Metric {1: CPU, 2: RAM, 3: DISK, 4: MEMORY, 5: TIME ON SITE, 11: ACTIVITIES}

:small_blue_diamond: Click on the Activities : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/activities.png" class="lazy" width="100%"><br>

:o: **Token info**

It used to Get Token information.

:small_blue_diamond: Click on the Token info : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/token.png" class="lazy" width="100%"><br>

:o: **Users**

It used to Get list user info by page.

:small_blue_diamond: Click on the Users : Expand Operation button, which is located on the left side.
:small_blue_diamond: Copy the admin API token from System Settings on the admin dashboard.
:small_blue_diamond: Fill out all necessary parameter values.
:small_blue_diamond: Click to execute to see the response result.

<br><img alt="rest api" src="/NEW_IMG/users.png" class="lazy" width="100%"><br>