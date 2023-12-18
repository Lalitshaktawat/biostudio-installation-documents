![BioStudio logo](https://cdn.bioturing.com/documentation/idiag/logo.png)

# <p> <span style="color:blue"> Installation Steps: </span> <span style="color:green"> BioTuring BioStudio </span> </p>

## Introduction

>**Software to tackle biomedical challenges:**

<div class="warning" style='background-color:#E9D8FD; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<code><b>Colaboratory</b></code> , or <code><b>BioStudio</b></code> for short, is a product from <b style="color: darkblue"><u>Bioturing</b></u>.<code><b>BioStudio</b></code> has a variety of features and <b style="color: black"> pre-built notebooks </b>, for user to download and use. We are providing all types of user friendly <b style="color: black"> tools </b> that helps, users to post their data and analyze the reports. Our product can be used to write and execute arbitrary python, R code, Golang, Julia, RStudio, VS Code and many more through the browser, and is especially well suited to data analysis and education. More technically, <b> BioStudio </b> is a hosted Jupyter notebook service that requires no setup to use. <b style="color: black"> Users can build their own notebook based on their requirements</b>.

**We are keep adding new features and functionalities to BioStudio.**
</p>
</span>
</div>


# System Requirements

>**Before installing the BioStudio, some pre-installation steps are required:**

|| **Basic recommendation**| **Optional**|
|---------------------|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| **CPU**             | <strong style="color:red;">16 core</strong>| This is basic requirement to start  BioStudio and based on requirement, Resources as well as machine can be added.  |
| **RAM**             | <strong style="color:red;">64 GB</strong> | As above                                                                                                           |
| **HDD**             | / partition can be 100 GB | As above.                                                                                      |
|                     | Data Volume : 1TB| As above.                                                                                                |
| **OS**              | Any OS. Ubuntu 20.04 and above.| BioStudio is more supportive with Linux OS. For better performance linux OS is recommended.|
| **AWS Instance**    | Support any type of instance type. Depend on needs| AWS <strong style="color:red;">g5.4xlarge</strong> in case using GPU.                                          |
|**Platform**         | Docker / Kubernetes                                                                                                        |

<br/>

| **Note**            |                                                                                                                   |
|---------------------|-------------------------------------------------------------------------------------------------------------------|
|                     | In case we want to use **GPU** based **Notebooks** with BioStudio. We need to install NVIDIA and below would be a requirement.        |
|                     | The system has one or multiple NVIDIA GPU(s) (at least 16 GB memory per GPU) - with Turing architecture or above. |
|                     | BioStudio supports any Linux OS. We are recommending Ubuntu 20.04 or above.                                        |
|                     | SSL can be configured later also.                                                                                 |
|                     | Please contact support@bioturing.com to get the token for your company.                                           |
|                     |                                                                                                                   |
| **Security**        |                                                                                                                   |
|                     | The BioStudio platform uses HTTPS protocol to securely communicate over the network.                               |
|                     | All of the users need to be authenticated using a BioTuring account or the company's **SSO** to access the platform.      |
|                     | We highly recommend setting up a private VPC network for IP restriction.                                          |
|                     | The data stays behind the company firewall.                                                                       |
|                     | The BioStudio platform does not track any usage logs.                                                              |
|                     |                                                                                                                   |
| **Data visibility** |                                                                                                                   |
|                     | Data can be uploaded to Personal Workspace or Data Sharing group.                                                 |
|                     | In the Personal Workspace, only the owner can able to see and manipulate the data she/he uploaded.                        |
|                     | In the Data Sharing group, only people in the group can able to see the data.                                             |
|                     | In the Data Sharing group, only people with sufficient permissions can able to manipulate the data.                       |

## Network requirements

| Domain                                                           | Explain                                                            |
|------------------------------------------------------------------|--------------------------------------------------------------------|
| *.bioturing.com                                                  | We need to retrieve data from the BioTuring ecosystem server.      |
| *.anaconda.org                                                   | We need to retrieve packages from the Anaconda server.             |
| *repo.anaconda.com                                               | We need to retrieve packages from the Anaconda repo server.        |
| Amazon S3                                                        | We need to retrieve resources from the BioTuring ecosystem server. |
| github.com                                                       | We need to retrieve packages from the Github.                      |
| cdn-eu-west-1.s3.eu-west-1.amazonaws.com (euro -west1)           | We need to retrieve packages from the CDN.                         |
| s3.us-west-2.amazonaws.com/cdn.bioturing.com (us -west2)         | We need to retrieve packages from the CDN.                         |
| cdn.bioturing.com (us -west2)                                    | We need to retrieve packages from the CDN.                         |


:point_right: **Please contact** :email: [support@bioturing.com](mailto:support@bioturing.com) to get the **token** for your company.

<div class="warning" style='background-color:#E9D8FD; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<span style='font-size:20px;'>&#128276;</span> <b>Note:</b> Our software can be installed with minimum capacity of instance / server. The ideal system that we recommend for most companies is <b style="color: black">  AWS c5a.8xlarge</b> for <b style="color: black"> CPU </b> based. Instance can be chosen based on requirement. If the notebook is based on GPU, we can select GPU based instance.
Our Product is containerized based applications. Kindly select the machine based on your requirements. <b style="color: black"> BioStudio </b> can be run on <b style="color: black"> Docker </b> using Docker engine and <b style="color: black"> Kubernetes</b>.

<b style="color: purple">:sparkles: <u>Important note</u> :sparkles::</b> We can install <b style="color: black"> BBrowserX talk2data (Bioturing ecosystem)</b> :link: [BBrowserX](https://github.com/bioturing/bbrowserx-wiki/wiki/Installation-guide) and <b style="color: black"> BioStudio </b> on the same server. Installation process is the same to run our <b>installation script</b> for <b>BioStudio</b>. Step by step Instructions to install BioStudio are given below. Only changes on domain name for BioStudio. <b>Kindly do not use BBrowserX talk2data domain name during this installation, In case you are planing to install BBrowserX and BioStudio on same machine.</b>

:dizzy: <b>BioStudio token can be updated later, after installation</b>.
:dizzy: <b>Contact point to get BioStudio token is</b> :email: [support@bioturing.com](mailto:support@bioturing.com)
:dizzy: <b>SSL certificate can be installed later, If BioStudio planned to install on separate instance.</b>

User can access <b>BioStudio application using two ways</b>, In case installed BBrowserx and BioStudio on the <b>same machine</b>.

:one: Browse the BioStudio application `https://<BioStudio Domain name>` , If you have SSL certificate for BioStudio domain and configured with Nginx else use http protocol.
:two: Use BioStudio Desktop application - using IP address.

<b>Bioturing Launcher</b> :link: [Desktop Application](https://colablocal.bioturing.com/document/bioturing-launcher)

:bell:If <b>BioStudio</b> will install on separate server. BioStudio can be accessed using any browser by <b>IP address</b> or <b>Domain name</b>.
</p>
</span>
</div>


# Download and Install 
> **Note:** We suggest starting from scratch to avoid package/driver conflicts. For Tag naming conversion, kindly select based on your architecture.

# New Server Set up on AWS.

:large_orange_diamond: Login to AWS console with admin user account to launch an EC2 instance.

**Note:** It’s up to the client. How they are going to manage infrastructure, Load, Network, Access and traffic …etc.

## Create a VPC
:link: [Amazon VPC guide](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)

:link: [VPC Creation guide](https://docs.aws.amazon.com/vpc/latest/userguide/create-vpc.html)

<br>

:large_orange_diamond: Search **VPC** on the search box.

<br><img alt="VPC Search" src="https://cdn.bioturing.com/documentation/idiag/VPC-Search.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: Select the appropriate **region** for VPC.

<br><img alt="Region Selection" src="https://cdn.bioturing.com/documentation/idiag/region-selection.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: Click on **Create VPC.*


<br><img alt="Create VPC" src="https://cdn.bioturing.com/documentation/idiag/Create_VPC1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Fill-out **Name tag** , **IPv4 CIDR** block details.

<br><img alt="Create VPC fill" src="https://cdn.bioturing.com/documentation/idiag/Create-VPC2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Mentioned **Tags** and select **Create VPC** push button.

<br><img alt="Create VPC click" src="https://cdn.bioturing.com/documentation/idiag/Create-VPC3.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Verify** VPC creation successfully completed.

<br><img alt="VPC creation succeed" src="https://cdn.bioturing.com/documentation/idiag/VPC-Created-Successfully.png" class="lazy" width="100%"><br>

## Create a Subnet

:large_orange_diamond: Time to create Subnet. Click on **Create subnet.**
<br><img alt="Create Subnet" src="https://cdn.bioturing.com/documentation/idiag/Create-subnet1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **VPC ID** and type **Subnet name.**

<br><img alt="Create Subnet fill" src="https://cdn.bioturing.com/documentation/idiag/Create-subnet2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Fill **CIDR block**, type **Tag Key** and **Value** then Click on **Create subnet.**

<br><img alt="Create Subnet fill CIDR" src="https://cdn.bioturing.com/documentation/idiag/Create_subnet-3.png" class="lazy" width="100%"><br>

:large_orange_diamond: Subnet created successfully.

<br><img alt="Subnet Succeed" src="https://cdn.bioturing.com/documentation/idiag/Subnet-created-successfully.png" class="lazy" width="100%"><br>

:large_orange_diamond: Check **Subnet** detail.

<br><img alt="Subnet Detail" src="https://cdn.bioturing.com/documentation/idiag/Subnet-detail.png" class="lazy" width="100%"><br><br>

## Create Internet Gateway

> **Note:** As noticed. During Subnet creation :arrows_clockwise: Router table was automatically created.

:o: Time to create **Internet Gateway.**

:large_orange_diamond: **Router Table.**

<br><img alt="Subnet Detail" src="https://cdn.bioturing.com/documentation/idiag/Router_table.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **Internet gateway** and Click on **Create internet gateway**.

<br><img alt="internet gateway creation" src="https://cdn.bioturing.com/documentation/idiag/Create-IG.png" class="lazy" width="100%"><br>


:large_orange_diamond: Fill **Name Tag**, **Key** and **Value** then Click **Create internet gateway.**

<br><img alt="IG creation step" src="https://cdn.bioturing.com/documentation/idiag/Create-IG1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Internet gateway created successfully.

<br><br><img alt="IG creation Succeed" src="https://cdn.bioturing.com/documentation/idiag/IG-Created-success.png" class="lazy" width="100%"><br><br>


## **Internet Gateway** attached to VPC.

:large_orange_diamond: In Internet gateway Click on **Action** and select **Attached to VPC.**

<br><br><img alt="IG attached to VPC" src="https://cdn.bioturing.com/documentation/idiag/IG-Attached-to-vpc1.png" class="lazy" width="100%"><br><br>
<img alt="IG attached to VPC done" src="https://cdn.bioturing.com/documentation/idiag/Attached-to-vpc2.png" class="lazy" width="100%"><br><br>
<img alt="IG attached to VPC done" src="https://cdn.bioturing.com/documentation/idiag/Attached-to-vpc-final-step.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Internet Gateway** attached to VPC completed.

<br><img alt="IG attached to VPC done" src="https://cdn.bioturing.com/documentation/idiag/IG-attached-to-vpc-done.png" class="lazy" width="100%"><br>

:large_orange_diamond: Now Update Route Table for **Subnet association** and add **Route** to use Internet gateway to router table.

:large_orange_diamond: Update **Route Table** for **Subnet association.**

## Subnet association to Router Table.

:large_orange_diamond: Select **Subnet associations** from **Route tables** :arrow_forward: Second tab.

<br><img alt="Subnet association selection" src="https://cdn.bioturing.com/documentation/idiag/Subnet_associated-with-router.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Edit subnet associations** and select Subnet name, which you would like to associate then Click on **Save associations** button.

<br><img alt="Subnet association done" src="https://cdn.bioturing.com/documentation/idiag/Subnet_associated_save.png" class="lazy" width="100%"><br>

:large_orange_diamond: Subnet association completed.

<br><img alt="Association success" src="https://cdn.bioturing.com/documentation/idiag/Subnet_associated_success.png" class="lazy" width="100%"><br>

## Update Router table to use Internet gateway.

:large_orange_diamond: Select **Routes** from **Route tables** :arrow_forward: First tab.

:large_orange_diamond: Click on **Edit routes.**

<br><img alt="IG to Route step1" src="https://cdn.bioturing.com/documentation/idiag/Ig-to-Router1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Fill the value **0.0.0.0/0** and select Internet gateway name as showing on below screenshot.

:large_orange_diamond: Click on **Save change.**

<br><img alt="IG to Route step2" src="https://cdn.bioturing.com/documentation/idiag/Ig-to-Router2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Router table updated.

<br><img alt="IG to Route step2" src="https://cdn.bioturing.com/documentation/idiag/Ig-to-Router3.png" class="lazy" width="100%"><br>

## Create ec2 Instance

:large_orange_diamond: Click on Search Bar and type ec2.

<br><img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/ec2-search.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **instances (running).**

<br><img alt="ec2 instance" src="https://cdn.bioturing.com/documentation/idiag/instance1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Launch instances.**

<br><img alt="ec2 launch" src="https://cdn.bioturing.com/documentation/idiag/Launch-in1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Type **name** of instance.

<br><img alt="ec2 name" src="https://cdn.bioturing.com/documentation/idiag/In2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **Operating System.** Here, We are selecting **ubuntu.**

<br><img alt="ec2 os" src="https://cdn.bioturing.com/documentation/idiag/In4.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **g5.8xlarge** instance.

:mag: Select instance type based on your requirements.

<br><img alt="ec2 Instance type" src="https://cdn.bioturing.com/documentation/idiag/In5.png" class="lazy" width="100%"><br>

:large_orange_diamond: Create a **Keypair** to connect to ec2 instance. Type **Key pair name** and Click on **Create key pair.**

<br><img alt="ec2 Key pair" src="https://cdn.bioturing.com/documentation/idiag/In6-keypair 002.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Key pair** will download.

<br><img alt="ec2 Keypair download" src="https://cdn.bioturing.com/documentation/idiag/keypair-download.png" class="lazy" width="100%"><br>

:large_orange_diamond: On the **Network settings** select correct **VPC** and **Subnet ID**

<br><img alt="ec2 Netset" src="https://cdn.bioturing.com/documentation/idiag/select_subnet.png" class="lazy" width="100%"><br>

:large_orange_diamond: On the **firewall (Security groups)** section. Create new security group by giving appropriate name.

<br><img alt="ec2 SG" src="https://cdn.bioturing.com/documentation/idiag/Security-GR1.png" class="lazy" width="100%"><br>


:large_orange_diamond: Allow **SSH** , **HTTP** and **HTTPS**. Source will be **0.0.0.0/0**.

<br><img alt="ec2 Sg1" src="https://cdn.bioturing.com/documentation/idiag/Security-GR2 002.png" class="lazy" width="100%"><br>

:o: **Configure Storage**

:large_orange_diamond: **Root Volume is 100GB**

:large_orange_diamond: **EBS Volume is 1000GB ~ 1TB**

<br><img alt="ec2 Storage" src="https://cdn.bioturing.com/documentation/idiag/Security-GR3andDisk.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Launch instance.**

<br><img alt="ec2 final step" src="https://cdn.bioturing.com/documentation/idiag/launch_instance1-final-step.png" class="lazy" width="100%"><br>

:large_orange_diamond: Instance creation will be **in progress.**

<br><img alt="ec2 Launched" src="https://cdn.bioturing.com/documentation/idiag/Instance_Created.png" class="lazy" width="100%"><br>

## Assign Elastic IP to instance

:large_orange_diamond: Click on **Elastic IPs** and Click on **Allocate Elastic IP address.**

<br><img alt="Elastic IP assign step1" src="https://cdn.bioturing.com/documentation/idiag/Easltic-ip1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **Network Boarder Group** and take Elastic IP address.

<br><img alt="Elastic IP assign step1" src="https://cdn.bioturing.com/documentation/idiag/ElasticIp2.png" class="lazy" width="100%"><br>

<img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/ElasticIpAllocate.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Associate Elastic IP address.**

 <br><img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/EasticIP-allocated.png" class="lazy" width="100%"><br> 

<img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/EaslticIP_all1.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **Instance** and **Private IP address.**

<br><img alt="ec2 Assign" src="https://cdn.bioturing.com/documentation/idiag/EaslticIP_all2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Associate.**

<br><img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/EaslticIP_all3 002.png" class="lazy" width="100%"><br>

:large_orange_diamond: Elastic IP address associated successfully.

<br><img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/EaslticIP_all5.png" class="lazy" width="100%"><br>

:large_orange_diamond: Take connection string and **SSH** to **ec2 Instnace.**

<br><img alt="ec2 search" src="https://cdn.bioturing.com/documentation/idiag/Connecting-string.png" class="lazy" width="100%"><br>

## Installation Started.

```R
# Copy the connection string. Use SSH key pair and connect to ec2 instance.
ssh -i "lalit-biocolab-keypair.pem" ubuntu@3.98.231.253
```

```R
# Before start installation. Kindly create below path.
```


| **Item**                 | **Note**                                                             | **Size**          |
|--------------------------|----------------------------------------------------------------------|-------------------|
| BioStudio Token          | To access our product.                                               |                   |
| Application Domain       | Access BioStudio on Browser.                                         |                   |
| META_DATA Volume         | This will use by Bioproxy to store database. [**/biocolab/metadata**]| 50GB              |
| SSL Volume               | Using by BioProxy. [**/biocolab/configs**]                           | 1GB or above      |
| Data Volume              | Using to store user data. [**/biocolab/userdata**]                   | 500GB or above    |
| Application data Volume  | Used to store application binary data.[**/biocolab/appdata**]        | 100GB or above    |
| Ethernet IP Address      | Use to pass IP address during installation (**eth0**)                |                   |

Run the **install.biocolab.docker.sh** script for docker environment and install require software.

---

```R
# Create required folder structure before execution.
mkdir -p /biocolab/metadata
mkdir -p /biocolab/configs
mkdir -p /biocolab/userdata
mkdir -p /biocolab/appdata

# Switch to /biocolab folder.
cd /biocolab

# Download script:
# Note: Installation script version would be changed based on updates.
# Our Team will get you updates and keep in touch with you during installation.

wget https://github.com/bioturing/installation/archive/refs/tags/V2.0.53.tar.gz

# uncompressed .gz
tar xvf V2.0.53.tar.gz

# Switch to installation folder
cd installation-2.0.53/

# Execute installation script
bash install.biocolab.docker.sh

# Verify both container up and running.
docker ps -a

# Configure SSO login
http://<Your Domain>/dashboard/
```

:large_orange_diamond: Download **V2.0.53.tar.gz**, which content script to install **BioStudio.**

<br><img alt="wget-script" src="https://cdn.bioturing.com/documentation/idiag/install-step1.png" class="lazy" width="100%"><br>

---

:bell: During execution of this script, It will prompt for input credential. Kindly note that user name is **admin** and keep store the **password** safely, which you are going to input. It needed to be performed admin activities.  

---

:large_orange_diamond: Execute **script.**

<br><img alt="Script execution" src="https://cdn.bioturing.com/documentation/idiag/install-step2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Follow **execution** script's instructions and input values accordingly.

<br><img alt="step1-provideinfo" src="https://cdn.bioturing.com/documentation/idiag/install-step4.png" class="lazy" width="100%"><br>

:large_orange_diamond: Change the IP, **If we have many.**

<br><img alt="Installation-step2" src="https://cdn.bioturing.com/documentation/idiag/Installation-step2.png" class="lazy" width="100%"><br>


<div class="warning" style='background-color: LightGray; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<code><b>BioProxy version : 1.0.26</b></code> 
<code><b>BioColab version : 2.0.50</b></code> 
</p>
</span>
</div>

```R
# Please provide the version based on Bioturing instruction.
# It would be vary based on updates. 
```

:large_orange_diamond: Verify both **container status - UP and running.**

<br><img alt="docker-image" src="https://cdn.bioturing.com/documentation/idiag/docker-image.png" class="lazy" width="100%"><br>

:large_orange_diamond: Browser **BioStudio.**

```R
# https://<Domain name>
```

:watch: **Kindly wait for a while. BioStudio software will take time to download packages and install.**


<br><img alt="brows-site" src="https://cdn.bioturing.com/documentation/idiag/brows-site.png" class="lazy" width="100%"><br>

## Register for **root admin**.

```R
https://<your domain>/dashboard
# It will prompt for Admin Login.
# Select Account Registration.
# Create admin account.
# Root Password is the one, we provided during installation.
# Login with the Dashboard using that account you registered earlier.
```

:large_orange_diamond: **Account Registration.**

<br><img alt="registration-admin-account" src="https://cdn.bioturing.com/documentation/idiag/reg-ad.png" class="lazy" width="100%"><br>

:large_orange_diamond: Crearte **Admin Account.**

<br><img alt="registration_form" src="https://cdn.bioturing.com/documentation/idiag/registration_form.png" class="lazy" width="100%"><br>

:large_orange_diamond: Login to **dashboard.**

```R
https://<your domain>/dashboard
```

<br><img alt="loin-admin" src="https://cdn.bioturing.com/documentation/idiag/loin-admin.png" class="lazy" width="100%"><br>

<div class="warning" style='background-color: LightGray; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<code><b> Workspace </b></code> <b style="color: darkblue">It is essential to create a machine and mount the volume before using the workspace.</b>
</p>
</span>
</div>

## Machine creation

```R
# Login with Dashboard using admin credential.
# Select Machines Tab form left-side menu.
# Select + Add New Machine.

Name: You can select any name to this machine. This is a private IP of your machine, That can be find in /etc/hosts file on BioStudio pods.

I already added a machine, so I will go with the update machine.
```

<img alt="Script execution" src="https://cdn.bioturing.com/documentation/idiag/mip.png" class="lazy" width="100%"><br>

:large_orange_diamond: Please fill out **Update machine metadata.**

<br><img alt="Machine update" src="https://cdn.bioturing.com/documentation/idiag/machine-update.png" class="lazy" width="100%"><br>

:large_orange_diamond: Please **add volume - Update machine Metadata.**

```R
# Machines --> Click on + sign to add volume.
# You can use any name for volume, but the volume path will always be /home.
# Workspace is now ready for use.
```

<br><img alt="Volume added" src="https://cdn.bioturing.com/documentation/idiag/volume-add.png" class="lazy" width="100%"><br>

# <p style="color: #000080"> SSO Set up </p>

> **We are supporting three types of protocol below:**

| **PROTOCOLS** |
|---------------|
| SAML          |
| OPENID        |
| OAUTH2        |



:bell: **Please contact** :email: [support@bioturing.com](mailto:support@bioturing.com) to add :heavy_plus_sign: more  **protocols** and **types** , If you are not able to find in the list based on your choice. :blush: **We are always happy to add more variety of protocols and types.**


| **SAML : Identity and Access Management** |
|---------------|
| Aliyun IDaaS  |
| Keycloak      |
| Default       |

| OPENID : Identity and Access Management |
|-----------------------------------------|
| Default                                 |

| **OAUTH2 : Identity and Access Management** |
|---------------------------------------------|
| Adfs                                        |
| Amazon                                      |
| Apple                                       |
| Auth0                                       |
| AzureAD                                     |
| BattleNet                                   |
| Bilibili                                    |
| Bitbucket                                   |
| Box                                         |
| Casdoor                                     |
| CloudFoundry                                |
| Custom                                      |
| Dailymotion                                 |
| Deezer                                      |
| DigitalOcean                                |
| Discord                                     |
| Douyin                                      |
| Dropbox                                     |
| EveOnline                                   |
| Fitbit                                      |
| Gitea                                       |
| Google                                      |
| Heroku                                      |
| InfluxCloud                                 |
| Infoflow                                    |
| Instagram                                   |
| Intercom                                    |
| Kakao                                       |
| Lastfm                                      |
| Line                                        |
| Mailru                                      |
| Meetup                                      |
| MicrosoftOnline                             |
| Naver                                       |
| Nextcloud                                   |
| Okta                                        |
| OneDrive                                    |
| Oura                                        |
| Patreon                                     |
| Paypal                                      |
| SalesForce                                  |
| Shopify                                     |
| Slack                                       |
| Soundcloud                                  |
| Spotify                                     |
| Steam                                       |
| Strava                                      |
| Stripe                                      |
| TikTok                                      |
| Tumblr                                      |
| Twitch                                      |
| Twitter                                     |
| Typetalk                                    |
| Uber                                        |
| VK                                          |
| Wepay                                       |
| Xero                                        |
| Yahoo                                       |
| Yammer                                      |
| Yandex                                      |
| Zoom                                        |


## <p style="color: #000080"> SSO configuration </p>

:high_brightness: Login to **Dashboard** using **admin** credential.

:link: https://<**Domain Name**>/dashboard

:link: http://<**Domain Name**>/dashboard

:high_brightness: Select **SSO** on :arrow_left: left side menu.

:high_brightness: Click on :arrow_right: **+ Add New SSO** push button.

<br><img alt="New SSO" src="https://cdn.bioturing.com/documentation/SSO_IMG/new-sso.png" class="lazy" width="100%"><br>

:large_orange_diamond: **New SSO configuration.**

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/SSO_IMG/protocol.png" class="lazy" width="100%"><br>

| **Option**               | **Description**                                                                                                                                |
|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| **Protocol**             | Rules that you would like to select for SSO configuration. It could be SAML, OPENID or OAUTH2.                                       |
| **Default**              | If you are configuring - multiple SSO service providers. You can mark one of them to use as a default by enabling Default option.                              |
| **App name**             | Specified application name. You can provide any name.                                                                                          |
| **Display Name**         | Name that you would like to use for SSO configuration. You can provide any name.                                                               |
| **Allow SSO Domains**    | This option allow you to restrict access to an application. Only selected domain are allow to access this application. Kindly provide your domain name, if you wish to allow to access user's belongs to your domain.                       |
| **Callback HTTPS URL**   | We must use this URL to configure SSO, if BioStudio configured **with** SSL access. So that once Authentication Successful. User will allow to access BioStudio application.              |
| **Callback HTTP URL**    | We must use this URL to configure SSO, If BioStudio configured **without** SSL. So that once Authentication Successful. User will allow to access BioStudio application.            |
| **Type**                 | Select what type of IDP service provider you are going to use. value will be changed based on selected Protocol.                                 |
| **Subtype**              | If you have more type of IDP. Type vlaue in Subtype.                                                                                            |
| **Disable SSL**          | By default SSL is disabled. If you would like to auth. with server's keys. Enable it and you can have public and private key to configure SSO. |
| **Configuration by**     | You can select to provide value by manual, Ready from XML content or Ready from XML file URL.                                                    |
| **IDP SSO URL**          | Identity Provider SSO URL that you can get it from IDP.                                                                                        |
| **IDP Issuer URL**       | Identity Provider Issuer URL that you can get it from IDP.                                                                                     |
| **IDP x509 Public Cert** | Identity Provider certificate. That you can download or copy the content and provide it here.                                                       |

:bell: **Note:** Callback HTTPS URL, Callback HTTP URL is **not** static and will **change** each time for new SSO configuration for the same potocol. 

:closed_lock_with_key: **Solution**: We can provide **dummy values** to **mendatory fields** and **click** on **Submit** button to :floppy_disk: **save**. Once saved, We can provide **Callback URL** to **SSO IT department** for further configuration. Collect all required values after configuring Callback URL from IDP and configure it further by update SSO.


:large_orange_diamond: **SAML Protocol** 

```R
SAML is an XML-based authentication protocol in which Identity Providers (IdP) -- entities that manage and store user credentials -- exchange digitally signed XML documents (SAML Assertions) allowing an end-user to access a **Service Provider **(SP).
Here IDP could be Aliyum IDaas, KeyCloak, auth0, or any of IDP service provider, which come under default.
BioStudio is comes under service provider.
```

<br><img alt="saml config" src="https://cdn.bioturing.com/documentation/SSO_IMG/SSO-CONF.png" class="lazy" width="100%"><br>

:large_blue_diamond: **SAML Protocol Configured.** 

<br><img alt="saml saved" src="https://cdn.bioturing.com/documentation/SSO_IMG/SAML-SAVED.png" class="lazy" width="100%"><br>

:large_blue_diamond: **SAML Protocol view metadata.**

```R
# Once clicked on Submit button. You can view metadata by clicking + ( Plus sign)
```

<br><img alt="saml metadata" src="https://cdn.bioturing.com/documentation/SSO_IMG/SSOmetadata.png" class="lazy" width="100%"><br><br>

:large_blue_diamond: **SAML metadata.**

<br><img alt="saml metadata detail" src="https://cdn.bioturing.com/documentation/SSO_IMG/ssometada-desc.png" class="lazy" width="100%"><br><br>

:large_blue_diamond: **SAML Protocol update / delete method.** 

> You can update the values of an existing SSO configuration whenever you want by selecting the update option for SSO.

```R
# In Order to update or delete existing SSO configuration. Please follow steps are given below.
1. Login to the dashboard using Admin credential.
2. Select SSO option available on left side menu.
3. Select SSO Application -- Action three DOTS to select your choice to update or delete.
```

```R
# option - Action.
```

<br><img alt="saml update" src="https://cdn.bioturing.com/documentation/SSO_IMG/SMAL-update.png" class="lazy" width="100%"><br>

```R
# option - Update.
```

<br><img alt="saml update" src="https://cdn.bioturing.com/documentation/SSO_IMG/update-sson.png" class="lazy" width="100%"><br>

```R
# option - Delete.
```



<br><img alt="saml delete" src="https://cdn.bioturing.com/documentation/SSO_IMG/delete-sson.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: **OPENID Protocol.**

```R
OpenID Connect is an interoperable authentication protocol based on the OAuth 2.0 framework of specifications (IETF RFC 6749 and 6750). It simplifies the way to verify the identity of users based on the authentication performed by an Authorization Server and to obtain user profile information in an interoperable and REST-like manner.
```

:large_blue_diamond: **OPENID configured.**

<br><img alt="Open ID" src="https://cdn.bioturing.com/documentation/SSO_IMG/openid.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: **OAUTH2 Protocol.**

```R
The OAuth 2.0 is the industry protocol for authorization. It allows a user to grant limited access to its protected resources. Designed to work specifically with Hypertext Transfer Protocol (HTTP), OAuth separates the role of the client from the resource owner. The client requests access to the resources controlled by the resource owner and hosted by the resource server. The resource server issues access tokens with the approval of the resource owner. The client uses the access tokens to access the protected resources hosted by the resource server.
```

> We are providing all type of IDP's to configure SSO using OAUTH2. List is given above.


:large_blue_diamond: **OAUTH2 configured with Google.**

<br><img alt="Oauth2 detail google" src="https://cdn.bioturing.com/documentation/SSO_IMG/oauth2google.png" class="lazy" width="100%"><br><br>


:large_blue_diamond: **OAUTH2 configured with Azure.**

<br><img alt="Oauth2 detail Azure" src="https://cdn.bioturing.com/documentation/SSO_IMG/OAUTH2Azure.png" class="lazy" width="100%"><br><br>

> In above explanation, We configured four types of SSO. It will appears to users during login to decide login method.

<br><img alt="Final SSO" src="https://cdn.bioturing.com/documentation/SSO_IMG/finalsso.png" class="lazy" width="100%"><br><br>

## SSO set up with Okta

:o: Login to Okta Account for **SAML / OPENID.**
:o: We are illustrating for SAML.
:o: Click on admin account push button and login to your Okta admin account.
  
```R
NOTE: Kindly follow the instructions and steps based on your infrastructure / IT department team. 
```

<br><img alt="loin-okta" src="https://cdn.bioturing.com/documentation/idiag/okta-account1.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: Click on **Create App Integration.**

<br><img alt="smal select" src="https://cdn.bioturing.com/documentation/idiag/oktastep2.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **SAML 2.0**

<br><img alt="Okta-app" src="https://cdn.bioturing.com/documentation/idiag/Okta-step3.png" class="lazy" width="100%"><br>

:large_orange_diamond: Write **App name**

<br><img alt="App name" src="https://cdn.bioturing.com/documentation/idiag/Oktastep4.png" class="lazy" width="100%"><br>

:large_orange_diamond: Upload application **logo** ( If you wish ).

<br><img alt="Okta logo" src="https://cdn.bioturing.com/documentation/idiag/Okta-step5.png" class="lazy" width="100%"><br>

:large_orange_diamond: On BioStudio dashboard login. Select SSO :arrow_right: Add New SSO.

<br><img alt="SSO login" src="https://cdn.bioturing.com/documentation/idiag/new_sso_login.png" class="lazy" width="100%"><br>

:large_orange_diamond: Copy **callback URL** from **New SSO login** and update on Okta.

<br><img alt="callback UR" src="https://cdn.bioturing.com/documentation/idiag/Oktaste7-fill-value.png" class="lazy" width="100%"><br>

:large_orange_diamond: Scroll down and click on **Next**

<br><img alt="SSO next" src="https://cdn.bioturing.com/documentation/idiag/okta-step8-next.png" class="lazy" width="100%"><br>

:large_orange_diamond: Follow **Step3: I'm an Okta customer adding an internal app.**

<br><img alt="Okta -step3" src="https://cdn.bioturing.com/documentation/idiag/okta-step9.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Finish.**


<br><img alt="Okta - Finish" src="https://cdn.bioturing.com/documentation/idiag/okta-step10-finish.png" class="lazy" width="100%"><br>

:large_orange_diamond: **SAML** config data is ready.

<br><img alt="loin-admin" src="https://cdn.bioturing.com/documentation/idiag/view-saml.png" class="lazy" width="100%"><br>

:large_orange_diamond: **View SAML setup instructions.**

<br><img alt="SAML Setup" src="https://cdn.bioturing.com/documentation/idiag/add-smal.png" class="lazy" width="100%"><br>


:large_orange_diamond: Get the value from Okta and fill on **SSO BioStudio**. Click on **Submit**.

<br><img alt="fill SSO" src="https://cdn.bioturing.com/documentation/idiag/Fill-sso.png" class="lazy" width="100%"><br>

:large_orange_diamond: **User assignment to Application.**

<br><img alt="Create user account" src="https://cdn.bioturing.com/documentation/idiag/okta-test-user-creation.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Assign User to Application.**

<br><img alt="loin-admin" src="https://cdn.bioturing.com/documentation/idiag/okta-user-assignment.png" class="lazy" width="100%"><br>

:large_orange_diamond: Login to **BioStudio.**

<br><img alt="loin-admin" src="https://cdn.bioturing.com/documentation/idiag/sso-login-test.png" class="lazy" width="100%"><br>


:large_orange_diamond: Login Succeed.

:large_orange_diamond: Before access **WORKSPACE**. It is necessary to access dashboard and create machine and well as create volume to be mounted.

:link: [Machine Creation and volume addition](https://colablocal.bioturing.com/document/installation#machine-creation)


<br><img alt="loin-admin" src="https://cdn.bioturing.com/documentation/idiag/SSO-successful-login.png" class="lazy" width="100%"><br>

:large_orange_diamond: Access BioStudio services.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/idiag/BioColab-img.png" class="lazy" width="100%"><br>

## SSO set up with PingID

:large_orange_diamond: **Add an application to PingID**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingida.png" class="lazy" width="100%"><br>


:large_orange_diamond: **Select SAML Application method and click on Configure**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid2.png" class="lazy" width="100%"><br>


:large_orange_diamond: **Login to BioColab Admin Dashboard**

```R
# https://<Domain name>/dashboard
```

It will prompt for Admin credentials. Please provide Admin credentials to login.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid3.png" class="lazy" width="100%"><br>


:large_orange_diamond:  Select SSO setting from left side menu and click on **+ Add New SSO**. If you are going to
set up SSO at the same time.

:bell: Note: If we are going to provide a Callback URL to another team to configure with IDP. Then we must provide dummy values to the mandatory field and click on submit button to save. Later we can update.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid4.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Copy Callback HTTPS URL that needs to be configured with IDP.**


<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid5.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **Manually Enter** and fill **callback URL** to **ACS URLs** and **Entity ID** would be the **last value** of that URL.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid6.png" class="lazy" width="100%"><br>

:large_orange_diamond: Fill the value based on over instruction.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid7.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Click on Save button.**

- Now update attribute mapping.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid8.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Select Configuration Tab and get all required values.**

:one: **Issuer ID**

:two: **Initiate Single Sign-On URL**

:three: **Download singing certificate**


<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingidc.png" class="lazy" width="100%"><br>

:large_orange_diamond: login to Biocolab dashboard admin and fill those values to required fields by **updating SSO settings.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid9.png" class="lazy" width="100%"><br>

:large_orange_diamond: I created two users but on the existing set up you might have a user's list already on the portal with a specified group to assign applications.

- On the Identity. I configured two users below.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid9-1.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Now I created one Group and assigned those user’s to that Group**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid10.png" class="lazy" width="100%"><br>

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingidg.png" class="lazy" width="100%"><br>

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid11.png" class="lazy" width="100%"><br>

:large_orange_diamond: **There are many ways to assign users to the group. Like User → Group → Edit – assign. Assign a group to the application.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid12.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Now all set and time to test SSO login with those users.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid13.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Provide PingID username and password, which we configured with Ping ID.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid15.png" class="lazy" width="100%"><br>

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid16.png" class="lazy" width="40%"><br>

:large_orange_diamond: **User is able to login successfully.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid17.png" class="lazy" width="40%"><br>

## SSO set up with Azure AD ( SAML )

```R
# Login to the dashboard admin
# https://<domain name>/dashboard
# provide admin credential, if already registered.
# If admin not yet registered, Kindly follow the instruction and registered first.
# NOTE: Make sure root password handy that you passed during BioStudio installation.
```

- Dashboard login.

- It will prompt for Admin credentials. Please provide Admin credentials to login.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid3.png" class="lazy" width="100%"><br>

:large_orange_diamond:  Select SSO setting from left side menu and click on **+ Add New SSO**. If you are going to
set up SSO at the same time.

:bell: Note: If we are going to provide a callback URL to another team to configure with IDP, Then we must provide dummy values to the mandatory field and click on the submit button to save. Later, we can update.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/pingid4.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Copy Callback HTTPS URL that needs to be configured with IDP.**

:bell: I am following to save the existing callback URL. Later, we will configure this.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az1a.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: **Login to Azure Cloud.**

:large_orange_diamond: **Open  Microsoft Entra ID ( Azure Active Directory )**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az2.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Click on Enterprise applications.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az3.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click **+ New application.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az4.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click **+ Create your own application.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az5.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Input your application name.** Click on **Create**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az6.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Application has been added.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az7.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Single sign-on.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az8.png" class="lazy" width="100%"><br>


:large_orange_diamond: Click on **SAML.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az9.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **Edit -- Basic SAML Configuration**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az10.png" class="lazy" width="100%"><br>

- Fill required field.
  
:one: Identifier (Entity ID) : **Callback URL**
:two: Reply URL (Assertion Consumer Service URL) : **Callback URL**

:large_orange_diamond: Login to BioStudio dashboard and click on three dot to select **Update SSO setting**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az11.png" class="lazy" width="100%"><br>

- Copy callback URL and fill on required fields.
  
<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az12.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: Click on **Save** button.

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az13.png" class="lazy" width="100%"><br>

- Download **Certificate (Base64)**
- Copy **Login URL**
- Copy **Microsoft Entra ID Identifier**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az14.png" class="lazy" width="100%"><br>

:pencil2: **Certificate (Base64)** = **IDP x509 Public Cert**
:pencil2: **Login URL** = **IDP SSO URL**
:pencil2: **Microsoft Entra ID Identifier** = **IDP Issuer URL**

- Fill appropriate values to BioStudio SSO configuration.

:large_orange_diamond: Login to BioStudio dashboard and click on three dot to select **Update SSO setting**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az11.png" class="lazy" width="100%"><br>

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az15.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Create user and assign application to the user**

:large_orange_diamond: Click on **Users and groups**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az16.png" class="lazy" width="100%"><br>

:large_orange_diamond: Click on **+ Add user/group**

:large_orange_diamond: Click on **Add user** and click on **Select**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az17.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Click on Assign**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az18.png" class="lazy" width="100%"><br>

:large_orange_diamond: **User has been Assign to this application.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az19.png" class="lazy" width="100%"><br>


:large_orange_diamond: **Login succeed.**

<br><img alt="BioColab-img" src="https://cdn.bioturing.com/documentation/SSO_IMG/az20.png" class="lazy" width="100%"><br>

## SSL setup.
<div class="warning" style='background-color: LightGray; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<code><b>SSL Setup :</b></code> Kindly get <b style="color: darkblue"> X.509 Provate and Public key</b>. 
</p>
</span>
</div>

```R

I] Upload SSL file using web-ui.
# Just need tu put right value on write box and update.
# Or upload files as required.
# System will auto detect those updates.

II] Login to server and follow below steps.
# Copy tls.crt and tls.key file to /biocolab/configs.
# It was auto detected by our software and update the certificates.
```

:large_orange_diamond: SSL using  WebUI

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/SSL-setup.png" class="lazy" width="100%"><br>

:large_orange_diamond: SSL direct upload on server location.

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/tls-cer.png" class="lazy" width="100%"><br>

## Kubernetes Setup for BioStudio

> Helm chart version : **1.0.70**

```R
# Before installing the BioTuring System on Linux/K8S, some pre-installation steps are required:
# System: K8s
# A token obtained from BioTuring for BioStudio.
# BioStudio supporting GPU and CPU type of instance / Machine. 
# Kindly select GPU, If you wish to use Prebuilt GPU based notebook or wish to generate GPU based note book.
```

## Prepare GPU toolkit for K8S

```R
Patch container engines (Docker, Containerd)
Install NVidia container toolkit on each node following the guide:
```

:link: [nvidia toolkit install guide](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)

:large_orange_diamond: Check container engines (Docker, Containerd)

```R
# For microk8s :
microk8s kubectl describe no | grep Runtime

# For vanilla :
kubectl describe no | grep Runtime
```  

:arrow_forward: If container engine is Containerd, add these lines to : **/etc/containerd/config.toml**

```R
privileged_without_host_devices = false
base_runtime_spec = ""
[plugins."io.containerd.grpc.v1.cri".containerd.runtimes.runc.options]
    SystemdCgroup = true
[plugins."io.containerd.grpc.v1.cri".containerd.runtimes.nvidia]
    privileged_without_host_devices = false
    runtime_engine = ""
    runtime_root = ""
    runtime_type = "io.containerd.runc.v1"
    [plugins."io.containerd.grpc.v1.cri".containerd.runtimes.nvidia.options]
    BinaryName = "/usr/bin/nvidia-container-runtime"
    SystemdCgroup = true
[plugins."io.containerd.grpc.v1.cri".cni]
bin_dir = "/opt/cni/bin"
conf_dir = "/etc/cni/net.d"
```

:arrow_forward: After that, restart containerd

```R
sudo systemctl restart containerd
sudo nvidia-container-cli --load-kmods info
```

If container engine is **Docker**, add these lines to: **/etc/docker/daemon.json**

```R
{
    "default-runtime": "nvidia",
    "runtimes": {
        "nvidia": {
            "path": "nvidia-container-runtime",
            "runtimeArgs": []
        }
    }
}
```

:arrow_forward: After that, restart docker

```R
sudo systemctl restart docker
sudo nvidia-container-cli --load-kmods info
```

## Install BioTuring ecosystem on K8S

---
We support all k8s engines: GKE (Google Kubernetes Engine), EKS (Amazon Elastic Kubernetes Service), AKS (Azure Kubernetes Service), MicroK8s, and vanilla K8S ...etc.

Ensure that **helm (version 3)** is installed.
   
:arrow_forward: First, check the Helm version.

```R
# Example :

microk8s enable helm3

microk8s helm3 version
```

**Helm command tips:**

```R
# Add repo charts
helm repo add bioturing https://bioturing.github.io/charts/apps/
helm repo update
helm search repo bioturing

# Login BioTuring registry
helm registry login -u admin registry.bioturing.com

# Show information of helm chart name
helm show all bioturing/<helm chart name> --version <helm chart version>

# Action into helm chart name
helm template bioturing bioturing/<helm chart name> --version <helm chart version>
helm install bioturing bioturing/<helm chart name> --version <helm chart version>
helm upgrade bioturing bioturing/<helm chart name> --version <helm chart version>
```

:o: Add BioTuring Helm charts
```R
# Example:

For Vanilla K8s:

helm repo add bioturing https://bioturing.github.io/charts/apps/

For Microk8s:

microk8s helm3 repo add bioturing https://bioturing.github.io/charts/apps/
```

## Helm Chart



| **Key**                                    | **Type** | **Default**        | **Description**      |
|--------------------------------------------|----------|--------------------|----------------------|
| image.biocolab.repository                  | string   | bioturing/biocolab | biocolab repository  |
| image.biocolab.tag                         | int      | 2.0.50             | biocolab image tag   |
| image.bioproxy.repository                  | string   | bioturing/biocolab | bioproxy repository  |
| image.bioproxy.tag                         | int      | 1.0.26             | bioproxy image tag   |
| imagePullSecrets                           | object   | {}                 | secrets              |
| secret.data.allowips                       | string   | ""                 | allow ip             |
| secret.data.cbtoken                        | string   | ""                 | Colab token          |
| secret.data.domain                         | string   | ""                 | domain name          |
| secret.admin.username                      | string   | admin              | admin user name      |
| secret.admin.password                      | string   | passwdadmin12         | admin password       |
| secret.postgresql.dbcolab                  | string   | ""                 | postgres DB name     |
| secret.postgresql.dbhub                    | string   | ""                 | postgres hub DB name |
| secret.postgresql.username                 | string   | ""                 | postgres user name   |
| secret.postgresql.password                 | string   | ""                 | postgres password    |
| secret.server.aria2c_list_ips              | object   | {}                 |                      |
| secret.server.certificate                  | string   | ""                 | Server certificate   |
| secret.server.key                          | string   | ""                 | Server Key           |
| secret.server.collaborative_mode           | bool     |  false             |                      |
| secret.server.debug_mode                   | bool     |  false             |                      |
| secret.server.enable_https                 | bool     |  false             |                      |
| secret.server.memcached_list               | string   | ""                 |                      |
| secret.server.mqtt_list_ips                | string   | ""                 |                      |
| secret.server.redis_list                   | string   | ""                 |                      |
| secret.server.redis_password               | string   | ""                 |                      |
| secret.server.tracing_mode                 | bool     |  false             |                      |
| secret.server.trakfik_proxy_mode           | bool     |  false             |                      |
| secret.server.use_letsencrypt              | bool     |  false             |                      |
| secret.server.use_redis_cache              | bool     |  false             |                      |
| service.ports.biocolab.aria2c.port         | int      | 6800               |                      |
| service.ports.biocolab.http.port           | int      | 11123              | application port     |
| service.ports.biocolab.jobqueue.port       | int      | 11300              |                      |
| service.ports.biocolab.mqtttcp.port        | int      | 1883               |                      |
| service.ports.biocolab.mqttweb.port        | int      | 9001               |                      |
| service.ports.biocolab.notebook.port       | int      | 18000              |                      |
| service.ports.bioproxy.http.port           | int      | 80                 | http port            |
| service.ports.bioproxy.https.port          | int      | 443                | https port           |
| service.ports.bioproxy.memcached.port      | int      | 11211              |                      |
| service.ports.bioproxy.ntfsp1.port         | int      | 111                |                      |
| service.ports.bioproxy.ntfsp2.port         | int      | 2049               |                      |
| service.ports.bioproxy.ntfsp3.port         | int      | 32767              |                      |
| service.ports.bioproxy.ntfsp4.port         | int      | 32765              |                      |
| service.ports.bioproxy.postgresql.port     | int      | 5432               |                      |
| service.ports.bioproxy.redis.port          | int      | 6379               | redis port           |
| persistence.dirs.app.size                  | String   | 100Gi                | application data     |
| persistence.dirs.app.storageClass          | string   | ""                 |                      |
| persistence.dirs.metadata.size             | String   | 5Gi                | metadata             |
| persistence.dirs.metadata.storageClass     | string   | ""                 |                      |
| persistence.dirs.user.size                 | String   | 500Gi                | user data            |
| persistence.dirs.user.storageClass         | string   | ""                 |                      |
| ingress.annotations                        | object   | {}                 |                      |
| ingress.className                          | string   | ""                 |                      |
| ingress.classNginxName                     | string   | nginx              |                      |
| ingress.enabled                            | bool     | true               |                      |
| ingress.tls                                | bool     | true               |                      |
| ingress.tls.enabled                        | bool     | true               |                      |
| ingress.useNginx                           | bool     |  false             |                      |
| nodeSelector                               | object   | {}                 |                      |
| podAnnotations                             | object   | {}                 |                      |
| podSecurityContext                         | object   | {}                 |                      |
| replicaCount                               | int      | 1                  |                      |
| resources                                  | object   | {}                 |                      |
| service.type                               | string   | ClusterIP          |                      |
| serviceAccount.annotations                 | object   | {}                 |                      |
| serviceAccount.name                        | string   | ""                 |                      |
| tolerations                                | object   | {}                 |                      |
| host_ip                                    | int      | 0.0.0.0            |                      |
| affinity                                   | object   | {}                 |                      |
| autoscaling                                | object   | {}                 |                      |
| autoscaling.enabled                        | bool     |  false             |                      |
| autoscaling.maxReplicas                    | int      |                    | 100                  |
| autoscaling.minReplicas                    | int      |                    | 2                    |
| autoscaling.targetCPUUtilizationPercentage | int      |                    | 80                   |
| gpu.runtimeClassName                       | string   | ""           |                      |

<br>

:large_orange_diamond: Select **helm chart version.**

:o:Kindly select **latest version** of **Helm Chart**. Support team will get in touch with you and share latest version tag.

```R
# Click on install.
```

<br><img alt="BioColab version" src="https://cdn.bioturing.com/documentation/idiag/Biocolab-version.png" class="lazy" width="100%"><br>

:large_orange_diamond: Select **namespace** and type name of **Statefulset**.

:large_orange_diamond: Click on **Next**

<br><img alt="Type name" src="https://cdn.bioturing.com/documentation/idiag/biocolab-step1-namespace.png" class="lazy" width="100%"><br>

:large_orange_diamond: Verify ***Tag*** and ***repository***

<br><img alt="tag verification" src="https://cdn.bioturing.com/documentation/idiag/verify-image-tag.png" class="lazy" width="100%"><br>

:large_orange_diamond: **Update values:**
  
```R
# Change volume size according to your data.
# Update domain name and Colab token.
# Update credentials based on your choice.
# Click on install.
```

<br><img alt="PVC and domain" src="https://cdn.bioturing.com/documentation/idiag/pvc-domain.png" class="lazy" width="100%"><br><br>

:large_orange_diamond: BioStudio will start installation based on helm chart.

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/helm-installed.png" class="lazy" width="100%"><br>

:large_orange_diamond: Verify **statefulset.**

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/stateful-set.png" class="lazy" width="100%"><br>

:large_orange_diamond: Verify **ingress.**

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/ingress.png" class="lazy" width="100%"><br>


:large_orange_diamond: Browse **your domain**.

<br><img alt="ssl-setup" src="https://cdn.bioturing.com/documentation/idiag/biocolab-web.png" class="lazy" width="100%"><br>

:small_orange_diamond: Before access **WORKSPACE**. It is necessary to access dashboard and create machine and well as create volume to be mounted.

```R
# Note: Kindly follow to create Machine and volume creation process in order to utilize our product.
# It is a necessary step.
# For any support and enquiry. Drop a mail to us support@bioturing.com
```

![BioStudio logo](https://cdn.bioturing.com/documentation/EKS_PIC/logo.png)

# <p style="color: #006400">  BioStudio Deployments on Kubernetes</p>

# <p style="color: #000080"> Introduction </p>

<div class="warning" style='background-color:#E9D8FD; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
<span>
<p style='margin-top:1em; text-align:justify'; text-justify:inter-word;>
<code><b>BioStudio on K8s</b></code> BioStudio software is compatible and easy to install on all kind of <b style="color: darkblue">Operating System </b> as well as on <b style="color: darkblue"> Docker, Kubernetes, Standalone machine, Cloud, On-premises, VM and all type of infrastructure platform</b>.</b> We are happy to inform that we are a leading brands company to provide all of our <b style="color: blue"><u>Softwares as a Service (SaaS)</b></u>. It is directly ready to use for end users.
</p>
</span>
</div>

:bell: **Please contact** :e-mail: [**support@bioturing.com**] **in case you need any support or have any inquiry for us.** 

> **We are supporting all kind of service provider including on-premise.**

```R
BioStudio on K8s. Install Software on Kubernetes Clusters with the Helm.
```

## AWS EKS Cluster

:passport_control: **Login to AWS console.** 

:o: **Serach for EKS in serach bar.** 

<img alt="Search" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-search.png" class="lazy" width="100%"> 

<b></b>

:o: **select create on Add Cluster.** 

<b></b>

<img alt="create" src="https://cdn.bioturing.com/documentation/EKS_PIC/select-add-cluster-create.png" class="lazy" width="100%"> 

<b></b>

:o: **Configure Cluster.** 
<b></b>

<img alt="Configure" src="https://cdn.bioturing.com/documentation/EKS_PIC/select-cluster-nameandKube-version.png" class="lazy" width="100%"> 

<b></b>

:o: **Create Cluster Service role.**

```R
role --> Create role
``` 
<b></b>

<img alt="Create role" src="https://cdn.bioturing.com/documentation/EKS_PIC/role-create-role.png" class="lazy" width="100%"> 

<b></b>

:o: **Select AWS service and EKS on use case.** 

<b></b>

<img alt="eks" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-service-eks.png" class="lazy" width="100%"> 

<b></b>

:o: **Select EKS -Cluster.** 

<b></b>
<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-ekscluster-next.png" class="lazy" width="100%"> 
<b></b>
 
:o: **Add permission.** 

```R
AmzonEKSClusterPolicy
``` 
:arrow_right: **click on next.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/autao-add-permission.png" class="lazy" width="100%">

<b></b>

:o: **Fill Role detail.** 

:arrow_right: **Create role.** 

<b></b>
<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eksrole-detail.png" class="lazy" width="100%"> 
<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/add-tag-crearte-role.png" class="lazy" width="100%"> 
<b></b>

:o: **Role created .** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/role-creation-done.png" class="lazy" width="100%"> 

<b></b>


:o: **Select appropriate role that we created earlier..** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/role-view-oneks.png" class="lazy" width="100%"> 

<b></b>

:o: **provide appropriate tag.** 

:arrow_right: **click on next.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-cluster-tag.png" class="lazy" width="100%"> 

<b></b>

:o: **Specify networking. VPC and Networking.** 

:link: [Amazon EKS VPC and subnet requirements and considerations](https://docs.aws.amazon.com/eks/latest/userguide/network_reqs.html)

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-vpc-subnet-default.png" class="lazy" width="100%"> 

<b></b>

:o: **Select Security Group.** 

:arrow_right: **click on next.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/Cluster-endpoint-next.png" class="lazy" width="100%"> 

<b></b>

:o: **Select Configuring logging.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/configure-login.png" class="lazy" width="100%"> 

<b></b>

:o: **Select Add-ons.** 

:arrow_right: **click on next.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/select-addons.png" class="lazy" width="100%"> 

:arrow_right: **Select Version of Add-ons and click on next.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/configure-addons-serting.png" class="lazy" width="100%"> 
<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/configure-addons-next.png" class="lazy" width="100%"> 
<b></b>

:o: **Click on Create.** 

<img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/scrill-down-create.png" class="lazy" width="100%"> 
<b></b>


:blush: **You are done to create cluster. Wait for a while to setup this.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/cluster-creation-under-progress.png" class="lazy" width="100%"><br>

:gift: **Kubernetes Cluster is Active now.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-cluster-ready.png" class="lazy" width="100%"><br>

:link: [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

```R
Kindly select the OS version installation according to your Operating System.
``` 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-intallation-on-window.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-accept-licence.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-setup-location.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-install-final-step.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-installation-in-progress.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-install-completed-finish.png" class="lazy" width="100%"><br>

:o: Test AWS cli

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-version-test.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-cli-clusater-check.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aws-eks-cluster-status.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/kubectl-version.png" class="lazy" width="100%"><br> 

:o: **Installing Kubectl command utility.** 

:link: [Chocolatey](https://chocolatey.org/install#individual)

```R
There are many ways to install Kubectl command utility too. Here we are using window machine, So just to prefer Choco.
``` 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/choco-install.png" class="lazy" width="100%"><br> 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/kubectl-command-install.png" class="lazy" width="100%"><br> 

<b></b>

:o: **Adding worker node to Kubernete cluster.** 

```R
EKS --> Compute --> Add node group.
In order to add node to the cluster. We need to add node group. Each node group can content different kind of node ( compute resources ). We can add many node group based on requirements.
``` 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/compute-add-node.png" class="lazy" width="100%"><br>

:o: **Configure node group.** 

```R
In node group configuration, We need to provide node name as well as must create Node IAM role. to handle worker node. Once click on IAM console. A new window will open to create new IAM role.
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-gr-config.png" class="lazy" width="100%"><br> 

:o: **Click on Create role.** 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/createrolefor-node.png" class="lazy" width="100%"><br> 

:o: **Select AWS service.** 

```R
Use cases for other AWS services. EC2
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-role-policy.png" class="lazy" width="100%"><br>

```R
Add three tick mark policy that role.
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-policy-for-node.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/eks-node-policy-ec2.png" class="lazy" width="100%"><br>

:o: **Click on Create role.** 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-role-created.png" class="lazy" width="100%"><br> 

```R
Once role is ready. Now time to assign this role to node group.
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/attach-iamroleTo-nodeconfig.png" class="lazy" width="100%"><br> 


```R
You have two option to create Ec2 instance.
1. Launch from EKS node configuration wizard.
2. Using Template
```

:one: **Launch from EKS node configuration wizard.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-gr-conf.png" class="lazy" width="100%"><br>

:o: **Click on Next.** 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/create-node-next.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/secondway-node-creation.png" class="lazy" width="100%"><br> 

:o: **Click on Next.** 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-group-scale.png" class="lazy" width="100%"><br> 

:o: **Click on Next.** 
<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/add-node-gr-networl.png" class="lazy" width="100%"><br> 

:o: **Click on Create.** 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/create-node-gr-final.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-under-creation.png" class="lazy" width="100%"><br> 

:arrows_counterclockwise: **Wait for a while to add node to the Cluster.**

:two: **Add node group using template wizard.**

:o: **Click on Create Launch template.**

:arrow_forward: Follow the instruction based on Template creation steps.

:link: [Create Template](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/create-launch-template.html)


<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/create-template.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/node-creation.png" class="lazy" width="100%"><br> 
 
<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/launch-template.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/keypair.png" class="lazy" width="100%"><br> 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/create-template-01.png" class="lazy" width="100%"><br> 

:o: **Once followed to provide all the value. Click on create launch template.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/Template-created.png" class="lazy" width="100%"><br> 

:o: **Once template ready. Add to the node group.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/add-launch-template.png" class="lazy" width="100%"><br> 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/resources-addedto-cluster.png" class="lazy" width="100%"><br> 

:o: **In order to use PVC creation. We must have driver installed with cluster.**

:o: **Click on Add-ons tab.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/addon-click.png" class="lazy" width="100%"><br>

:o: **Click on Get more Add-ons.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/ebs-driver-creation.png" class="lazy" width="100%"><br> 

:o: **Select Amazon EBS CSI Driver.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/selectaddo.png" class="lazy" width="100%"><br>

:o: **Click on next.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/addnxt.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/consel.png" class="lazy" width="100%"><br> 

:o: **Click on Create.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/ebs-csi-driver-addon-cluster.png" class="lazy" width="100%"><br> 

:eight_pointed_black_star: **We need to create IAM OIDC provider for your cluster.**

:link: [OIDC](https://docs.aws.amazon.com/eks/latest/userguide/enable-iam-roles-for-service-accounts.html)

:o: **Copy the OpenID Connect provider URL.**

:arrow_right: **Search IAM and click on role**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/iam.png" class="lazy" width="100%"><br> 

:arrow_right: **Select Identity provider on Access management.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/id.png" class="lazy" width="100%"><br> 

:arrow_right: **Click on Add provider.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/id.png" class="lazy" width="100%"><br> 


:arrow_right: **Click on OpenID Connect.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/opidc.png" class="lazy" width="100%"><br> 

:arrow_right: **Paste Provider URL tht we copied earlier from Cluster.**

:arrow_right: **Click on Get thumbprint.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/gt.png" class="lazy" width="100%"><br> 

:arrow_right: **Audience, enter sts.amazonaws.com and choose Add provider.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/aud.png" class="lazy" width="100%"><br> 

:o: **Create Amazon EBS CSI driver IAM role.**

:link: [CSI driver IAM role](https://docs.aws.amazon.com/eks/latest/userguide/csi-iam-role.html)

```R
IAM --> Roles --> Create role
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/crw.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/create-openid-role.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/openid-next.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/openid-driver-permission-asignment.png" class="lazy" width="100%"><br> 

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/OpenID-Create_role-1.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/OpenID-Create_role_Completed.png" class="lazy" width="100%"><br> 

:arrow_right: **Edit trust relationship policy.**

:arrow_right: **Click on Edit trust policy. Add the following line after comma**

:bell: **Change the value based on your OpenID**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/num.png" class="lazy" width="100%"><br> 

```R
"oidc.eks.ca-central-1.amazonaws.com/id/7B6A410BCEF7466327A6CE441E164591:sub": "system:serviceaccount:kube-system:ebs-csi-controller-sa" 
```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/etp.png" class="lazy" width="100%"><br> 

:arrow_right: **Click on Update policy.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/up.png" class="lazy" width="100%"><br> 

:bell: **Make sure user should have permissions "AmazonEC2FullAccess".**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/mk.png" class="lazy" width="100%"><br> 

:o: **Update EBS CSI Driver fro IAM Role.**

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/upcs.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/editad.png" class="lazy" width="100%"><br>

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/ebs-driver-updateforrole.png" class="lazy" width="100%"><br> 

:arrow_right: **Test.**
```R
aws eks --region ca-central-1  describe-cluster --name BioColab-EKS  --query cluster.status --profile lalitshaktawat

aws eks update-kubeconfig --region ca-central-1 --name BioColab-EKS --profile lalitshaktawat

eksctl utils associate-iam-oidc-provider --region=ca-central-1 --cluster=BioColab-EKS --approve --region ca-central-1 --profile lalitshaktawat

kubectl config current-context  

```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/pvt.png" class="lazy" width="100%"><br> 

:arrow_right: **Troubleshoot.** 

```R
We might face an issue related to PVC. Pod will not start and it will be on pending status. We just need to recreate ebs-csi-controller to resolve this issue.


kubectl delete pods -n kube-system -l=app=ebs-csi-controller

```

<br><img alt="eks-pic" src="https://cdn.bioturing.com/documentation/EKS_PIC/rs.png" class="lazy" width="100%"><br> 

```R
========
pvc.yaml
========
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: ebs-claim1
spec:
  accessModes:
    - ReadWriteOnce
  storageClassName: gp2
  resources:
    requests:
      storage: 1Gi

========
pod.yaml
========
apiVersion: v1
kind: Pod
metadata:
  name: app
spec:
  containers:
  - name: app
    image: centos
    command: ["/bin/sh"]
    args: ["-c", "while true; do echo $(date -u) >> /data/out.txt; sleep 5; done"]
    volumeMounts:
    - name: persistent-storage
      mountPath: /data
  volumes:
  - name: persistent-storage
    persistentVolumeClaim:
      claimName: ebs-claim1
```

```R
Create resources for testing. It is just a test. You can skip this step.
======================================================================== 
kubectl apply -f .\pvc.yaml
kubectl apply -f .\pod.yaml
kubectl get pods
kubectl get pvc

Delete resources.
=================
kubectl delete po/<pod name> -n <namespace name>
```

:link: [kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
   
:o: **Installing Helm.**

:arrow_right: **Please follow link below to install Helm.** 

:link: [Helm Installation](https://archive.eksworkshop.com/beginner/060_helm/helm_intro/install/)

```R
helm repo add bioturing https://bioturing.github.io/charts/apps/
helm repo update
helm search repo bioturing
```

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/EKS_PIC/hel.png" class="lazy" width="100%"><br> 

:bell: **I downloaded latest version of BioStudio and adjusted values accordingly.** 

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/EKS_PIC/done-wihout-lb.png" class="lazy" width="100%"><br>

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/EKS_PIC/pvc-done.png" class="lazy" width="100%"><br> 

:o: **Kindly setup Load balancer (ALB) with your DNS.**

:o: **Please contact** :e-mail: [**support@bioturing.com**] for any inquiry.

# <p style="color: green"> Machine name on K8S </p>

```R
# We must use local DNS service name to add machine.

<Service Name>.<Namespace>.svc.cluster.local

# bioc-test-release-biocolab-colab.bioc-test.svc.cluster.local

# biocolab-preprod-biocolab-colab.bioturing-preprod.svc.cluster.local
```

# BioStudio Checklist

:bell: **Note**:  Ensure that the BioProxy container **doesn't** have HTTP_PROXY, HTTPS_PROXY, and NO_PROXY settings configured

```R
1] Process running with host.
ps -ef
netstat -nltup

2] Process running with Bioproxy container	
ps -ef
netstat -nltup
				
3] Process running with BioColab container
ps -ef
netstat -nltup		
				
4] Check application up and running and connectivity.
				
curl command testing				
				
	curl <localhost>			
	curl <localhost>:<http port>			
	curl <localhost>:<application port>			
	curl <localhost>:<nginx port>			
				
5] check whiltelist of domain with Host and both containers.		
				
- curl https://colab.biotruing.com
-- Should show contents

- curl https://cdn.biotruing.com
-- wget https://cdn.bioturing.com/documentation/adm.png

- curl https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com
-- wget https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com/colab/apps/0w-byh0iNCWigGEjbZybU.92ae1dec-6bf9-4041-9d06-330e0fe7b564.zip

- curl https://s3.us-west-2.amazonaws.com/cdn.bioturing.com
-- wget https://s3.us-west-2.amazonaws.com/cdn.bioturing.com/documentation/adm.png

- curl https://studio.bioturing.com
-- Should show contents				
				
		
				
6] Check application varification processes
with Host machine

# ps -ef | grep 'docker'
# ps -ef | grep 'miniconda'
# ps -ef | grep nginx
# ps -ef | grep postgres			
				
7] Check dashboard setting

8] Check websocket

9] Check to download notebook and running

10] Guide for SSO login

```

# Test and verification

Before start installation below is the status:

```R
root@ip-172-31-39-182:/biocolab/installation-2.0.53# netstat -nltup
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 127.0.0.53:53           0.0.0.0:*               LISTEN      2892/systemd-resolv
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN      2820/sshd: /usr/sbi
tcp6       0      0 :::22                   :::*                    LISTEN      2820/sshd: /usr/sbi
udp        0      0 127.0.0.53:53           0.0.0.0:*                           2892/systemd-resolv
udp        0      0 172.31.39.182:68        0.0.0.0:*                           2882/systemd-networ
udp        0      0 127.0.0.1:323           0.0.0.0:*                           2808/chronyd
udp6       0      0 ::1:323                 :::*                                2808/chronyd

root@ip-172-31-39-182:/biocolab/installation-2.0.53# env
SHELL=/bin/bash
PWD=/biocolab/installation-2.0.53
LOGNAME=root
HOME=/root
LANG=C.UTF-8
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
LESSCLOSE=/usr/bin/lesspipe %s %s
TERM=xterm-256color
LESSOPEN=| /usr/bin/lesspipe %s
USER=root
SHLVL=1
XDG_DATA_DIRS=/usr/local/share:/usr/share:/var/lib/snapd/desktop
PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
MAIL=/var/mail/root
_=/usr/bin/env
OLDPWD=/biocolab
```



## Testing with normal structure

**After installation**

:o: HTTP port : **80** and HTTPS port : **443**
**Application port** : **11123**

### netstat command testing

Below are the port should be in as status.

:one: Check `netstat -nltup` with Host and inside the container.

`netstat -nltup # from host`

```R
root@ip-172-31-39-182:/biocolab/installation-2.0.53# netstat -nltup
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 127.0.0.53:53           0.0.0.0:*               LISTEN      2892/systemd-resolv
tcp        0      0 0.0.0.0:1883            0.0.0.0:*               LISTEN      10842/docker-proxy
tcp        0      0 0.0.0.0:18000           0.0.0.0:*               LISTEN      10736/docker-proxy
tcp        0      0 0.0.0.0:443             0.0.0.0:*               LISTEN      10059/docker-proxy
tcp        0      0 0.0.0.0:80              0.0.0.0:*               LISTEN      10081/docker-proxy
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN      2820/sshd: /usr/sbi
tcp        0      0 0.0.0.0:5432            0.0.0.0:*               LISTEN      10009/docker-proxy
tcp        0      0 0.0.0.0:6800            0.0.0.0:*               LISTEN      10821/docker-proxy
tcp        0      0 0.0.0.0:6379            0.0.0.0:*               LISTEN      9982/docker-proxy
tcp        0      0 0.0.0.0:9091            0.0.0.0:*               LISTEN      9958/docker-proxy
tcp        0      0 0.0.0.0:9001            0.0.0.0:*               LISTEN      10802/docker-proxy
tcp        0      0 0.0.0.0:11300           0.0.0.0:*               LISTEN      10757/docker-proxy
tcp        0      0 0.0.0.0:11211           0.0.0.0:*               LISTEN      9937/docker-proxy
tcp        0      0 0.0.0.0:11123           0.0.0.0:*               LISTEN      10778/docker-proxy
tcp        0      0 0.0.0.0:32767           0.0.0.0:*               LISTEN      9893/docker-proxy
tcp        0      0 0.0.0.0:32765           0.0.0.0:*               LISTEN      9915/docker-proxy
tcp6       0      0 :::1883                 :::*                    LISTEN      10849/docker-proxy
tcp6       0      0 :::18000                :::*                    LISTEN      10744/docker-proxy
tcp6       0      0 :::443                  :::*                    LISTEN      10066/docker-proxy
tcp6       0      0 :::80                   :::*                    LISTEN      10088/docker-proxy
tcp6       0      0 :::22                   :::*                    LISTEN      2820/sshd: /usr/sbi
tcp6       0      0 :::5432                 :::*                    LISTEN      10030/docker-proxy
tcp6       0      0 :::6800                 :::*                    LISTEN      10829/docker-proxy
tcp6       0      0 :::6379                 :::*                    LISTEN      9988/docker-proxy
tcp6       0      0 :::9091                 :::*                    LISTEN      9965/docker-proxy
tcp6       0      0 :::9001                 :::*                    LISTEN      10809/docker-proxy
tcp6       0      0 :::11300                :::*                    LISTEN      10764/docker-proxy
tcp6       0      0 :::11211                :::*                    LISTEN      9943/docker-proxy
tcp6       0      0 :::11123                :::*                    LISTEN      10786/docker-proxy
tcp6       0      0 :::32767                :::*                    LISTEN      9900/docker-proxy
tcp6       0      0 :::32765                :::*                    LISTEN      9921/docker-proxy
udp        0      0 127.0.0.53:53           0.0.0.0:*                           2892/systemd-resolv
udp        0      0 172.31.39.182:68        0.0.0.0:*                           2882/systemd-networ
udp        0      0 127.0.0.1:323           0.0.0.0:*                           2808/chronyd
udp6       0      0 ::1:323                 :::*                                2808/chronyd
```

`netstat -nltup # inside the container`

```R
root@ip-172-31-39-182:/biocolab/installation-2.0.53# docker exec -it bioproxy /bin/bash
root@6c1fca69acf1:/home# netstat -nltup
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 0.0.0.0:11211           0.0.0.0:*               LISTEN      -
tcp        0      0 127.0.0.1:8886          0.0.0.0:*               LISTEN      183/node
tcp        0      0 127.0.0.1:9005          0.0.0.0:*               LISTEN      167/python3
tcp        0      0 0.0.0.0:5432            0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:6379            0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:8077            0.0.0.0:*               LISTEN      182/nginx: master p
tcp        0      0 127.0.0.1:5555          0.0.0.0:*               LISTEN      298/dataplaneapi
tcp        0      0 0.0.0.0:80              0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:443             0.0.0.0:*               LISTEN      -
tcp6       0      0 :::11211                :::*                    LISTEN      -
tcp6       0      0 :::5432                 :::*                    LISTEN      -
tcp6       0      0 :::8077                 :::*                    LISTEN      182/nginx: master p
udp        0      0 0.0.0.0:58951           0.0.0.0:*                           -
udp        0      0 0.0.0.0:36226           0.0.0.0:*                           -
root@6c1fca69acf1:/home#

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53# docker exec -it bioproxy /bin/bash
root@6c1fca69acf1:/home# netstat -nltup
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 0.0.0.0:11211           0.0.0.0:*               LISTEN      -
tcp        0      0 127.0.0.1:8886          0.0.0.0:*               LISTEN      183/node
tcp        0      0 127.0.0.1:9005          0.0.0.0:*               LISTEN      167/python3
tcp        0      0 0.0.0.0:5432            0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:6379            0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:8077            0.0.0.0:*               LISTEN      182/nginx: master p
tcp        0      0 127.0.0.1:5555          0.0.0.0:*               LISTEN      298/dataplaneapi
tcp        0      0 0.0.0.0:80              0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:443             0.0.0.0:*               LISTEN      -
tcp6       0      0 :::11211                :::*                    LISTEN      -
tcp6       0      0 :::5432                 :::*                    LISTEN      -
tcp6       0      0 :::8077                 :::*                    LISTEN      182/nginx: master p
udp        0      0 0.0.0.0:58951           0.0.0.0:*                           -
udp        0      0 0.0.0.0:36226           0.0.0.0:*                           -
root@6c1fca69acf1:/home#

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53# docker exec -it biocolab /bin/bash
root@5fc5db8bc5cf:/home# netstat -nltup
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 0.0.0.0:9001            0.0.0.0:*               LISTEN      -
tcp        0      0 127.0.0.1:18001         0.0.0.0:*               LISTEN      513/node
tcp        0      0 0.0.0.0:11123           0.0.0.0:*               LISTEN      148/t2d_dsc_tool
tcp        0      0 0.0.0.0:11300           0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:18081           0.0.0.0:*               LISTEN      360/python3.10
tcp        0      0 0.0.0.0:18000           0.0.0.0:*               LISTEN      513/node
tcp        0      0 0.0.0.0:1883            0.0.0.0:*               LISTEN      -
tcp        0      0 0.0.0.0:2223            0.0.0.0:*               LISTEN      149/sshd: /usr/sbin
tcp        0      0 127.0.0.1:11113         0.0.0.0:*               LISTEN      147/t2d_blc_tool
tcp        0      0 0.0.0.0:6800            0.0.0.0:*               LISTEN      144/aria2c
tcp6       0      0 :::9001                 :::*                    LISTEN      -
tcp6       0      0 :::1883                 :::*                    LISTEN      -
tcp6       0      0 :::2222                 :::*                    LISTEN      148/t2d_dsc_tool
tcp6       0      0 :::2223                 :::*                    LISTEN      149/sshd: /usr/sbin
root@5fc5db8bc5cf:/home#
```

### Environmental variables

**Bioproxy : environmental variable**

```R

# docker exec -it bioproxy /bin/bash

root@507cd2637a97:/home# env
NFS_T2_PORT=2049
SHELL=/bin/bash
POSTGRESQL_CLIENT_MIN_MESSAGES=error
DEBUG_MODE=false
HTTPS_SERVER_PORT=443
POSTGRESQL_USERNAME=XXXXXXXXXXXXXX
REDIS_PASSWORD=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
PKG_CONFIG_PATH=/usr/lib64/pkgconfig:/usr/lib/pkgconfig:/usr/local/lib64/pkgconfig:/usr/local/lib/pkgconfig
POSTGRESQL_DATA_DIR=/bitnami/postgresql/data
HOSTNAME=507cd2637a97
LANGUAGE=en_US:en
POSTGRESQL_ENABLE_LDAP=no
MAX_THREADS=32
USE_LETSENCRYPT=false
POSTGRESQL_LOG_HOSTNAME=false
NFS_T1_PORT=111
PWD=/home
OS_FLAVOUR=debian-11
GIT_SSL_NO_VERIFY=true
NFS_VOLUME_DIR=
PYTHONHTTPSVERIFY=0
NSS_WRAPPER_LIB=/opt/bitnami/common/lib/libnss_wrapper.so
ENABLE_HTTPS=false
TZ=UTC
POSTGRESQL_DATABASE=biocohub
NFS_T4_PORT=32767
APP_DOMAIN=<Client BioStudio Domain>
HOME=/
LANG=en_US.UTF-8
POSTGRESQL_VOLUME_DIR=/bitnami/postgresql
POSTGRESQL_POSTGRES_PASSWORD=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
CONFIG_DIR=/home/configs
POSTGRESQL_PORT_NUMBER=5432
POSTGRESQL_SHARED_PRELOAD_LIBRARIES=pgaudit
PG_DIR=
POSTGRESQL_LOG_DISCONNECTIONS=false
PG_PASSWORD=
MAX_CONNECTION=5000
BITNAMI_DEBUG=false
POSTGRESQL_LOG_CONNECTIONS=false
MAKEFLAGS=-j16
NFS_T3_PORT=32765
TERM=xterm
PG_USERNAME=
SSL_NO_VERIFY=1
MEMCACHED_PORT=11211
NO_PROXY=localhost,127.0.0.1
COLAB_LIST_SERVER=172.31.39.123:11123
DISPLAY=:1
SHLVL=1
POSTGRESQL_ENABLE_TLS=no
BITNAMI_APP_NAME=postgresql
POSTGRESQL_PASSWORD=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
REDIS_PORT=6379
LD_LIBRARY_PATH=/usr/lib64:/usr/lib:/usr/local/lib64:/usr/local/lib
APP_VERSION=15.2.0
COLAB_REDIS_DIR=/bitnami/postgresql/redis
PGDATA=/bitnami/postgresql/data
HTTP_SERVER_PORT=80
LC_ALL=C.UTF-8
OS_NAME=linux
PATH=/opt/bitnami/common/bin:/opt/bitnami/postgresql/bin:/opt/bitnami/postgresql/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/root/.local/bin
POSTGRESQL_PGAUDIT_LOG_CATALOG=off
DEBIAN_FRONTEND=noninteractive
OS_ARCH=amd64
_=/usr/bin/env
root@507cd2637a97:/home#

root@507cd2637a97:/home# cat /etc/environment 
root@507cd2637a97:/home#
root@507cd2637a97:/home# exit

```

**BioColab : environmental variable**

```R
# docker exec -it biocolab /bin/bash

SHELL=/bin/bash
NV_LIBCUBLAS_VERSION=11.11.3.6-1
NVIDIA_VISIBLE_DEVICES=all
DEBUG_MODE=false
CACHE_MODE=false
PYTHONUNBUFFERED=1
CYPRESS_CONFIG=false
RETICULATE_PYTHON=/miniconda/user/bin/python
no_proxy=localhost,fc00::/7,.svc,kubernetes,127.0.0.1,10.0.0.0/8,10.42.0.90,.local,fe80::/10,192.168.10.0/24,.cluster.local,::1/128,.default,0.0.0.0
REDIS_PASSWORD=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
R_GZIPCMD=/usr/bin/gzip
CONDA_EXE=/miniconda/user/bin/conda
XORG_DPI=96
COLLABORATIVE_MODE=false
PKG_CONFIG_PATH=/usr/lib64/pkgconfig:/usr/lib/pkgconfig:/usr/local/lib64/pkgconfig:/usr/local/lib/pkgconfig
ADMIN_USERNAME=admin
GECKODRIVER_VERSION=0.33.0
HOSTNAME=b1a226ccc20a
LANGUAGE=C.UTF-8
TMP_PATH=
NODE_OPTIONS=--max-old-space-size=16000
PYTORCH_ENABLE_MPS_FALLBACK=1
JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
NVIDIA_REQUIRE_CUDA=cuda>=11.8 brand=tesla,driver>=450,driver<451 brand=tesla,driver>=470,driver<471 brand=unknown,driver>=470,driver<471 brand=nvidia,driver>=470,driver<471 brand=nvidiartx,driver>=470,driver<471 brand=geforce,driver>=470,driver<471 brand=geforcertx,driver>=470,driver<471 brand=quadro,driver>=470,driver<471 brand=quadrortx,driver>=470,driver<471 brand=titan,driver>=470,driver<471 brand=titanrtx,driver>=470,driver<471 brand=tesla,driver>=510,driver<511 brand=unknown,driver>=510,driver<511 brand=nvidia,driver>=510,driver<511 brand=nvidiartx,driver>=510,driver<511 brand=geforce,driver>=510,driver<511 brand=geforcertx,driver>=510,driver<511 brand=quadro,driver>=510,driver<511 brand=quadrortx,driver>=510,driver<511 brand=titan,driver>=510,driver<511 brand=titanrtx,driver>=510,driver<511 brand=tesla,driver>=515,driver<516 brand=unknown,driver>=515,driver<516 brand=nvidia,driver>=515,driver<516 brand=nvidiartx,driver>=515,driver<516 brand=geforce,driver>=515,driver<516 brand=geforcertx,driver>=515,driver<516 brand=quadro,driver>=515,driver<516 brand=quadrortx,driver>=515,driver<516 brand=titan,driver>=515,driver<516 brand=titanrtx,driver>=515,driver<516
SEVER_INFO_COLAB_TOKEN_KEY=
MAMBA_SSL_NO_REVOKE=1
ADMIN_EXT_ID=
NV_NVTX_VERSION=11.8.86-1
TRACING_MODE=false
DEV_MODE=false
CORE_APP_VERSION=92ae1dec-6bf9-4041-9d06-330e0fe7b564
PYDEVD_DISABLE_FILE_VALIDATION=1
HUB_API_KEY=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
NV_LIBCUSPARSE_VERSION=11.7.5.86-1
JAVA_OPTS=-Djava.awt.headless=false
PG_HUB_DATABASE=biocohub
NV_LIBNPP_VERSION=11.8.0.86-1
HUB_SERVER_PORT=18000
JULIA_PKGDIR=/miniconda/user/share/julia
LAB_SHARED_PATH=/usr/local/share/jupyter/lab
PACK_R=BiocManager devtools extrafont geometry ggplot2 httr magic multcomp plotly plotrix rmarkdown rstudioapi xslx ggbio glmpca gganimate ggalt ggdendro ggpubr igraph odbc
NCCL_VERSION=2.15.5-1
NEW_INSTALL_MODE=true
STATIC_PATH=/appdata/share/static
PWD=/home
USE_REDIS_CACHE=true
CODE_VERSION=4.16.1
MAX_UPLOAD_FILE_SIZE=21474836480
PORT=11123
NVIDIA_DRIVER_CAPABILITIES=compute,utility
GIT_SSL_NO_VERIFY=true
NV_LIBNPP_PACKAGE=libnpp-11-8=11.8.0.86-1
PYTHONHTTPSVERIFY=0
TZ=Etc/UTC
OPENAI_KEY=sk-XXXXXXXXXXXXXXXXXXXXXXXXXXXX
OPENBLAS_NUM_THREADS=8
STATIC_PACK_MODE=true
UPGRADE_RESOURCE_URL=https://colab.bioturing.com
NVIDIA_PRODUCT_NAME=CUDA
USER_PATH=
API_KEY=2015f6c1b7ef431267460c249deda53c
APP_DATA=/appdata
LD_PRELOAD=/miniconda/user/lib/mambasos.so
NV_CUDA_CUDART_VERSION=11.8.89-1
RPC_SECRET=bioturing500
SSHDP_SERVER_PORT=2222
HOME=/root
COLAB_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXX
LANG=C.UTF-8
FENET_KEY=
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
CARGO_HOME=/miniconda/user
NXF_CONDA_ENABLED=true
AMZ_S3_KEY=
RPC_PORT=6800
CUDA_VERSION=11.8.0
NV_LIBCUBLAS_PACKAGE=libcublas-11-8=11.11.3.6-1
SECRET_KEY=2703e1db-a539-4f5d-ac09-c6f8f6a76e8c
TEMPLATE_PATH=/appdata/share/template
UPGRADE_SCHEDULE_SECOND=900
ADMIN_PASSWORD=admin
SERVER_ID=srv1
REDIS_LIST=172.31.39.123:6379
https_proxy=
PG_PASSWORD=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
AMZ_S3_ENABLE=
ARIA2C_SERVER_PORT=6800
HUB_SECRET_PATH=
HTTP_PSERVER_PORT=11113
AMZ_S3_REGION=
NV_LIBCUBLAS_PACKAGE_NAME=libcublas-11-8
HUB_DB_STORAGE_PATH=
DATA_PATH=
QT_QPA_PLATFORM=offscreen
PG_DATABASE=biocolab
AMZ_S3_BUCKET=
BEANSTALKD_SERVER_IP=127.0.0.1
JWT_SECRET_KEY=5366a55744659eaf6b85d5dc6d9c0c4a
MQTT_SERVER_PORT=9001
LESSCLOSE=/usr/bin/lesspipe %s %s
MAKEFLAGS=-j64
JUPYTER_ENABLE_LAB=yes
MAMBA_EXE=/miniconda/user/bin/mamba
HUB_LIST_IPS=172.31.39.123
TERM=xterm
LOG_PATH=
PG_USERNAME=XXXXXXXXXXXXXX
HOST=0.0.0.0
RUSTUP_HOME=/miniconda/user
LESSOPEN=| /usr/bin/lesspipe %s
TRAEFIK_PROXY_MODE=false
GOTRACEBACK=
SSL_NO_VERIFY=1
CURL_CA_BUNDLE=
NO_PROXY=localhost,fc00::/7,.svc,kubernetes,127.0.0.1,10.0.0.0/8,10.42.0.90,.local,fe80::/10,192.168.10.0/24,.cluster.local,::1/128,.default,0.0.0.0
SERVER_VERSION=2.0.38
VERIFY_SSL_CERT=0
GIT_DISCOVERY_ACROSS_FILESYSTEM=1
DISPLAY=:0.0
GOMAXPROCS=
CRAN_URL=https://cloud.r-project.org/
SHLVL=1
APP_DOMAIN_URL=https://<Client BioStudio Domain>
SSHD_SERVER_PORT=2223
NV_CUDA_LIB_VERSION=11.8.0-1
NVARCH=x86_64
HTTPS_PROXY=
HTTP_PROXY=
JULIA_DEPOT_PATH=/miniconda/user/share/julia
HDF5_USE_FILE_LOCKING=FALSE
ROOT_PATH=
PG_PORT=5432
http_proxy=
NV_CUDA_COMPAT_PACKAGE=cuda-compat-11-8
REBUILT_AFTER=2023-03-13
AMZ_S3_SYNC=
RSTUDIO_VERSION=2023.06.1
STRIPTAG_MODE=false
NV_LIBNCCL_PACKAGE=libnccl2=2.15.5-1+cuda11.8
LD_LIBRARY_PATH=/usr/local/nvidia/lib:/usr/local/nvidia/lib64
MQTT_LIST_IPS=172.31.39.123
UPLOAD_PATH=
LC_ALL=C.UTF-8
R_CRAN_WEB=https://cloud.r-project.org
RSESSION_PROXY_RSTUDIO_1_4=yes
PATH=/appdata/bin:/appdata/apps:/usr/local/nvidia/bin:/usr/local/cuda/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/sbin:/usr/bin:/usr/sbin:/usr/X11R6/bin:/bin:/sbin:/root/.local/bin:/miniconda/user/bin:/usr/local/go/bin::/usr/lib/jvm/java-11-openjdk-amd64/bin:/miniconda/user/bin:/usr/local/go/bin:/usr/lib/jvm/java-11-openjdk-amd64/bin:/opt/quarto/bin
MEMCACHED_LIST=172.31.39.123:11211
NV_LIBNCCL_PACKAGE_NAME=libnccl2
MQTT_SERVER_TCP_PORT=1883
NV_LIBNCCL_PACKAGE_VERSION=2.15.5-1
MAMBA_DISABLE_LOCKFILE=FALSE
FLASK_ENV=production
RETICULATE_MINICONDA_ENABLED=TRUE
AMZ_S3_SECRET=
HUB_SECRET_COOKIE=adad744917fc58d2250c2d59400b26c4e45f0fc9af092482cdfd8a5a40c61423
PG_HOST=172.31.39.123
DEBUG=false
SERVICE_ENDPOINT=
MANUAL_REGISTER_KERNEL=
DEBIAN_FRONTEND=noninteractive
CONTENT_PATH=
BEANSTALKD_SERVER_PORT=11300
ARIA2C_LIST_IPS=172.31.39.123
SUPERSET_ENV=production
_=/usr/bin/env


root@c355340b52ce:/home# cat /etc/environment
PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin"
no_proxy="kubernetes,.svc,.default,localhost,0.0.0.0,.cluster.local,172.17.0.0/16,fe80::/10,.local,172.17.0.3,fc00::/7,::1/128,192.168.10.0/24,10.0.0.0/8,10.42.0.90,127.0.0.1"

```

### BioStudio process verification

**Process running with Bioproxy container**

```R
root@ip-172-31-39-123:/biocolab/installation-2.0.53/biocolab# docker exec -it bioproxy /bin/bash
root@507cd2637a97:/home# ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 03:50 pts/0    00:00:00 /bin/bash /super.sh
root         204       1  0 03:50 pts/0    00:00:02 /usr/bin/python3 /usr/bin/supervisord -n -c /etc/supervisor/supervisord.conf
root         205     204  0 03:50 pts/0    00:00:00 /usr/sbin/cron -f
memcach+     206     204  0 03:50 pts/0    00:00:00 /usr/bin/memcached -p 11211 -u memcached -m 128 -c 1024000 -P /memcached/program.pid
postgres     207     204  0 03:50 pts/0    00:00:00 /opt/bitnami/postgresql/bin/postgres -D /bitnami/postgresql/data --config-file=/opt/bitnami/postgresql/conf/po
redis        208     204  0 03:50 pts/0    00:00:11 /usr/bin/redis-server 0.0.0.0:6379
root         219     204  0 03:50 pts/0    00:00:00 nginx: master process /usr/sbin/nginx -g daemon off;
root         220     204  0 03:50 pts/0    00:00:00 /usr/bin/node /server.js
www-data     221     204  0 03:50 pts/0    00:00:04 /usr/local/sbin/haproxy -f /etc/haproxy/haproxy.cfg -p /var/run/haproxy.pid
www-data     253     219  0 03:50 pts/0    00:00:00 nginx: worker process
www-data     254     219  0 03:50 pts/0    00:00:00 nginx: worker process
www-data     255     219  0 03:50 pts/0    00:00:00 nginx: worker process
www-data     257     219  0 03:50 pts/0    00:00:00 nginx: worker process
postgres     308     207  0 03:50 ?        00:00:00 postgres: checkpointer
postgres     309     207  0 03:50 ?        00:00:00 postgres: background writer
postgres     311     207  0 03:50 ?        00:00:00 postgres: walwriter
postgres     312     207  0 03:50 ?        00:00:00 postgres: autovacuum launcher
postgres     313     207  0 03:50 ?        00:00:00 postgres: logical replication launcher
root         336     204  0 03:50 pts/0    00:00:02 /usr/local/bin/dataplaneapi --port 5555 -b /usr/local/sbin/haproxy -c /etc/haproxy/haproxy.cfg -d 5 -r /usr/bi
postgres     705     207  0 03:58 ?        00:00:00 postgres: postgres postgres 172.17.0.1(37132) idle
postgres     706     207  0 03:58 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(37140) idle
postgres     707     207  0 03:58 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(37156) idle
postgres    1036     207  0 04:08 ?        00:00:00 postgres: postgres biocohub 172.17.0.1(57498) idle
root        4206       0  1 05:33 pts/1    00:00:00 /bin/bash
root        4212    4206  0 05:33 pts/1    00:00:00 ps -ef
root@507cd2637a97:/home#
```

**Process running with BioColab container**

```R
root@ip-172-31-39-123:/biocolab/installation-2.0.53/biocolab# docker exec -it biocolab /bin/bash
root@b1a226ccc20a:/home# ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 03:56 pts/0    00:00:00 /bin/bash /super.sh
root         110       1  0 03:56 pts/0    00:00:09 /usr/bin/python3 /usr/bin/supervisord -n -c /etc/supervisor/supervisord.conf
mosquit+     112     110  0 03:56 pts/0    00:00:02 /usr/local/sbin/mosquitto -c /mosquitto/config/mosquitto.conf
beansta+     113     110  0 03:56 pts/0    00:00:00 /usr/local/bin/beanstalkd -b /appdata/beanstalkd -f 1000 -u beanstalkd
root         115     110  0 03:56 pts/0    00:00:00 /usr/bin/Xvfb :0.0 -screen 0 800x600x16 -dpi 75 -nolisten tcp -audit 4 -ac -auth /root/.Xauthority
root         125     110  0 03:56 pts/0    00:00:00 /usr/bin/aria2c --enable-rpc --rpc-listen-all --rpc-allow-origin-all --rpc-secret=************ --rpc-listen-po
root         128     110  0 03:56 pts/0    00:00:00 sshd: /usr/sbin/sshd -p 2223 -D [listener] 0 of 10-100 startups
root         129     110  0 03:56 pts/0    00:00:00 /usr/sbin/cron -f
root         462     110  1 03:58 pts/0    00:01:43 /appdata/apps/t2d_dsc_tool
root         484     110  0 03:58 pts/0    00:00:10 /appdata/apps/t2d_blc_tool
root        1846     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1858     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1867     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1880     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1881     110  0 04:06 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1882     110  0 04:06 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1883     110  0 04:06 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1884     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1885     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1886     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1887     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1888     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1889     110  0 04:06 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1890     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1891     110  0 04:06 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root        1957     110  0 04:08 pts/0    00:00:00 /bin/bash /start.sh
root        1958    1957  0 04:08 pts/0    00:00:04 /miniconda/user/bin/python3.10 /miniconda/user/bin/jupyterhub --config /configs/hub/etc/config.py --ip 0.0.0.0
root        1965    1958  0 04:08 ?        00:00:01 node /miniconda/user/bin/configurable-http-proxy --ip 0.0.0.0 --port 18000 --api-ip 127.0.0.1 --api-port 18001
root        1975    1958  0 04:08 ?        00:00:00 /miniconda/user/bin/python3.10 -m jupyterhub_idle_culler --timeout=36000
root        2021     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2022     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2023     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2024     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2025     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2026     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2027     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2028     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2029     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2030     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2031     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2032     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2033     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2034     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2035     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2036     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2037     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2038     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2039     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2040     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker
root        2094     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root        2095     110  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root        2107     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2108     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2109     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2110     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2111     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2112     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2113     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2114     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2115     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2116     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2117     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2118     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2119     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2120     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2121     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2122     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2123     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2124     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2125     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2126     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2127     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2128     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2129     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2130     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        2131     110  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root        5607       0  1 05:34 pts/1    00:00:00 /bin/bash
root        5619    5607  0 05:34 pts/1    00:00:00 ps -ef
root@b1a226ccc20a:/home#
```
### curl command testing

```R
curl <localhost>
curl <localhost>:<http port>
curl <localhost>:<application port>
curl <localhost>:<nginx port>
```

:bell: **NOTE** : BioStudio is running on http (80) and https (443)

**Curl with host**

```R
root@ip-172-31-39-182:/biocolab/installation-2.0.53# curl localhost 
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta property="og:type" content="article" />
    <meta property="og:url" content="https://studio.bioturing.com/" />
    <meta property="og:description" content="BioStudio is the complete analytics platform that empowers scientists to expand their research
 horizons without technical complexities." />
    <meta property="og:image" content="https://cdn.bioturing.com/shared/hero_banner.webp" />
    <meta property="og:title" content="Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed f
or bioinformaticians" />
    <title>Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed for bioinformaticians</title>
    <link rel="icon" type="image/x-icon" href="//localhost/static/favicon.ico" />
    <link rel="stylesheet" href="//localhost/static/widgets/dsc.css?v=2023102981838">
    <script src="//localhost/static/js/tailwind.js"></script>
    <script src="//localhost/static/js/tailwind.config.js?v=2023102981838"></script>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/global.css?v=2023102981838"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/jquery-backToTop.min.css"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/fontawesome.5631.min.css"/>
    <link
      rel="stylesheet"
      type="text/css"
      href="//localhost/static/css/toastr.min.css"
    />
    <script lang="javascript">
        window.BIOCOLAB_NEED_MQTT = true;
        window.CURRENT_DOMAIN = "https://<Client BioStudio Domain>";
        window.CURRENT_FULL_HOST = "https://localhost";
        window.DSC_DOMAIN = window.location.origin;
        window.CURRENT_URI = "/";
        window.CURRENT_USER = "{}";
        window.IS_MAIN_DOMAIN = false;


-------

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53# curl localhost:80

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta property="og:type" content="article" />
    <meta property="og:url" content="https://studio.bioturing.com/" />
    <meta property="og:description" content="BioStudio is the complete analytics platform that empowers scientists to expand their research
 horizons without technical complexities." />
    <meta property="og:image" content="https://cdn.bioturing.com/shared/hero_banner.webp" />
    <meta property="og:title" content="Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed f
or bioinformaticians" />
    <title>Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed for bioinformaticians</title>
    <link rel="icon" type="image/x-icon" href="//localhost/static/favicon.ico" />
    <link rel="stylesheet" href="//localhost/static/widgets/dsc.css?v=2023102981838">
    <script src="//localhost/static/js/tailwind.js"></script>
    <script src="//localhost/static/js/tailwind.config.js?v=2023102981838"></script>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/global.css?v=2023102981838"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/jquery-backToTop.min.css"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/fontawesome.5631.min.css"/>
    <link
      rel="stylesheet"
      type="text/css"
      href="//localhost/static/css/toastr.min.css"
    />
    <script lang="javascript">
        window.BIOCOLAB_NEED_MQTT = true;
        window.CURRENT_DOMAIN = "https://<Client BioStudio Domain>";
        window.CURRENT_FULL_HOST = "https://localhost";
        window.DSC_DOMAIN = window.location.origin;
        window.CURRENT_URI = "/";
        window.CURRENT_USER = "{}";
        window.IS_MAIN_DOMAIN = false;


-------

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53# curl localhost:11123
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta property="og:type" content="article" />
    <meta property="og:url" content="https://studio.bioturing.com/" />
    <meta property="og:description" content="BioStudio is the complete analytics platform that empowers scientists to expand their research
 horizons without technical complexities." />
    <meta property="og:image" content="https://cdn.bioturing.com/shared/hero_banner.webp" />
    <meta property="og:title" content="Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed f
or bioinformaticians" />
    <title>Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed for bioinformaticians</title>
    <link rel="icon" type="image/x-icon" href="//localhost:11123/static/favicon.ico" />
    <link rel="stylesheet" href="//localhost:11123/static/widgets/dsc.css?v=2023102981838">
    <script src="//localhost:11123/static/js/tailwind.js"></script>
    <script src="//localhost:11123/static/js/tailwind.config.js?v=2023102981838"></script>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/global.css?v=2023102981838"/>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/jquery-backToTop.min.css"/>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/fontawesome.5631.min.css"/>
    <link
      rel="stylesheet"
      type="text/css"
      href="//localhost:11123/static/css/toastr.min.css"
    />
    <script lang="javascript">
        window.BIOCOLAB_NEED_MQTT = true;
        window.CURRENT_DOMAIN = "https://<Client BioStudio Domain>";
        window.CURRENT_FULL_HOST = "https://localhost:11123";
        window.DSC_DOMAIN = window.location.origin;
        window.CURRENT_URI = "/";
        window.CURRENT_USER = "{}";
        window.IS_MAIN_DOMAIN = false;
```

**Curl inside the container**

```R

# BioProxy container 

root@ip-172-31-39-182:/biocolab/installation-2.0.53# docker exec -it bioproxy /bin/bash
root@6c1fca69acf1:/home# curl localhost
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta property="og:type" content="article" />
    <meta property="og:url" content="https://studio.bioturing.com/" />
    <meta property="og:description" content="BioStudio is the complete analytics platform that empowers scientists to expand their research
 horizons without technical complexities." />
    <meta property="og:image" content="https://cdn.bioturing.com/shared/hero_banner.webp" />
    <meta property="og:title" content="Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed f
or bioinformaticians" />
    <title>Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed for bioinformaticians</title>
    <link rel="icon" type="image/x-icon" href="//localhost/static/favicon.ico" />
    <link rel="stylesheet" href="//localhost/static/widgets/dsc.css?v=2023102981838">
    <script src="//localhost/static/js/tailwind.js"></script>
    <script src="//localhost/static/js/tailwind.config.js?v=2023102981838"></script>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/global.css?v=2023102981838"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/jquery-backToTop.min.css"/>
    <link rel="stylesheet" type="text/css" href="//localhost/static/css/fontawesome.5631.min.css"/>
    <link
      rel="stylesheet"
      type="text/css"
      href="//localhost/static/css/toastr.min.css"
    />
    <script lang="javascript">
        window.BIOCOLAB_NEED_MQTT = true;
        window.CURRENT_DOMAIN = "https://<Client BioStudio Domain>";
        window.CURRENT_FULL_HOST = "https://localhost";
        window.DSC_DOMAIN = window.location.origin;
        window.CURRENT_URI = "/";
        window.CURRENT_USER = "{}";
        window.IS_MAIN_DOMAIN = false;


-------

-------

# BioColab Container

NOTE: Here we can only curl with application port.

root@5fc5db8bc5cf:/home# curl localhost:11123 
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
 37  168k   37 65219   <!DOCTYPE html>      0 --:--:-- --:--:-- --:--:--     0
 0 <html lang="en">

   <head>
0   159k      <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta property="og:type" content="article" />
     <meta property="og:url" content="https://studio.bioturing.com/" />
  0  0:00:01 --:--:--  0:00:    <meta property="og:description" content="BioStudio is the complete analytics platform that empowers scientists to expand their research
01  159k horizons without technical complexities." />
    <meta property="og:image" content="https://cdn.bioturing.com/shared/hero_banner.webp" />
    <meta property="og:title" content="Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed f
or bioinformaticians" />
    <title>Provides curated, ready-to-run notebooks, multi-omics data, and applications specifically designed for bioinformaticians</title>
    <link rel="icon" type="image/x-icon" href="//localhost:11123/static/favicon.ico" />
    <link rel="stylesheet" href="//localhost:11123/static/widgets/dsc.css?v=2023102981838">
    <script src="//localhost:11123/static/js/tailwind.js"></script>
    <script src="//localhost:11123/static/js/tailwind.config.js?v=2023102981838"></script>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/global.css?v=2023102981838"/>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/jquery-backToTop.min.css"/>
    <link rel="stylesheet" type="text/css" href="//localhost:11123/static/css/fontawesome.5631.min.css"/>
    <link
      rel="stylesheet"
      type="text/css"
      href="//localhost:11123/static/css/toastr.min.css"
    />
    <script lang="javascript">
        window.BIOCOLAB_NEED_MQTT = true;
        window.CURRENT_DOMAIN = "https://<Client BioStudio Domain>";
        window.CURRENT_FULL_HOST = "https://localhost:11123";
        window.DSC_DOMAIN = window.location.origin;
        window.CURRENT_URI = "/";
        window.CURRENT_USER = "{}";
        window.IS_MAIN_DOMAIN = false;


```

### Check nslookup

```R
nslookup <Domain name>

root@ip-172-31-39-182:/biocolab/installation-2.0.53# nslookup <Client BioStudio Domain>
Server:         127.0.0.53
Address:        127.0.0.53#53

Non-authoritative answer:
Name:   <Client BioStudio Domain>
Address: 54.203.5.109

root@ip-172-31-39-182:/biocolab/installation-2.0.53# 
```

### check whiltelist of domian

**Check with host**

```R
# curl https://colab.biotruing.com
-- Should show contents

# curl https://cdn.biotruing.com
# wget https://cdn.bioturing.com/documentation/adm.png

# curl https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com
# wget https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com/colab/apps/0w-byh0iNCWigGEjbZybU.92ae1dec-6bf9-4041-9d06-330e0fe7b564.zip

# curl https://s3.us-west-2.amazonaws.com/cdn.bioturing.com
# wget https://s3.us-west-2.amazonaws.com/cdn.bioturing.com/documentation/adm.png

# curl https://studio.bioturing.com
-- Should show contents
```

**Check inside the both containers**

```R

# Both container should show the same output and all would have the result.

# curl https://colab.biotruing.com
-- Should show contents

# curl https://cdn.biotruing.com
# wget https://cdn.bioturing.com/documentation/adm.png

# curl https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com
# wget https://cdn-eu-west-1.s3.eu-west-1.amazonaws.com/colab/apps/0w-byh0iNCWigGEjbZybU.92ae1dec-6bf9-4041-9d06-330e0fe7b564.zip

# curl https://s3.us-west-2.amazonaws.com/cdn.bioturing.com
# wget https://s3.us-west-2.amazonaws.com/cdn.bioturing.com/documentation/adm.png

# curl https://studio.bioturing.com
-- Should show contents

```

### Check application varification processes

**with Host machine**

```R
# ps -ef | grep 'docker'
# ps -ef | grep 'miniconda'
# ps -ef | grep nginx
# ps -ef | grep postgres


root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# ps -ef | grep 'docker'
root        4243       1  1 03:24 ?        00:02:54 /usr/bin/dockerd -H fd:// --containerd=/run/containerd/containerd.sock
root        9893    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 32767 -container-ip 172.17.0.2 -container-port 32767
root        9900    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 32767 -container-ip 172.17.0.2 -container-port 32767
root        9915    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 32765 -container-ip 172.17.0.2 -container-port 32765
root        9921    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 32765 -container-ip 172.17.0.2 -container-port 32765
root        9937    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 11211 -container-ip 172.17.0.2 -container-port 11211
root        9943    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 11211 -container-ip 172.17.0.2 -container-port 11211
root        9958    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 9091 -container-ip 172.17.0.2 -container-port 9091
root        9965    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 9091 -container-ip 172.17.0.2 -container-port 9091
root        9982    4243  0 04:04 ?        00:00:06 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 6379 -container-ip 172.17.0.2 -container-port 6379
root        9988    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 6379 -container-ip 172.17.0.2 -container-port 6379
root       10009    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 5432 -container-ip 172.17.0.2 -container-port 5432
root       10030    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 5432 -container-ip 172.17.0.2 -container-port 5432
root       10059    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 443 -container-ip 172.17.0.2 -container-port 443
root       10066    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 443 -container-ip 172.17.0.2 -container-port 443
root       10081    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 80 -container-ip 172.17.0.2 -container-port 80
root       10088    4243  0 04:04 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 80 -container-ip 172.17.0.2 -container-port 80
root       10736    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 18000 -container-ip 172.17.0.3 -container-port 18000
root       10744    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 18000 -container-ip 172.17.0.3 -container-port 18000
root       10757    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 11300 -container-ip 172.17.0.3 -container-port 11300
root       10764    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 11300 -container-ip 172.17.0.3 -container-port 11300
root       10778    4243  0 04:08 ?        00:00:05 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 11123 -container-ip 172.17.0.3 -container-port 11123
root       10786    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 11123 -container-ip 172.17.0.3 -container-port 11123
root       10802    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 9001 -container-ip 172.17.0.3 -container-port 9001
root       10809    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 9001 -container-ip 172.17.0.3 -container-port 9001
root       10821    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 6800 -container-ip 172.17.0.3 -container-port 6800
root       10829    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 6800 -container-ip 172.17.0.3 -container-port 6800
root       10842    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip 0.0.0.0 -host-port 1883 -container-ip 172.17.0.3 -container-port 1883
root       10849    4243  0 04:08 ?        00:00:00 /usr/bin/docker-proxy -proto tcp -host-ip :: -host-port 1883 -container-ip 172.17.0.3 -container-port 1883
root       46489    1507  0 07:54 pts/1    00:00:00 grep --color=auto docker
root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# 

-------

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# ps -ef | grep 'miniconda'
root       11186   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11187   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11188   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11189   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11190   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11191   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11192   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11193   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11194   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11195   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11196   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11197   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11199   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11200   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11201   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11202   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11203   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11204   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11205   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11206   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root       11218   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root       11219   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root       11220   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11221   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11222   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11223   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11224   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11225   11035  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11226   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11229   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11230   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11231   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11232   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11234   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11235   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11236   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11237   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11238   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11239   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11240   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11241   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11242   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11243   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11244   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11245   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11246   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11247   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root       11248   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11249   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11250   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11251   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11252   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11253   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11254   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11255   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11256   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11257   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11258   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11259   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11260   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11261   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11262   11035  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root       11264   11263  0 04:08 pts/0    00:00:10 /miniconda/user/bin/python3.10 /miniconda/user/bin/jupyterhub --config /configs/hub/etc/config.py --ip 0.0.0.0 --port 18000 --no-ssl
root       11422   11264  0 04:08 ?        00:00:02 node /miniconda/user/bin/configurable-http-proxy --ip 0.0.0.0 --port 18000 --api-ip 127.0.0.1 --api-port 18001 --error-target http://5fc5db8bc5cf:18081/hub/error --log-level info
root       11436   11264  0 04:08 ?        00:00:00 /miniconda/user/bin/python3.10 -m jupyterhub_idle_culler --timeout=36000
root       46573    1507  0 07:54 pts/1    00:00:00 grep --color=auto miniconda
root@ip-172-31-39-182:/biocolab/installation-2.0.53/test#

-------

-------


root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# ps -ef | grep nginx
root       10327   10312  0 04:04 pts/0    00:00:00 nginx: master process /usr/sbin/nginx -g daemon off;
www-data   10374   10327  0 04:04 pts/0    00:00:00 nginx: worker process
www-data   10375   10327  0 04:04 pts/0    00:00:00 nginx: worker process
www-data   10376   10327  0 04:04 pts/0    00:00:00 nginx: worker process
www-data   10377   10327  0 04:04 pts/0    00:00:00 nginx: worker process
root       46627    1507  0 07:54 pts/1    00:00:00 grep --color=auto nginx
root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# 

-------

-------

root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# ps -ef | grep postgres
ubuntu     10315   10312  0 04:04 pts/0    00:00:00 /opt/bitnami/postgresql/bin/postgres -D /bitnami/postgresql/data --config-file=/opt/bitnami/postgresql/conf/postgresql.conf --external_pid_file=/opt/bitnami/postgresql/tmp/postgresql.pid --hba_file=/opt/bitnami/postgresql/conf/pg_hba.conf
ubuntu     10384   10315  0 04:04 ?        00:00:00 postgres: checkpointer
ubuntu     10385   10315  0 04:04 ?        00:00:00 postgres: background writer
ubuntu     10388   10315  0 04:04 ?        00:00:00 postgres: walwriter
ubuntu     10389   10315  0 04:04 ?        00:00:00 postgres: autovacuum launcher
ubuntu     10390   10315  0 04:04 ?        00:00:00 postgres: logical replication launcher
ubuntu     11335   10315  0 04:08 ?        00:00:00 postgres: postgres postgres 172.17.0.1(38918) idle
ubuntu     11336   10315  0 04:08 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(38924) idle
ubuntu     11421   10315  0 04:08 ?        00:00:00 postgres: postgres biocohub 172.17.0.1(38936) idle
ubuntu     11516   10315  0 04:09 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(55506) idle
root       46638    1507  0 07:55 pts/1    00:00:00 grep --color=auto postgres
root@ip-172-31-39-182:/biocolab/installation-2.0.53/test#
```

**Check process with BioProxy container**

```R
root@ip-172-31-39-182:/biocolab/installation-2.0.53/test# docker exec -it  bioproxy /bin/bash
root@6c1fca69acf1:/home# ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 04:04 pts/0    00:00:00 /bin/bash /super.sh
root         167       1  0 04:04 pts/0    00:00:06 /usr/bin/python3 /usr/bin/supervisord -n -c /etc/supervisor/supervisord.conf
root         168     167  0 04:04 pts/0    00:00:00 /usr/sbin/cron -f
memcach+     169     167  0 04:04 pts/0    00:00:02 /usr/bin/memcached -p 11211 -u memcached -m 128 -c 1024000 -P /memcached/program.pid   
postgres     170     167  0 04:04 pts/0    00:00:00 /opt/bitnami/postgresql/bin/postgres -D /bitnami/postgresql/data --config-file=/opt/bit
redis        171     167  0 04:04 pts/0    00:00:25 /usr/bin/redis-server 0.0.0.0:6379
root         182     167  0 04:04 pts/0    00:00:00 nginx: master process /usr/sbin/nginx -g daemon off;
root         183     167  0 04:04 pts/0    00:00:00 /usr/bin/node /server.js
www-data     184     167  0 04:04 pts/0    00:00:10 /usr/local/sbin/haproxy -f /etc/haproxy/haproxy.cfg -p /var/run/haproxy.pid
www-data     229     182  0 04:04 pts/0    00:00:00 nginx: worker process
www-data     230     182  0 04:04 pts/0    00:00:00 nginx: worker process
www-data     231     182  0 04:04 pts/0    00:00:00 nginx: worker process
www-data     232     182  0 04:04 pts/0    00:00:00 nginx: worker process
postgres     239     170  0 04:04 ?        00:00:00 postgres: checkpointer
postgres     240     170  0 04:04 ?        00:00:00 postgres: background writer
postgres     243     170  0 04:04 ?        00:00:00 postgres: walwriter
postgres     244     170  0 04:04 ?        00:00:00 postgres: autovacuum launcher
postgres     245     170  0 04:04 ?        00:00:00 postgres: logical replication launcher
root         298     167  0 04:04 pts/0    00:00:05 /usr/local/bin/dataplaneapi --port 5555 -b /usr/local/sbin/haproxy -c /etc/haproxy/hapr
postgres     467     170  0 04:08 ?        00:00:00 postgres: postgres postgres 172.17.0.1(38918) idle
postgres     468     170  0 04:08 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(38924) idle
postgres     469     170  0 04:08 ?        00:00:00 postgres: postgres biocohub 172.17.0.1(38936) idle
postgres     473     170  0 04:09 ?        00:00:00 postgres: postgres biocolab 172.17.0.1(55506) idle
root        9008       0  0 07:57 pts/1    00:00:00 /bin/bash
root        9014    9008  0 07:57 pts/1    00:00:00 ps -ef
root@6c1fca69acf1:/home#

```

**Check process with BioColab container**

```R
root@5fc5db8bc5cf:/home# ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 04:08 pts/0    00:00:00 /bin/bash /super.sh
root         131       1  0 04:08 pts/0    00:00:10 /usr/bin/python3 /usr/bin/supervisord -n -c /etc/supervisor/supervisord.conf
mosquit+     133     131  0 04:08 pts/0    00:00:06 /usr/local/sbin/mosquitto -c /mosquitto/config/mosquitto.conf
beansta+     134     131  0 04:08 pts/0    00:00:00 /usr/local/bin/beanstalkd -b /appdata/beanstalkd -f 1000 -u beanstalkd
root         136     131  0 04:08 pts/0    00:00:00 /usr/bin/Xvfb :0.0 -screen 0 800x600x16 -dpi 75 -nolisten tcp -audit 4 -ac -auth /root/
root         144     131  0 04:08 pts/0    00:00:00 /usr/bin/aria2c --enable-rpc --rpc-listen-all --rpc-allow-origin-all --rpc-secret=*****
root         147     131  0 04:08 pts/0    00:00:22 /appdata/apps/t2d_blc_tool
root         148     131  0 04:08 pts/0    00:01:50 /appdata/apps/t2d_dsc_tool
root         149     131  0 04:08 pts/0    00:00:00 sshd: /usr/sbin/sshd -p 2223 -D [listener] 0 of 10-100 startups
root         150     131  0 04:08 pts/0    00:00:00 /usr/sbin/cron -f
root         282     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         283     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         284     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         285     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         286     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         287     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         288     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         289     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         290     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         291     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         292     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         293     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         295     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         296     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         297     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         298     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         299     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         300     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         301     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         302     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-custom-task-worker      
root         314     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root         315     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-pack-notebook-worker
root         316     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         317     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         318     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         319     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         320     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         321     131  0 04:08 pts/0    00:00:00 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         322     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         325     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         326     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         327     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         328     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         330     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         331     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         332     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         333     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         334     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         335     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         336     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         337     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         338     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         339     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         340     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         341     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         342     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         343     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-setup-notebook-worker
root         344     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         345     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         346     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         347     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         348     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         349     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         350     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         351     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         352     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         353     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         354     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         355     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         356     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         357     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         358     131  0 04:08 pts/0    00:00:01 /miniconda/user/bin/python3.10 /miniconda/user/bin/bhub-create-kernel-worker
root         359     131  0 04:08 pts/0    00:00:00 /bin/bash /start.sh
root         360     359  0 04:08 pts/0    00:00:10 /miniconda/user/bin/python3.10 /miniconda/user/bin/jupyterhub --config /configs/hub/etc
root         513     360  0 04:08 ?        00:00:02 node /miniconda/user/bin/configurable-http-proxy --ip 0.0.0.0 --port 18000 --api-ip 127
root         527     360  0 04:08 ?        00:00:00 /miniconda/user/bin/python3.10 -m jupyterhub_idle_culler --timeout=36000
root        9394       0  0 07:58 pts/1    00:00:00 /bin/bash
root        9406    9394  0 07:58 pts/1    00:00:00 ps -ef
root@5fc5db8bc5cf:/home#
```

### Application location

**Application location**

**BioColab**

docker exec -it  biocolab /bin/bash

```R
root@5fc5db8bc5cf:/appdata/share/miniconda# ll
total 16
drwxr-xr-x  4 root root 4096 Dec 15 04:08 ./
drwxr-xr-x  6 root root 4096 Dec 15 03:36 ../
drwxr-xr-x  2 root root 4096 Sep 18 08:09 apps/
lrwxrwxrwx  1 root root   24 Dec 15 04:08 miniconda -> /appdata/share/miniconda/
drwxr-xr-x 38 root root 4096 Oct 10 12:41 user/
root@5fc5db8bc5cf:/appdata/share/miniconda# pwd
/appdata/share/miniconda
root@5fc5db8bc5cf:/appdata/share/miniconda#

```

**Installation for APP**

```R
root@5fc5db8bc5cf:/appdata/.bbcache# ls -l
total 12
-rwx------ 1 root root  908 Dec 15 08:08 c446c0082184bd48d6b2ad37b6ab6007.license
-rw------- 1 root root  908 Dec 15 08:08 c446c0082184bd48d6b2ad37b6ab6007.license_bk
drwx------ 4 root root 4096 Dec 15 03:30 searching
root@5fc5db8bc5cf:/appdata/.bbcache# ls searching/
conda.bleve  download
root@5fc5db8bc5cf:/appdata/.bbcache# tree
.
├── c446c0082184bd48d6b2ad37b6ab6007.license
├── c446c0082184bd48d6b2ad37b6ab6007.license_bk
└── searching
    ├── conda.bleve
    │   ├── index_meta.json
    │   └── store
    │       ├── 00000000013c.zap
    │       ├── 00000000014f.zap
    │       ├── 000000000155.zap
    │       ├── 000000000164.zap
    │       ├── 000000000173.zap
    │       ├── 00000000017d.zap
    │       ├── 000000000191.zap
    │       ├── 000000000192.zap
    │       └── root.bolt
    └── download
        ├── anaconda_channeldata.json
        ├── anaconda_channeldata.json.converted
        ├── anaconda_linux-64.json
        ├── anaconda_noarch.json
        ├── bioconda_linux-64.json
        ├── bioconda_noarch.json
        ├── bioturing_linux-64.json
        ├── bioturing_noarch.json
        ├── cctbx202211_linux-64.json
        ├── cctbx202211_noarch.json
        ├── conda-forge_channeldata.json
        ├── conda-forge_channeldata.json.converted
        ├── conda-forge_linux-64.json
        ├── conda-forge_noarch.json
        ├── fastai_linux-64.json
        ├── fastai_noarch.json
        ├── fastchan_linux-64.json
        ├── fastchan_noarch.json
        ├── intel_linux-64.json
        ├── intel_noarch.json
        ├── main_linux-64.json
        ├── main_noarch.json
        ├── nvidia_linux-64.json
        ├── nvidia_noarch.json
        ├── ome_linux-64.json
        ├── ome_noarch.json
        ├── prometeia_linux-64.json
        ├── prometeia_noarch.json
        ├── pytorch_linux-64.json
        ├── pytorch_noarch.json
        ├── r_linux-64.json
        ├── r_noarch.json
        ├── sunpy_linux-64.json
        └── sunpy_noarch.json

4 directories, 46 files
root@5fc5db8bc5cf:/appdata/.bbcache#

```


**Application log**

```R
root@5fc5db8bc5cf:/appdata/logs# pwd
/appdata/logs
root@5fc5db8bc5cf:/appdata/logs# ls -l
total 0
-rwx------ 1 root root 0 Dec 15 03:44 jupyterhub.log
root@5fc5db8bc5cf:/appdata/logs#

# ls -la /var/log/supervisor

root@5fc5db8bc5cf:/appdata/logs# ls -la /var/log/supervisor
total 444
drwx------ 1 root root   4096 Dec 15 04:08 .
drwxr-xr-x 1 root root   4096 Dec 15 04:08 ..
-rwx------ 1 root root      0 Dec 15 04:08 aria2c_stderr.log
-rwx------ 1 root root  12536 Dec 15 07:33 aria2c_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 beanstalkd_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 beanstalkd_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:08 bhub-create-custom-task-worker_stderr.log
-rw-r--r-- 1 root root 108160 Dec 15 08:03 bhub-create-custom-task-worker_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:08 bhub-create-kernel-worker_stderr.log
-rw-r--r-- 1 root root  90120 Dec 15 08:03 bhub-create-kernel-worker_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:08 bhub-pack-notebook-worker_stderr.log
-rw-r--r-- 1 root root  11416 Dec 15 08:03 bhub-pack-notebook-worker_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:08 bhub-setup-notebook-worker_stderr.log
-rw-r--r-- 1 root root 143950 Dec 15 08:03 bhub-setup-notebook-worker_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 cleanup_stderr.log
-rwx------ 1 root root     24 Dec 15 04:08 cleanup_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 colab-unset-vars_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 colab-unset-vars_stdout.log
-rwx------ 1 root root    720 Dec 15 04:08 colab_stderr.log
-rwx------ 1 root root    151 Dec 15 04:08 colab_stdout.log
-rwx------ 1 root root   4050 Dec 15 04:08 colabblc_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 colabblc_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 cron_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 cron_stdout.log
-rwx------ 1 root root    613 Dec 15 04:08 jupyterhub-upgrade-db_stderr.log
-rwx------ 1 root root     26 Dec 15 04:08 jupyterhub-upgrade-db_stdout.log
-rwx------ 1 root root     77 Dec 15 04:08 jupyterhub_stderr.log
-rwx------ 1 root root   3554 Dec 15 08:03 jupyterhub_stdout.log
-rwx------ 1 root root  14333 Dec 15 08:04 mosquitto_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 mosquitto_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 sshd_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 sshd_stdout.log
-rwx------ 1 root root      0 Dec 15 04:08 xvfb_stderr.log
-rwx------ 1 root root      0 Dec 15 04:08 xvfb_stdout.log
root@5fc5db8bc5cf:/appdata/logs#
```

**BioProxy**

docker exec -it  bioproxy /bin/bash

```R
root@6c1fca69acf1:/# ls
bin               checkstatus.sh                 etc    memcached  postgresql-entrypoint.sh    run        sys
bitnami           dev                            home   mnt        prepare_letsencrypt_pem.sh  sbin       tmp
boot              docker-entrypoint-initdb.d     lib    nfs        proc                        server.js  usr
certbot_timer.sh  docker-entrypoint-preinitdb.d  lib64  nfs.sh     renew.sh                    srv        var
checkssl.sh       docker-entrypoint.sh           media  opt        root                        super.sh
root@6c1fca69acf1:/#

-------

-------

root@6c1fca69acf1:/var/log/supervisor# ls -l
total 220
-rw-r--r-- 1 root root     45 Dec 15 04:04 certbot_stderr.log
-rw-r--r-- 1 root root     21 Dec 15 04:04 certbot_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 cron_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 cron_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 dataplaneapi_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 dataplaneapi_stdout.log
-rw-r--r-- 1 root root    997 Dec 15 04:08 haproxy_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 haproxy_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 memcached_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 memcached_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 nfsserver_stderr.log
-rw-r--r-- 1 root root 170850 Dec 15 08:08 nfsserver_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 nginx_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 nginx_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 pgentrypoint_stderr.log
-rw-r--r-- 1 root root     19 Dec 15 04:04 pgentrypoint_stdout.log
-rw-r--r-- 1 root root  24450 Dec 15 08:09 postgresql_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 postgresql_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 redis_stderr.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 redis_stdout.log
-rw-r--r-- 1 root root      0 Dec 15 04:04 sslapi_stderr.log
-rw-r--r-- 1 root root     81 Dec 15 04:04 sslapi_stdout.log
root@6c1fca69acf1:/var/log/supervisor#
```

## Certificate chain

When ever you would have bundle , pem, p7b three files then you must combine pem, bundle.pem and create certificate chain.

```R
cat test.pem test_bundle.pem > test_chained.pem
```

now you would have test_chained.pem and test.p7b file.

```R
# openssl x509 -text -noout -in test_chained.pem
```

above command will show the detail and validation.

## BioStudio Supervior services

All supervisior service configured in below location.

```R
/etc/supervisor/supervisord.conf
```

**Restart t2d services inside BioColab**

```R
root@b1a226ccc20a:/etc/supervisor# supervisorctl restart colabblc:*
colabblc:colabblc_00: stopped
colabblc:colabblc_00: started
```

**Restart haproxy services inside BioColab**

```R
root@507cd2637a97:/home# supervisorctl restart haproxy:*
haproxy:haproxy_00: stopped
haproxy:haproxy_00: started
```

# Installing Nginx Proxy

[Nginx installation : 1](https://ubuntu.com/tutorials/install-and-configure-nginx#1-overview)

[Nginx installation : 2](https://docs.nginx.com/nginx/admin-guide/installing-nginx/installing-nginx-open-source/)

```R
# sudo apt install nginx

root@ip-172-31-39-123:/biocolab/installation-2.0.53/biocolab# curl -I 127.0.0.1
HTTP/1.1 200 OK
Server: nginx/1.18.0 (Ubuntu)
Date: Mon, 18 Dec 2023 07:09:02 GMT
Content-Type: text/html
Content-Length: 612
Last-Modified: Mon, 18 Dec 2023 07:08:18 GMT
Connection: keep-alive
ETag: "657fefe2-264"
Accept-Ranges: bytes

```

:bell: NOTE: Unti, we will not post vhost entry with Nginx, You can see browser window was Nginx s running well.


## Nginx Configuration

[vhost setup](https://serverspace.io/support/help/nginx-virtual-hosts-on-ubuntu-20-04/)

```R
# In case of we are not having SSL

server {
    listen 0.0.0.0:80;
    server_name <Your Domain>.com www.<Your Domain>.com;
    #return 301 https:<Your Domain>.com$request_uri;

    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:8081;
        proxy_http_version 1.1;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Host $http_host;
        add_header X-Host $host;
        proxy_set_header X-Forwarded-Host $http_host;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
    }
    location ~ /\.ht {
        deny all;
    }
}

server {
    listen 0.0.0.0:443;
#       ssl http2;
    server_name <Your Domain>.com www.<Your Domain>.com;
    if ($host = 'www.<Your Domain>.com' ) {
        rewrite  ^/(.*)$  https://<Your Domain>.com/$1  permanent;
    }
    #ssl_certificate /etc/ssl/certs/testdomain.pem;
    #ssl_certificate_key /etc/pki/tls/private/testdomain.key;
    #ssl_session_timeout 1d;
    #ssl_session_cache shared:SSL:20m;
    #ssl_prefer_server_ciphers on;
    #ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
    #ssl_ciphers EECDH+AESGCM:EDH+AESGCM:AES256+EECDH:AES256+EDH;
    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:8081;
        proxy_http_version 1.1;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Host $http_host;
        add_header X-Host $host;
        proxy_set_header X-Forwarded-Host $http_host;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
    }
    location ~ /\.ht {
        deny all;
    }
}
```

# Troubleshoot

## Not able to install Docker.

:o: **Reason**

```R
Ceriticate issue.

 curl: (77) error setting certificate file: /etc/ssl/certs/ca-certificates.crt
```

:o: **Resolution**

```R
# echo insecure >> ~/.curlrc
```

## fstab entry for mount point.

:o: **Reason**

```R
To auto mount patition.
```

:o: **Resolution**

```R
UUID="3ad2185e-82dd-40cd-8d43-1a82a780d0be"     /biocolab   xfs    defaults   0   0
```


## Error code 413 ( Not able to upload large file).

:o: **Reason**

```R
The HTTP 413 Content Too Large response status code signifies that the request entity surpasses the server-defined limits. This issue pertains to resource limitations.
```

:o: **Resolution**

```R
That issue can be fixed by updating the (Nginx) load balancer by incorporating the following value:

client_max_body_size = 0

By implementing this configuration, users will have the flexibility to upload files without any imposed size restrictions. Setting this value to zero will exempt the client request a body size check, allowing users to upload files of unlimited sizes.

- nginx load balancing standalone : client_max_body_size 0
- nginx k8s ingress : nginx.ingress.kubernetes.io/proxy-body-size 0

in case you have seperate Nginx Load Balancer.

    nginx.ingress.kubernetes.io/client_max_body_size: 100m
    nginx.ingress.kubernetes.io/proxy-body-size: 100m
    nginx.ingress.kubernetes.io/proxy-read-timeout: 3600
    nginx.ingress.kubernetes.io/proxy-send-timeout: 3600

--Based on situation -- anotation and values can be vary--

Kubernete ingress:

    nginx.ingress.kubernetes.io/client_max_body_size: 5000M
    nginx.ingress.kubernetes.io/proxy-body-size: 5000M
    nginx.ingress.kubernetes.io/proxy-buffer-size: 16k
    nginx.ingress.kubernetes.io/proxy-connect-timeout: "3600"
    nginx.ingress.kubernetes.io/proxy-read-timeout: "3600"
    nginx.ingress.kubernetes.io/proxy-send-timeout: "3600"
    nginx.ingress.kubernetes.io/use-regex: "true"

    nginx.ingress.kubernetes.io/rewrite-target /;
    nginx.ingress.kubernetes.io/ssl_protocols TLSv1 TLSv1.1 TLSv1.2 TLSv1.3;
    nginx.ingress.kubernetes.io/client-header-buffer-size 100k;

 Nginx lb:


    proxy_buffers 4 256k;
    proxy_buffer_size 256k;
    proxy_busy_buffers_size 256k;
    proxy_connect_timeout 3600s;
    proxy_read_timeout 3600s;
    proxy_send_timeout 3600s;
    client_max_body_size 5000M;

For Nginx LB, the value we updated will not be effective until we restart or reload it.

Restart Nginx in case needed:
 
1] Check Syntax

sudo nginx -t

 
2] Restart

sudo nginx -s reload  

or

sudo systemctl reload nginx  

or

sudo systemctl restart nginx  

```

**Ref**:

[Nginx Proxy Module](https://nginx.org/en/docs/http/ngx_http_proxy_module.html#proxy_buffer_size)
[Nginx HTTP Module](https://nginx.org/en/docs/http/ngx_http_core_module.html#client_max_body_size)
[Nginx Suffix rule](https://nginx.org/en/docs/syntax.html)

## Conda installation error.

:o: **Reason**

```R
There are several reason that conda driver failed to installed. It could be due to network, blocking, Speed, Software incompatibility with OS ...
```

:o: **Resolution**

```R
Driver can be intalled manually.
Kindly visit below site and choose driver according to OS.

https://developer.nvidia.com/cuda-downloads

root@biocolab-server:/lalit-test-nvidia-driver# sh cuda_12.2.2_535.104.05_linux.run
===========
= Summary =
===========

Driver:   Installed
Toolkit:  Installed in /usr/local/cuda-12.2/

Please make sure that
 -   PATH includes /usr/local/cuda-12.2/bin
 -   LD_LIBRARY_PATH includes /usr/local/cuda-12.2/lib64, or, add /usr/local/cuda-12.2/lib64 to /etc/ld.so.conf and run ldconfig as root

To uninstall the CUDA Toolkit, run cuda-uninstaller in /usr/local/cuda-12.2/bin
To uninstall the NVIDIA Driver, run nvidia-uninstall
Logfile is /var/log/cuda-installer.log
root@biocolab-server:/lalit-test-nvidia-driver# 

=====================================
= Solution with cuda version 11.7.1 =
=====================================

sh cuda_11.7.1_515.65.01_linux.run --no-drm

```

## Conda uninstallation.

```R
Sometime, we need to reinstall cuda tool kits. Please follow URL below to uninstall cuda tool kit.

https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html

root@biocolab-server:/usr/local/cuda-12.2/bin# pwd
/usr/local/cuda-12.2/bin
root@biocolab-server:/usr/local/cuda-12.2/bin# ls -lhrt cuda*
-rwxr-xr-x 1 root root   15M Sep 22 05:47 cuda-gdb
-rwxr-xr-x 1 root root  789K Sep 22 05:47 cuda-gdbserver
-rwxr-xr-x 1 root root  6.6M Sep 22 05:49 cudafe++
-rwxr-xr-x 1 root root 1023K Sep 22 05:49 cuda-uninstaller
root@biocolab-server:/usr/local/cuda-12.2/bin#

To uninstall cuda driver. Just run uninstallation script.

cd /usr/local/cuda-12.2/bin

root@biocolab-server:/usr/local/cuda-12.2/bin# ./cuda-uninstaller
 Successfully uninstalled 

```

<img alt="Troubleshoot" src="https://cdn.bioturing.com/documentation/TR_SHOOT/tru.png" class="lazy" width="100%"> 

## Containers are failed to start automatically.

:o: **Reason**

```R
There could be several reasons. It could be port mapping or ports are already in use ...etc
```

:o: **Resolution**

```R
Try to identify exact reason by start container manaully by following commands below.

Check docker status

# systemctl status docker.service

# systemctl status docker.service

# docker info 

Check container status

# docker ps -a

Run container manually

# docker start biocolab

# docker start bioproxy

Chcek container log to see if we could see any errors

# docker logs biocolab

# docker logs bioproxy

NOTE: Service should be disable which cause port issue. Like NFS.

```

:pencil2: **Please contact** :e-mail: [**support@bioturing.com**] and share your issue.

## Not able to launch server once try to go inside WORKSPACE.

<br><img alt="Troubleshoot" src="https://cdn.bioturing.com/documentation/TR_SHOOT/trw.png" class="lazy" width="100%"><br>

:o: **Reason**

```R
This issue is related to machine creation is not correct and volume. It could be wrong (Private IP) or wrong DNS.
```

:o: **Resolution**

```R
In order to resovle this issue. Please check and make sure that you configured machine private IP / DNS correctly.

Kindly run the following command to check machine IP.

# docker exec biocolab cat /etc/hosts

Check Machine Private IP configured with your DNS. 

Note this IP and cross check with Machine IP creation on Admin dashboard.

http://<Domain name>/dashboard.

Kindly check you must create volume attached with this machine. 

NOTE: volume name can be anything but Volume path should be "/home"

```

## Not able to download notebook.

:o: **Reason**

```R
There could be several reason behind this issue. Common reason is blocking below sites.

*.bioturing.com
*.anaconda.org
*repo.anaconda.com
Amazon S3
github.com
cdn-eu-west-1.s3.eu-west-1.amazonaws.com (euro -west1)
s3.us-west-2.amazonaws.com/cdn.bioturing.com (us -west2)
cdn.bioturing.com (us -west2)
```

:o: **Resolution**

```R
Kindly allow below sites.
*.bioturing.com
*.anaconda.org
*repo.anaconda.com
Amazon S3
github.com
cdn-eu-west-1.s3.eu-west-1.amazonaws.com (euro -west1)
s3.us-west-2.amazonaws.com/cdn.bioturing.com (us -west2)
cdn.bioturing.com (us -west2)
```

## Workspace / any other element access is not showing graphics clear and images are not showing correctly.

:o: **Reason**

```R
This issue is related to redirection from Load Balancer.
```

:o: **Resolution**

```R
Please check redirection rule on Load Balancer.

It should be "/*"

So that load balancer allowed all redirections.
```

## Nginx config for BioStudio in case installing on the same server.

**Bioturing ecosystem**
```R
server {
    listen 0.0.0.0:80;
    server_name <test-domain.com> www.<test-domain.com>;
    return 301 https://<test-domain.com>$request_uri;
}
server {
    listen 0.0.0.0:443 ssl http2;
    # listen 0.0.0.0:443;
    server_name <test-domain.com> www.<test-domain.com>;
    if ($host = 'www.<test-domain.com>' ) {
        rewrite  ^/(.*)$  https://<test-domain.com>/$1  permanent;
    }
    ssl_certificate /etc/ssl/certs/<test-domain.com>.pem;
    ssl_certificate_key /etc/pki/tls/private/<test-domain.com>.key;
    ssl_session_timeout 1d;
    ssl_session_cache shared:SSL:20m;
    ssl_prefer_server_ciphers on;
    ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
    ssl_ciphers EECDH+AESGCM:EDH+AESGCM:AES256+EECDH:AES256+EDH;
    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:3000/;
        proxy_intercept_errors on;
        error_page 404 /404_not_found;
    }
}

```

**BioStudio**

```R
server {
    listen 0.0.0.0:80;
    server_name <testdomain>.com www.<testdomain>.com;
    return 301 https://<testdomain>.com$request_uri;

    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:8081;
        proxy_http_version 1.1;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Host $http_host;
        add_header X-Host $host;
        proxy_set_header X-Forwarded-Host $http_host;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
    }
    location ~ /\.ht {
        deny all;
    }
}

server {
    listen 0.0.0.0:443 ssl http2;
    server_name <testdomain>.com www.<testdomain>.com;
    if ($host = 'www.<testdomain>.com' ) {
        rewrite  ^/(.*)$  https://<testdomain>.com/$1  permanent;
    }
    ssl_certificate /etc/ssl/certs/testdomain.pem;
    ssl_certificate_key /etc/pki/tls/private/testdomain.key;
    ssl_session_timeout 1d;
    ssl_session_cache shared:SSL:20m;
    ssl_prefer_server_ciphers on;
    ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
    ssl_ciphers EECDH+AESGCM:EDH+AESGCM:AES256+EECDH:AES256+EDH;
    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:8081;
        proxy_http_version 1.1;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Host $http_host;
        add_header X-Host $host;
        proxy_set_header X-Forwarded-Host $http_host;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
    }
    location ~ /\.ht {
        deny all;
    }
}


============== OR ============== 

server {
    listen 0.0.0.0:80;
    server_name <testdomain>.com www.<testdomain>.com;
    return 301 https://<testdomain>.com$request_uri;
}

server {
    listen 0.0.0.0:443 ssl http2;
    server_name <testdomain>.com www.<testdomain>.com;
    if ($host = 'www.<testdomain>.com' ) {
        rewrite  ^/(.*)$  https://<testdomain>.com/$1  permanent;
    }
    ssl_certificate /etc/ssl/certs/testdomain.pem;
    ssl_certificate_key /etc/pki/tls/private/testdomain.key;
    ssl_session_timeout 1d;
    ssl_session_cache shared:SSL:20m;
    ssl_prefer_server_ciphers on;
    ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
    ssl_ciphers EECDH+AESGCM:EDH+AESGCM:AES256+EECDH:AES256+EDH;
    ignore_invalid_headers off;
    client_max_body_size 0;
    client_body_timeout 1d;
    proxy_buffering off;
    proxy_read_timeout 1d;
    proxy_connect_timeout 1d;
    proxy_send_timeout 1d;
    location / {
        proxy_pass http://127.0.0.1:8080;
        proxy_http_version 1.1;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Host $http_host;
        add_header X-Host $host;
        proxy_set_header X-Forwarded-Host $http_host;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
    }
    location ~ /\.ht {
        deny all;
    }
}



============== OR ==============

# In case you have external Load balancers

upstream bioturing_router_http {
    ip_hash;
    server XX.XX.X.XX:80;
    server XX.XX.X.XX:80;
}

server {
    listen 443 ssl http2;
    server_name biocolab.pass-yellow.astrazeneca.net;
    ssl_certicate /etc/ssl/certs/pass-astrazeneca_net-yellow.crt;
    ssl_certicate_key /etc/ssl/certs/pass-astrazeneca_net-yellow.key;
    ssl_protocols TLSv1 TLSv1.1 TLSv1.2 TLSv1.3;

    location / {
        # For reverse proxy to backends
        proxy_pass http://bioturing_router_http;
        proxy_redirect off;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For  $proxy_add_x_forwarded_for;
        proxy_connect_timeout 3600;
        proxy_read_timeout 3600;
        proxy_write_timeout 3600;


        # For HTTP/HTTPS
        client_max_body_size 5000m;
        client_header_buffer_size 16k;
          large_client_header_buffers  4 32k;

        # For websocket
        proxy_http_version 1.1;
        proxy_set_header Upgrade "websocket";
        proxy_set_header Connection 'Upgrade';
        proxy_cache_bypass "websocket";
        proxy_set_header Connection “keep-alive”;
    }
}

# In K8s Nginx Ingress. Please help to make sure that the below annotation is set up.

nginx.ingress.kubernetes.io/rewrite-target /;
nginx.ingress.kubernetes.io/ssl_protocols TLSv1 TLSv1.1 TLSv1.2 TLSv1.3;
nginx.ingress.kubernetes.io/client-header-buffer-size 100k;
```
## Multiple redirection and timeout issue.

:o: **Reason**

```R
Ingress setting is not correct on LB.
```

:o: **Resolution**

```R
There is no any specific solution. Issue could be form Load Balancer or would be form Application.
```

:o: **How to test websocket?**

```R
BioStudio has an inbuilt feature to test Websocket.

1] Login to BioStudio Admin dashboard.

2] Select System Setting -- Click to Check BioStudio button

```

<br><img alt="Protocol" src="https://cdn.bioturing.com/documentation/EKS_PIC/cbs.png" class="lazy" width="100%"><br><br> 

```R
You could see the result below.
```

<br><br> <img alt="Protocol" src="https://cdn.bioturing.com/documentation/EKS_PIC/cbc.png" class="lazy" width="100%"> 