# Set up a custom environment for analyses in BioStudio

# Conda Environment Manager

**BioStudio** currently using **conda manager**. **Conda** is an open-source package management system and environment management system. A **conda environment** is a directory that contains a specific collection of **conda packages** that you have installed.

To access this features,  Click on **Package Environments** icon on left side menu  or **Menu Icon** located at right side on the menu bar.

<img alt="BioStudio-env" src="./pic/pkr.png" class="lazy" width="100%">

-- **OR** --

<img alt="BioStudio-env" src="./pic/ccen12.png" class="lazy" width="100%">


 **Conda environments** utilities can be used based on requirement.

<img alt="BioStudio-env" src="./pic/ccrn.png" class="lazy" width="100%">

## Create new environment

You can create new conda environment with pre-installed language by clicking on **Create New** button

1. Enter environment name in the input field.
2. Select require language with version that you would like to have in  new  environment.
3. Click on **OK** button to process next step.

<img alt="BioStudio-env" src="./pic/cne.png" class="lazy" width="100%">

Terminal will automatic open on right side and with activated environment. It's up to client to use this activated environment.

We can close this terminal by clicking **Close** button.

<img alt="BioStudio-env" src="./pic/cnea.png" class="lazy" width="100%">

## Refresh environment list

  Click on **Refresh** icon to update environment list.


<img alt="BioStudio-env" src="./pic/cner.png" class="lazy" width="100%">

In order to open new terminal with activate specific environment from the list. Click on **Terminal** icon.

<img alt="BioStudio-env" src="./pic/enva.png" class="lazy" width="100%">

## Clone environment

We can create the similar environment from existing environment by clicking on **Clone** icon.
   1. Enter the new environment name
   2. Click On **OK** button

<img alt="BioStudio-env" src="./pic/envcl.png" class="lazy" width="100%">

<img alt="BioStudio-env" src="./pic/envcll.png" class="lazy" width="100%">

## Import environment from YAML file

We can create environment from **YAML file** by clicking on **Import** button.
1. Enter the new environment
2. Upload **YAML** file from local machine
3. Click on **OK** button
  
<img alt="BioStudio-env" src="./pic/im.png" class="lazy" width="100%">

## Export environment to YAML file
We can export environment to **YAML file**  and you can download it on your local
   1. Select the enviroment which you would like to export from dropdown menu
   2. Click on Export Button 
   3. Once it finished, it will automatically download yaml file to your local machine. In case not downloaded, click on **Download YAML** link

<img alt="BioStudio-env" src="./pic/ceed.png" class="lazy" width="100%">


## Export environment to YAML file
Environment can be deleted by clicking **Delete Environment** button. Click OK in the popup to confirm your action.

<img alt="BioStudio-env" src="./pic/delen.png" class="lazy" width="100%">

<img alt="BioStudio-env" src="./pic/cde.png" class="lazy" width="100%">

# Install/Uninstall packages

You can install  packages to selected environment from available package on Explore / Repositories.

- You can choose environment to install/uninstall packages.

<img alt="BioStudio-env" src="./pic/ccpp.png" class="lazy" width="60%">


## Find and install packages
You can find and install packages to the selected environment.

1. Select the environment
2. Click on Explore Tab
3. Type the package name in the search field and press **Enter**. It will show all package for the same name from different channels.

<img alt="BioStudio-env" src="./pic/pan.png" class="lazy" width="100%">

4. After you get the search results, click the intended package to open it on new tab. This allows you to view the package details and choose the version to install. Then, click on  **Install**. Click OK in the popup to confirm your action.

<img alt="BioStudio-env" src="./pic/panda1.png" class="lazy" width="100%">

Installed packages would be listed on **Installed** tab. You can uninstall or update it later.

## Update packages

You can update existing conda packages in the environment
1. Select the environment
2. Switch to  **Installed** tab. Search packages you want to update, then click on it to go to detail tab, select specific version that you would like to update.
3. Click OK in the popup to confirm your action.


<img alt="BioStudio-env" src="./pic/pup.png" class="lazy" width="100%">

## Uninstall packages

You can uninstall conda packages in the environment
1. Select the environment
2. Switch to  **Installed** tab. Search packages you want to uninstall, then click on **Uninstall** icon.
3. Click OK in the popup to confirm your action.

<img alt="BioStudio-env" src="./pic/panda2.png" class="lazy" width="100%">


## Install packages from Git repository

For packages from github repository, you can install it by following these steps:

<img alt="BioStudio-env" src="./pic/adn.png" class="lazy" width="100%">

1. Select the environment
2. Go to **Repositories** tab, Click to button **Add New Repository**
3. Enter Git repository URL, select package language and click on **Check** button.
4. It will prompt for branch. By default it will be main branch. You can switch to another branch that you would like install.
5. Click on **Install**. Click OK in the popup to confirm your action.

<img alt="BioStudio-env" src="./pic/addr.png" class="lazy" width="100%">

<img alt="BioStudio-env" src="./pic/sb.png" class="lazy" width="100%">

# Notebook Kernel Manager

**Kernels:** are specific instances of a programming environment that BioStudio uses to execute code in a notebook. Each kernel corresponds to a particular environment. This means that you can have multiple kernels running concurrently, each associated with a different environment.

