# **Architecture Diagram**

## **Overview**

<br/>

The BioStudio architecture diagram provides a comprehensive overview of the system's components and their relationships. It illustrates how different services and systems interact with each other and with all other services in detail.

## **On private server / K8S**

<br/>

### 1. Preparing the platform setup

<br/>

**Our product consists of containerized applications that can be deployed on Docker using the Docker engine (docker, containerd) as well as on Kubernetes.**

To install BioStudio on your private server, the following requirements must be met:

#### System requirements

| <div style="text-align: center">OS system</div> | <div style="text-align: center">Version</div>      |
| :---------------------------------------------- | :------------------------------------------------- |
| Centos                                          | 6.5 or above recommended - https://www.centos.org/ |
| Readhat                                         | Any - https://www.redhat.com/en                    |
| Debian                                          | 10 or above recommended - https://www.debian.org/  |
| Ubuntu                                          | 18.04 or above recommended - https://ubuntu.com/   |

#### Hardware requirements

| <div style="text-align: center">Hardware</div> | <div style="text-align: center">Size</div>   |
| :--------------------------------------------- | :------------------------------------------- |
| CPUs                                           | 16 cores or above recommended                |
| GPUs                                           | <strong style="color:red;">Optional</strong> |
| MEMORY                                         | <strong style="color:red;">64GB</strong> or above recommended                   |
| APP-STORAGE                                    | 100GB or above recommended                    |
| METADATA-STORAGE                               | 50GB or above recommended                    |
| USER-STORAGE                                   | 500GB or above recommended                   |
| SSL-STORAGE                 | 1GB or above recommended |
| RUNTIME-ENGINE                                 | Docker/Containerd, or Kubernetes             |

#### Network requirements

Access to these domains is required for the machine with the BioStudio software installed, as we need to retrieve data from the BioTuring ecosystem server.

| <div style="text-align: center">Domain</div> | <div style="text-align: center">Explain</div>                      |
| :------------------------------------------- | :----------------------------------------------------------------- |
| \*.bioturing.com                             | We need to retrieve data from the BioTuring ecosystem server.      |
| \*.anaconda.org                              | We need to retrieve packages from the Anaconda server.             |
| \*repo.anaconda.com                          | We need to retrieve packages from the Anaconda repo server.        |
| Amazon S3                                    | We need to retrieve resources from the BioTuring ecosystem server. |
| `github.com`                                    | We need to retrieve packages from the Github. |

#### Application services

| <div style="text-align: center">Service</div> | <div style="text-align: center">Explain</div>                                                                                                                                                                                                                              |
| :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| bioproxy                                      | Within this image, you will find a comprehensive set of features, such as an HTTP/HTTPS server with load balancing, an NFS server, and Minio S3, in addition to metadata databases like PostgreSQL, Redis, and Memcached, all of which are used by the BioStudio instance. |
| BioStudio                                     | You will have access to all the necessary features, such as workspaces, notebooks, and various software applications that your colleagues use, through this image.                                                                                                         |

#### Service ports

| <div style="text-align: center">Service</div> | <div style="text-align: center">Exposed Port</div>                                                                                                                                                                                                                                                                                                 |
| :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| bioproxy                                      | <strong style="color:red;">HTTP (80)</strong> - We can change the this port. You may share this setting with your colleagues: http://your_private_server_ip_or_domain:<strong style="color:red;">PORT</strong>. This setting will enable your colleagues to access BioStudio private server through either a web browser or desktop application.   |
| bioproxy                                      | <strong style="color:red;">HTTPS (443)</strong> - We can change the this port. You may share this setting with your colleagues: http://your_private_server_ip_or_domain:<strong style="color:red;">PORT</strong>. This setting will enable your colleagues to access BioStudio private server through either a web browser or desktop application. |
| bioproxy                                      | MEMCACHED (11121) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                                 |
| bioproxy                                      | REDIS (6379) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                                      |
| bioproxy                                      | POSTGRESQL (5432) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                                 |
|                                               |                                                                                                                                                                                                                                                                                                                                                    |
| BioStudio                                     | <strong style="color:red;">WORKSPACE (18000) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.</strong>                                                                                                                                                                                             |
| BioStudio                                     | <strong style="color:red;">APP (11123) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.</strong>                                                                                                                                                                                                   |
| BioStudio                                     | MQTT-WEBSOCKET (9001) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                             |
| BioStudio                                     | MQTT-TCP (1883) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                                   |
| BioStudio                                     | JOB (11300) - This port is restricted to LAN networks and is used to connect between bioproxy and BioStudio.                                                                                                                                                                                                                                       |

### 2. Internal service workflow

<br/>

It is possible to install both the <strong style="color:red">bioproxy</strong> and <strong style="color:red">BioStudio</strong> Docker images on a single physical machine.

