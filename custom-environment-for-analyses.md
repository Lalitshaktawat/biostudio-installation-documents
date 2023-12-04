# <p> <span style="color:blue"> Introduction: </span> <span style="color:green"> Custom environment set up in BioStudio </span> </p>


# Conda Environment Manager

**BioStudio** is currently utilizing **conda manager**. **Conda** is an open-source package management system and environment management system. A **conda environment** is a directory that contains a specific collection of **conda packages** that you have installed.

**To access this features:**

:high_brightness: Click on **Package Environments** icon on the left side menu. 

-- **OR** --

:high_brightness: **Menu Icon** located at right side on the menu bar.

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/pkr.png" class="lazy" width="100%">

-- **OR** --

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/ccen12.png" class="lazy" width="100%"><br>
 
**Conda environments** utilities can be used based on requirement.

<br>
<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/ccrn.png" class="lazy" width="100%">

## Create new environment

You can create a new Conda environment with pre-installed language by clicking on the **Create New** button.

:one: Enter the environment name in the input field.
:two: Select the required language with the version that you would like to have in the new environment.
:three: Click on **OK** button to process next step. <br>

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cne.png" class="lazy" width="100%">
<br><br>

The terminal will automatically open on the right side with an activated environment. It's up to the client to use this activated environment.

:high_brightness: We can close this terminal by clicking **Close** button.

<br>
<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cnea.png" class="lazy" width="100%">
<br>

## Refresh environment list

:high_brightness: Click on **Refresh** icon to update environment list.

<br>
<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cner.png" class="lazy" width="100%"><br><br>


In order to open a new terminal, activate a specific environment from the list.

:high_brightness: Click on **Terminal** icon.

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/enva.png" class="lazy" width="100%">

<br>

## Clone environment

We can create the **similar environment** from **existing environment** by clicking on **Clone** icon.

:one: Enter the new environment name.
:two: Click On **OK** button.

<br>

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/envcl.png" class="lazy" width="100%"><br><br>

It will appear on the **list** as below.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/envcll.png" class="lazy" width="100%"><br>

## Import environment from YAML file

We can create an environment from a **YAML file** by clicking on the **Import** button.
:one: Enter the new environment.
:two: Upload **YAML** file from local machine.
:three: Click on **OK** button.
  
<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/im.png" class="lazy" width="100%">

## Export environment to YAML file

We can export the environment to a **YAML file** that can be downloaded to your local.

:one: Select the environment that you would like to export from dropdown list.
:two: Click on **Export** Button.
:three: Once it is finished, it will automatically download **YAML** file to your local machine. In case not downloaded, click on **Download YAML** link.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/ceed.png" class="lazy" width="100%"><br>


## Export environment to YAML file

:high_brightness: Environment can be deleted by clicking **Delete Environment** button. 
:high_brightness: Click **OK** in the popup to confirm your action.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/delen.png" class="lazy" width="100%"><br><br>

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cde.png" class="lazy" width="100%"><br>

# Install/Uninstall packages

You can install  packages to selected environment from available package on Explore / Repositories.

- You can choose environment to install/uninstall packages.

<img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/ccpp.png" class="lazy" width="60%"><br>


## Find and install packages

You can find and install packages to the selected environment.

:one: Select the environment.
:two: Click on **Explore** Tab.
:three: Type the **package name** in the **search field** and press **Enter**. It will show all the packages for the same name from different channels.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/pan.png" class="lazy" width="100%"><br>

:four: After you get the search results, click the intended package to open it in a new tab. This allows you to view the package details and choose the version to install. 
:five: click on **Install**. Click OK in the popup to confirm your action.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/panda1.png" class="lazy" width="100%"><br><br>

Installed packages would be listed on **Installed** tab. You can uninstall or update it later.

## Update packages

You can update existing conda packages in the environment.
:one: Select the environment.
:two: Switch to  **Installed** tab. Search packages you want to update, then click on it to go to detail tab, select specific version that you would like to update.
:three: Click OK in the popup to confirm your action.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/pup.png" class="lazy" width="100%"><br>

## Uninstall packages

You can uninstall conda packages in the environment.
:one: Select the environment.
:two: Switch to  **Installed** tab. Search packages you want to uninstall, then click on **Uninstall** icon.
:three: Click OK in the popup to confirm your action.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/panda2.png" class="lazy" width="100%"><br>


## Install packages from Git repository

For packages from **github** repository, you can install it by following steps:

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/adn.png" class="lazy" width="100%"><br>

:one: Select the environment.
:two: Go to **Repositories** tab, Click to button **Add New Repository**.
:three: Enter Git repository URL, select package language and click on **Check** button.
:high_brightness: It will prompt for branch. By default it will be main branch. You can switch to another branch that you would like install.
:high_brightness: Click on **Install**. Click OK in the popup to confirm your action.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/addr.png" class="lazy" width="100%"><br>

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/sb.png" class="lazy" width="100%"><br>

# Notebook Kernel Manager

**Kernels:** are specific instances of a programming environment that BioStudio uses to execute code in a notebook. Each kernel corresponds to a particular environment. This means that you can have multiple kernels running concurrently, each associated with a different environment.

