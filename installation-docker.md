## BioStudio installation using Docker container.

We'd like to thank you for choosing **BioStudio**. It is so easy to install. We just need to run the installation script and follow the instructions.

Feel free to explore detailed information for BioStudio architecture and installation.

:link: [Architecture Documents](https://studio.bioturing.com/document/architecture)

:link: [Installation](https://studio.bioturing.com/document/installation)

**1]** System Requirements


|| **Basic recommendation**| **Optional**|
|---------------------|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| **CPU**             | <strong style="color:red;">16 core</strong>| This is basic requirement to start  BioStudio and based on requirement, Resources as well as machine can be added.  |
| **RAM**             | <strong style="color:red;">64 GB</strong> | As above                                                                                                           |
| **HDD**             | / partition can be 100 GB | As above.                                                                                      |
|                     | Data Volume : 1TB| As above.                                                                                                |
| **OS**              | Any OS. Ubuntu 20.04 and above.| BioStudio is more supportive with Linux OS. For better performance linux OS is recommended.|
| **AWS Instance**    | Support any type of instance type. Depend on needs| AWS <strong style="color:red;">g5.4xlarge</strong> in case using GPU.                                          |
|**Platform**         | Docker / Kubernetes                                                                                                        |

**GPU:** This is <strong style="color:red;">optional</strong>. If users want to run notebooks based on GPUs, then we need GPU-supported instances. We can install BioStudio on any type of instance, and in the future, it can be upgraded to a GPU.

**Other:** Yes, other types ( CPU ) also support.

**2]**  BioStudio Partition details:

- **app** : it used to store application related data. ( **100GB** )
- **metadata** : It is used to store postgresql database. ( **50GB** )
- **user** : It used to store user's data. Like user's generated notebooks and other works. ( **500GB or above** )
- **configs** : It used to store server configs. It can be ( **1GB or above** )

**3]** **Domain name** :
domain name:  DNS name obtained for BioStudio.

**4]** **BioStudio Authentication** :

Authentication: **SSO**
BioStudio supports three types of protocol ( **SAML, OPENID and OAUTH2** ) with all types of service providers.

:link:[SSO Set up](https://studio.bioturing.com/document/installation#p-stylecolor-000080-sso-set-up-p)

**5]** Network requirements:

Access to these domains is required for the machine with the BioStudio software installed, as we need to retrieve data from the BioTuring ecosystem server.

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


Installation Steps:

Once the machine is ready to install.  

Please **mount** data volume as **/biocolab**

Update **fstab** entry by adding line below.

```R
[Partition-name] /biocolab   xfs    defaults   0   0
```

:link: [Installation Steps](https://studio.bioturing.com/document/installation#installation-started)

**1]** Login to the server and create the required folder structure before execution.

```R
mkdir -p /biocolab/metadata
mkdir -p /biocolab/configs
mkdir -p /biocolab/userdata ( minimum 500GB or above )
mkdir -p /biocolab/appdata ( minimum 100GB or above )
```

**2]** Switch to biocolab folder.

```R
cd /biocolab
```

**3]** Download installation script.

```R
wget https://github.com/bioturing/installation/archive/refs/tags/V2.0.53.tar.gz
```

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/wget.png" class="lazy" width="100%"><br>

**4]** Uncompressed .gz file.

```R
tar xvf V2.0.53.tar.gz
```

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/t.png" class="lazy" width="100%"><br>

**5]** Switch to the installation folder.

```R
cd installation-2.0.53/
```

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/cd.png" class="lazy" width="100%"><br>

 
**6]** Execute installation script.

```R
bash install.biocolab.docker.sh
```

Following script execution instructions: 

**1]** During the execution, It will prompt for “**Install Self-Signed CA Certificate [y, n]**”: **n**

( We can use **n** )

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ca.png" class="lazy" width="100%"><br>

 
**2]** Next it will prompt for folder structure confirmation.

As we already created before. We just need to press the ENTER key to move to the next step.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/f.png" class="lazy" width="100%"><br>
 
**3]** Script will prompt for Token and Domain name. 

Please use the token provided by us.
Your specific domain name for BioStudio.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/dn.png" class="lazy" width="100%"><br>

**4]** Next step to set up credential for super user account. 
Please provide **password** for Admin user.

**NOTE:** Kindly keep save this password. We can not recovery it once lost.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/adm.png" class="lazy" width="100%"><br>

**5]** Input exposes ports.
We can use HTTP : 80 and HTTPS : 443

:bell: **Note:** If you are installing BioTuring ecosystem and BioStudio on the same machine. Please use different port like 8081 for HTTP and 4433 for HTTPS.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/po.png" class="lazy" width="100%"><br>

Wait for a while to install docker on your machine.

**6]** Instance / machine type selection ( GPU / CPU )

**Note:** Please be careful to select this option. 
If your instance / machine is based on **GPU**. Please press y to install nvidia cuda driver.
If your instance / machine is based on **CPU**. Please press n to continue to install BioColab.

Do you have a GPU on your machine: [y/n] **n** ( I used n as my machine does not support GPU ). Kindly select **Y** if your machine is having GPU support.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/gn.png" class="lazy" width="100%"><br> 

==OR==

Do you have a GPU on your machine: [y/n] **y** (in case you have GPU supported instance and would like to install driver)
– It will download the driver and install it.
– Type accept to move to the next step.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/26.png" class="lazy" width="100%"><br>


Use the down arrow key to reach **install** option and press enter to start cuda driver installation.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/27.png" class="lazy" width="100%"><br>

Wait for a while to complete execution to install nvidia driver.

**7]** Do you need install NVIDIA Docker 2 **[y, n**]:
Please press **y** if you wish to install Nvidia docker2.

 
**8]** Would you like to change IP:
We can simply press Enter or n. If we do not want to change IP.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/ci.png" class="lazy" width="100%"><br>

:bell: Note: The BioTuring team will share the latest image **tag** during installation or prior to starting installation.


**9]** Please enter Biocolab's Proxy **1.0.26** (latest):
We can press enter as it is the latest version.


<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/pver.png" class="lazy" width="100%"><br>

**10]** Install NFS server **[y, n]**:
We can simply press Enter or n. If we do not want to install NFS.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/nfs.png" class="lazy" width="100%"><br>

Wait for a while to download the Bioproxy image and start the container.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/bstart.png" class="lazy" width="100%"><br>

**11]** BioColab version installation **2.0.50** (latest):
We can press enter as it is the latest version.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/bcv.png" class="lazy" width="100%"><br>

Wait for a while to download the BioColab image and start the container.

**12]** check the status:

```R
docker ps -a
```
 
Both containers are UP and running.

<br><img alt="email-t" src="https://cdn.bioturing.com/documentation/emailtemp-pic/brn.png" class="lazy" width="100%"><br>

Once both containers are up and running successfully.

Installation has been completed.

I’d be more than happy to schedule a quick call and start BioStudio installation.  We only need approx. 30 minutes to complete these installation steps. Feel free to let us know what could be a good time to schedule a call.

If you have any questions or require any additional information or support, please don't hesitate to contact us at any point.

For more information or support, please contact us at support@bioturing.com.