Using the machine that has the <strong style="color:red">BBrowserX private server</strong> installed can help you optimize your costs.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[Requests from IP/DNS] -->|Access| M(BioStudio container \n in \n Your private server \n or Your K8S)
    M -->|Access| B(BioStudio container \n in \n Your private server \n or Your K8S)
    B --> C{Business Logic}
    C -->|Licenses| D[*.bioturing.com]
    C -->|Notebooks| E[*.bioturing.com]
    C -->|Packages| F[*.bioturing.com \n *.anaconada.org \n *.anaconda.com \n Amazon S3 \n github.com]
    C -->|In-house Data| G[NFS \n S3 \n GlusterFS]
    C -->|Databases| H[PostgreSQL \n MySQL \n MariaDB]
    C -->|Ecosystem| J[BBrowserX \n Talk2Data]
```

</div>

### 3. Connection workflow

<br/>

Connection workflow refers to the sequence of steps or processes that are involved in establishing and managing connections between two or more systems, devices, or applications.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[Private server \n or Your K8S] -->|HTTPS| B(*.bioturing.com)
    B --> C{Services}
    C -->|Licenses| D[Check licence]
    C -->|Download| E[Curated notebooks]
    C -->|Download| F[Curated packages]
    C -->|Download| G[Curated data]
    C -->|Install| H[Biological APPs]
```

</div>

### 4. User access workflow

<br/>

```mermaid
flowchart TD
    A[Your colleagues] --> |HTTP/HTTPS/VPN| B{Access \n IP/Domain}
    B -->|Internet Browser| C[Your private server \n or Your K8S]
    B -->|Desktop APP| C[Your private server]
    C -->|Download| F[Curated notebooks] -->|HTTPS| L(*.bioturing.com)
    C -->|Install| H[Biological APPs] -->|HTTPS| L(*.bioturing.com)
    C -->|Download| M[Curated data] -->|HTTPS| L(*.bioturing.com)
    C -->|Access| G[Private workspace]
    C -->|Access| N[Private enviroment]
    C -->|Access| J[In-house data]
    C -->|Access| Z[In-house database]
    C -->|Access| W[BBrowserX private server]
```

### 5. Setup HTTPS workflow

<br/>

SSL Certificate : Software supports HTTPS protocol. SSL can be configured later after installation too.

After installing your private server, you can update your SSL by accessing the dashboard at `http://your private server ip or domain:port/dashboard` and selecting Settings > Update SSL.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[HTTPS Certificate] -->|IN| B(Your private server \n or Your K8S)
    B -->|Generate| D[Self-Signed SSL Certificate]
    B -->|Use| E[Let's Encrypt] --> K[Inside bioproxy \n Need public your domain]
    B -->|Buy| F[comodosslstore.com \n namecheap.com]
```

</div>

### 6. What is the process to activate your BioStudio private server?

<br/>

To activate the BioStudio private server, you need to have a token that is obtained from BioTuring.

After installing your private server, you can update your BioStudio token by accessing the dashboard at `http://your private server ip or domain:port/dashboard` and selecting Settings > Update BioStudio Token.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[Your private server \n or Your K8S] <-->|HTTPS| B(studio.bioturing.com)
    B <-->|Validate| D[Your TOKEN]
```

</div>
</br>

### 7. How can you utilize your company's SSO for accessing your BioStudio private server?

<br/>

BioStudio supports various SSO protocols including SAML, OAuth2, and OpenID, as well as popular social SSO options like AzureAD, Okta, Apple, Twitter, LinkedIn, Google, and Github.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[Your colleagues] <-->|LOGIN| B(Your private server \n or Your K8S )
    B <-->|Redirect| D[Your SSO IP/domain \n To enable SSO, you need to configure \n the SSO settings in \n the BioStudio admin dashboard.]
    B <-->|Redirect| F[portal.bioturing.com \n If you are unable to configure the SSO settings, \n you can use \n the BioTuring portal for authentication.]
```

</div>

### 8. What is the process for scaling in/out your BioStudio private server?

<br/>

Bioproxy and BioStudio (Docker images) can be installed on multiple machines. However, only one Bioproxy instance is needed to balance the load across all BioStudio instances.

<div style="display: flex; justify-content: center">

```mermaid
flowchart TD
    A[Private server \n or Your K8S] -->|Control| B(bioproxy)
    B <-->|Load balancing| D[BioStudio 1]
    B <-->|Load balancing| E[BioStudio 2]
    B <-->|Load balancing| F[BioStudio N]
    D --> |Add volumes| N[Volume 1...N]
    E --> |Add volumes| M[Volume 1...N]
    F --> |Add volumes| K[Volume 1...N]
```

</div>

## **On BioTuring cloud**

<br/>

It is the on-demand availability of computer system resources, especially data storage (cloud storage) and computing power, without direct active management by the user.

For any query and support. Kindly contact us: [:email: support@bioturing.com](mailto:support@bioturing.com)