You can create with empty notebook or connect existing noteboook with pre-build kernels:

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/kk1.png" class="lazy" width="100%"><br>

You  can also create custom kernel based on your requirements.

## Create notebook kernel

:high_brightness: You can create kernel by clicking **Kernel** Icon.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/k.png" class="lazy" width="100%"><br>

Then, the popup will appear, which have four options:
```R
1. Basic
2. From Env (From existing environment)
3. From File
4. From BioTuring
```

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cn.png" class="lazy" width="100%"><br>

## Basic Mode

:one: Enter the kernel name.
:two: Choose A Mode: **Basic**. In this mode, it will create a general environment and kernel. All basic package will be attached with this Kernel.
:three: Select specific language in language field. Currently, BioStudio is supporting two languages: **Python** and **R**.
:four: Select version based on selected language. If pre-define versions are not suitable for your requirements, you can type the version that you would like to install, and then, click **Add Customize** button to apply.
:five: Click **Create** button.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/ck.png" class="lazy" width="100%"><br>

Once Kernel creation finished, It is also available **Recent Activity popup**. That can be view by clicking **Notification** icon (Top right bell icon).

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/rac.png" class="lazy" width="100%"><br><br>

You can view the log to tracking the status.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/rac-d.png" class="lazy" width="100%"><br>


## From Env Mode

:one: Enter the kernel name.
:two: Choose A Mode: **From Env**. In this mode, create kernel using existing environment.
:three: Select specific existing environment in environment field.
:four: Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
:five: Select version based on selected language.

:bell: Existing environment includes **Python package** and **R package** already. So the version field will be **disabled** and not allowed to be changed. But if you select a different language package that is not in the existing environment, then you are allowed to select the version. If pre-defined versions are not suitable for your requirements, you can type the version you would like to install, and then click the **Add Customize** button to apply.

:high_brightness: Click **Create** button

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/kff.png" class="lazy" width="100%"><br>

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cnkc.png" class="lazy" width="100%"><br>

## From File

:one: Enter the kernel name
:two:Choose A Mode: **From File**. 
**From File Mode** first create an environment that would be from YAML file then it will install language that was selected during creation.
:three: Upload environmental file by clicking **Browse** button.
:four: Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
:five: Select version based on selected language.

If pre-define versions is not suitable for your requirement, you can type version you would like to install, and then, click **Add Customize** button to apply.

:high_brightness: Click **Create** button.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/kffl.png" class="lazy" width="100%"><br>

## From BioTuring

:one: Enter the kernel name
:two: Choose A Mode: **From BioTuring**. 

**From BioTuring**  option is similar to From File. But environment will be uploaded form BioTuring cloud. It is requested environmental package from client.

:three: Select your request environment from Your Request Environment. If you have nothing and would like to request something, you can click on **Send us a request** to request that BioTuring's DataScience Team help you prepare your environment.
 
<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/prq.png" class="lazy" width="100%"><br>

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/kfbb.png" class="lazy" width="100%"><br>

:high_brightness: You can **download** or **edit** YAML file.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/biot.png" class="lazy" width="100%"><br>

:four: Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
:five: Select version based on selected language.

:bell: Existing environment includes **Python package** and **R package** already. So the version field will be **disabled** and not allowed to be changed. But if you select a different language package that is not in the existing environment, then you are allowed to select the version. If pre-defined versions are not suitable for your requirements, you can type the version you would like to install, and then click the **Add Customize** button to apply.

:six: Click **Create** button.
   
<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/cnk.png" class="lazy" width="100%"><br>

# KernelSpec Manager

:high_brightness: Open kernel manager by clicking **Kernel Manager** in **Create Notebook Kernel** Popup.

-- **OR** --

:high_brightness: clicking on **KernelSpec Manager** icon in **Quick Start Launcher**.


<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/km.png" class="lazy" width="100%"><br>

**KernelSpec Manager** help you edit kernel specification like display name and some advance parameters. It includes: 

:high_brightness: **User Kernels** : List of the Kernels, which were created by user. User can edit and remove these kernel.

:high_brightness: **System Kernels** : BioStudio pre-defines kernels. Which can be used to run a notebook. Users are not allowed to edit or remove these kernels, but they can be copied to user kernels.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/km23.png" class="lazy" width="100%"><br>

You can edit Kernel **Launcher Arguments** or **add some environment variables** as per your requirement.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/km24.png" class="lazy" width="100%"><br>

# Connect notebook with kernel

While run the notebook you can select Kernel by clicking switch kernel button.

:high_brightness: Select Kernel popup will appear. 

:high_brightness: Select the kernel to which you would like to connect. If the kernel had a previous session, Then you will have two options.

:high_brightness: **Create a new session**: Kernel will start from the beginning and does not have any old values for variables.

:high_brightness: **Current session**:  In this option, The notebook will run on the existing kernel and have all the available variables from the previous session.

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/nbkn.png" class="lazy" width="100%"><br>

<br><img alt="BioStudio-env" src="https://cdn.bioturing.com/documentation/pic/slk.png" class="lazy" width="100%"><br>
