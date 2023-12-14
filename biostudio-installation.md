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


| **Item**                 | **Note**                                                            | **Size** |
|--------------------------|---------------------------------------------------------------------|----------|
| BioStudio Token           | To access our product.                                              |          |
| Application Domain       | Access BioStudio on Browser.                                         |          |
| META_DATA Volume         | This will use by Bioproxy to store database. [**/biocolab/metadata**]  | 50GB     |
| SSL Volume               | Using by BioProxy. [**/biocolab/configs**]                                  | 1GB or above      |
| Data Volume              | Using to store user data. [**/biocolab/userdata**]                                   | 500GB or above   |
| Application data Volume  | Used to store application binary data.[**/biocolab/appdata**]                    | 100GB or above    |
| Ethernet IP Address       | Use to pass IP address during installation (**eth0**) |  |

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

wget https://github.com/bioturing/installation/archive/refs/tags/v2.0.51.tar.gz

# uncompressed .gz
tar xvf v2.0.51.tar.gz

# Switch to installation folder
cd installation-2.0.51/

# Execute installation script
bash install.biocolab.docker.sh

# Verify both container up and running.
docker ps -a

# Configure SSO login
http://<Your Domain>/dashboard/
```

:large_orange_diamond: Download **v2.0.51.tar.gz**, which content script to install **BioStudio.**

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
| serviceAccount.name                       | string   | ""                 |                      |
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