You can create with empty notebook or connect existing noteboook with pre-build kernels:

<img alt="BioStudio-env" src="./pic/kk1.png" class="lazy" width="100%">

You  can also create custom kernel based on your requirements.

## Create notebook kernel

You can create kernel by clicking **Kernel** Icon.
<img alt="BioStudio-env" src="./pic/k.png" class="lazy" width="100%">

Then, the popup will appear, which have four options:
- Basic
- From Env (From existing environment)
- From File
- From BioTuring

<img alt="BioStudio-env" src="./pic/cn.png" class="lazy" width="100%">

## Basic Mode
1. Enter the kernel name
2. Choose A Mode: **Basic**. In this mode, it will create general environment and kernel. All basic package will be attached with this Kernel.
3. Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
4. Select version based on selected language. If pre-define versions is not suitable for your requirement, you can type version you would like to install, and then, click **Add Customize** button to apply.
5. Click **Create** button

<img alt="BioStudio-env" src="./pic/ck.png" class="lazy" width="100%">

Once Kernel creation finished, It is also available **Recent Activity popup**. That can be view by clicking **Notification** icon (Top right bell icon).

<img alt="BioStudio-env" src="./pic/rac.png" class="lazy" width="100%">

You can view the log to tracking the status.

<img alt="BioStudio-env" src="./pic/rac-d.png" class="lazy" width="100%">


## From Env Mode


1. Enter the kernel name
2. Choose A Mode: **From Env**. In this mode, create kernel using existing environment.
3. Select specific existing environment in environment field.
4. Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
5. Select version based on selected language.
   Existing environment included Python package / R package already. So Version field will be disabled and not allowed to change. But if you will select different language package, which is not in existing environment then you are allow to select version. If pre-define versions is not suitable for your requirement, you can type version you would like to install, and then, click **Add Customize** button to apply.
6. Click **Create** button


<img alt="BioStudio-env" src="./pic/kff.png" class="lazy" width="100%">


<img alt="BioStudio-env" src="./pic/cnkc.png" class="lazy" width="100%">

## From File

1. Enter the kernel name
2. Choose A Mode: **From File**. 
   **From File Mode** first create an environment that would be from YAML file then it will install language that was selected during creation.
3. Upload environmental file by clicking **Browse** button.
4. Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
5. Select version based on selected language.
   If pre-define versions is not suitable for your requirement, you can type version you would like to install, and then, click **Add Customize** button to apply.
6. Click **Create** button

<img alt="BioStudio-env" src="./pic/kffl.png" class="lazy" width="100%">


## From BioTuring

1. Enter the kernel name
2. Choose A Mode: **From BioTuring**. 
   **From BioTuring**  option is similar to From File. But environment will be uploaded form BioTuring cloud. It is requested environmental package from client..
3. Select your request environment from Your request Environment. If you have no one, - You click on **Send us a request** to request BioTuring's DataScience Team  help you prepare your environment.
 
<img alt="BioStudio-env" src="./pic/prq.png" class="lazy" width="100%">

<img alt="BioStudio-env" src="./pic/kfbb.png" class="lazy" width="100%">

You can download or edit YAML file

<img alt="BioStudio-env" src="./pic/biot.png" class="lazy" width="100%">

4. Select specific language in language field. Currently, BioStudio is only supporting two languages: **Python** and **R**.
5. Select version based on selected language.
  Existing YAML file included Python package / R package already. So Version field will be disabled and not allowed to change. But if you will select different language package, which is not in existing YAML file then you are allow to select version. If pre-define versions is not suitable for your requirement, you can type version you would like to install, and then, click **Add Customize** button to apply.
6. Click **Create** button
   
<img alt="BioStudio-env" src="./pic/cnk.png" class="lazy" width="100%">




# KernelSpec Manager

Open kernel manager by clicking **Kernel Manager** in **Create Notebook Kernel** Popup or clicking on **KernelSpec Manager** icon in **Quick Start Launcher**.


<img alt="BioStudio-env" src="./pic/km.png" class="lazy" width="100%">

**KernelSpec Manager** help you edit kernel specification like display name and some advance parameters. It includes: 

- **User Kernels** : List of the Kernels, which were created by user. User can edit and remove these kernel.

- **System Kernels** : BioStudio pre-define kernels. Which can be used to run notebook.  User are not allowed to edit and remove these kernel, but can copy this kernel to user kernels.


<img alt="BioStudio-env" src="./pic/km23.png" class="lazy" width="100%">

You can edit Kernel **Launcher Arguments** or **add some environment variables** as per your requirement.


<img alt="BioStudio-env" src="./pic/km24.png" class="lazy" width="100%">



# Connect notebook with kernel

While run the notebook you can select Kernel by clicking switch kernel button.

Select Kernel popup will appear. 

Select the Kernel as you would like to connect. If the Kernel had a previous section. Then you will have two options. 

- **Create a new section**: Kernel will start from beginning and does not have any old values of variables.
- **Current section**:  In this option. Notebook will run on existing Kernel and can have the all available variables from previous section.

<img alt="BioStudio-env" src="./pic/nbkn.png" class="lazy" width="100%">

<img alt="BioStudio-env" src="./pic/slk.png" class="lazy" width="100%">