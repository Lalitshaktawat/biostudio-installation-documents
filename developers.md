# **Workspace interface**

BioStudio workspace is a collection of powerful tools and applications designed to assist scientists with their data manipulations.

The workspace interface consists of a main work area that lists all of the tools and applications available in BioStudio, a menu bar located at the top of workspace, a collapsible left sidebar, and a right sidebar.

<img alt="workspace" src="https://cdn.bioturing.com/documentation/md/getting_workspace.png" class="lazy" width="100%">

## **Main work area**

The main work area displays a comprehensive list of tools and applications that are accessible in BioStudio:

- **Most Used**: the applications that have been used frequently or most recently.
- **Languages**: all programming languages supported in BioStudio including Python, Go, Julia, Octave, R, Rust, Scala, etc.
- **Applications**: open-source applications integrated into BioStudio for enhanced functionality such as Terminal, File Browsers, Notebook Jobs, Shiny Server, and VScode.
- **Utilities**: all file formats supported in BioStudio including Diagram, Text file, Markdown file, CSV file, Julia file, Python file, R file, TSV file, etc.
- **Kernels**: all kernels created in your BioStudio account.

## **Top Menu bar**

The top menu bar located at the top of the BioStudio workspace interface features a set of top-level menus that provide access to various actions and functions. The default menus are as follows:

- **File**: actions related to files and directories
- **Edit**: actions related to editing documents and other activities
- **View**: actions that alter the appearance of BioStudio worspace
- **Run**: actions for running code in different activities such as notebooks and code consoles
- **Kernel**: actions for managing kernels, which are separate processes for running code
- **Git**: actions for working with Git
- **Diagram**: actions for working with Diagram files
- **Settings**: common settings and an advanced settings editor.

In addition to the default menus on the left sidebar, BioStudio workspace also provides some functional buttons on the right of the top menu bar, including:

- **Kernel**: enables users to create a new kernel.

<img alt="kernel" src="https://cdn.bioturing.com/documentation/md/dev_kernel.png" class="lazy" width="100%">
</br>
</br>

- **Notebook**: supports users in keeping track of all public notebooks in the BioStudio workspace.

<img alt="notebook" src="https://cdn.bioturing.com/documentation/md/dev_notebook.png" class="lazy" width="100%">
</br>
</br>

- **Notification**: displays all working statuses.
- **Your avatar**: allows users to manage their account and relevant settings.

## **Left sidebar**

The left sidebar contains several commonly-used tabs which are:

- **A file browser**: allows users to manage files and directories within their workspace.

<img alt="file" src="https://cdn.bioturing.com/documentation/md/dev_file.png" class="lazy" width="100%">
</br>
</br>

- **HDF Browser**: provides easy access to HDF format files.

<img alt="HDF" src="https://cdn.bioturing.com/documentation/md/dev_hdf.png" class="lazy" width="100%">
</br>
</br>

- **Table of contents**: shows the structure of a document and allows users to navigate to specific sections by clicking on entries in the sidebar. It is automatically generated when working with notebooks, markdown, or python files and each listed section will be hyperlinked to the actual section within your document.
  </br>

  Automatic section numbering feature is designed to number your notebook's sections and subsections based on your headings. This means that if you move any major sections around multiple times, you do not need to manually renumber the document and its subsections.

<img alt="table of content" src="https://cdn.bioturing.com/documentation/md/dev_toc.png" class="lazy"  width="100%">
</br>
</br>

If a notebook section has runnable code cells, a context menu is added to the corresponding table of contents heading. Clicking the "Run Cell(s)" option in the top menu bar will execute those code cells in the notebook.

<img alt="table of content" src="https://cdn.bioturing.com/documentation/md/dev_toc2.png" class="lazy"  width="100%">

</br>
</br>

- **AI assistant**: provides support to users through artificial intelligence tools such as ChatGPT and BioTuring Sonia AI. This feature is disabled by default.

<img alt="left sidebar - AI assistant" src="https://cdn.bioturing.com/documentation/md/dev_ai.png" class="lazy" width="100%">

</br>
</br>

- **Running panel**: displays a list of all currently running kernels and applications across all notebooks, code consoles, and directories.

<img alt="left sidebar - Running panel" src="https://cdn.bioturing.com/documentation/md/dev_panel.png" class="lazy" width="100%">

</br>
</br>

- **Git**: provides actions for working with Git.

<img alt="left sidebar - Git" src="https://cdn.bioturing.com/documentation/md/dev_git.png" class="lazy" width="100%">

</br>
</br>

- **IPython parallel**: enables parallel and distributed computing by distributing tasks across multiple cores, processors, or computers.

<img alt="left sidebar - IPython parallel" src="https://cdn.bioturing.com/documentation/md/dev_python.png" class="lazy" width="100%">

## **Right sidebar**

The right sidebar contains the following commonly-used tabs:

- **The property inspector**: ​is active in notebooks and allows users to view and edit metadata for notebook cells.

<img alt="right sidebar - The property inspector" src="https://cdn.bioturing.com/documentation/md/dev_inspec.png" class="lazy" width="100%">

</br>
</br>

- **The debugger**: enables users to debug code consoles and files directly from the notebooks.

<img alt="right sidebar - The debugger" src="https://cdn.bioturing.com/documentation/md/dev_debug.png" class="lazy" width="100%">

# **Create notebook kernel**

To create a new notebook kernel in the BioStudio workspace, follow these steps:

- **Step 1**: Click on the 'Kernel' button located on the right side of the top menu bar.
- **Step 2**: Enter your desired kernel name.
- **Step 3**: Select one of the three available modes below.

**Basic**: allows you to choose a programming language and its version from a drop-down list.

<img alt="Create notebook kernel - basic" src="https://cdn.bioturing.com/documentation/md/dev_kernel_basic.png" class="lazy"  width="100%">

</br>
</br>

**From environment**: allows you to select a notebook environment that you've previously created, as well as the programming language you want to use.

<img alt="Create notebook kernel - from environment" src="https://cdn.bioturing.com/documentation/md/dev_kernel_env.png" class="lazy"  width="100%">
</br>
</br>

**From file**: requires you to upload a YAML file that specifies the packages to be installed in the environment. The YAML file should include the names and versions of the desired packages, as well as any necessary dependencies.

<img alt="Create notebook kernel - from file" src="https://cdn.bioturing.com/documentation/md/dev_kernel_file.png" class="lazy"  width="100%">

</br>
</br>

# **Manage Conda environment**

Users can conveniently manage all packages in their Conda environments by accessing the Conda package manager in the Settings tab located on the top menu bar.

Once you access the Conda package manager interface, you will see a list of all available environments on the left side and a list of all packages in the selected environment on the right side.

<img alt="Conda environment - main page" src="https://cdn.bioturing.com/documentation/md/dev_env_main.png" class="lazy"  width="100%">

## **The left side**

Within the left side, there are several actions that can be performed on the selected Conda environment:

**Create**: allows you to create a new Conda environment by selecting your desire programing language.

**Clone**: allows you to clone the selected environment into a new one.

**Import**: allows you to create a new Conda environment by importing a YAML file.

**Export**: allows you to export the selected environment in YAML format.

**Remove**: allows you to remove the selected environment.

## **The right side**

After selecting a specific environment in the left side, the right side will display all the available packages along with their detailed description, installed version, installation status, and channel information.

You can easily search for specific packages and also change the view modes to display all packages, installed packages, not installed packages, updatable packages, or selected packages.

<img alt="Conda environment - right sidebar1" src="https://cdn.bioturing.com/documentation/md/dev_env_packages1.png" class="lazy"  width="100%">
</br>
</br>

To install new packages, simply select the desired packages and their versions and click on the **Apply package modifications** button located above the table. Otherwise, the latest version of the package will be installed by defaut.

For installed packages, BioStudio allows users to update to a new version or remove the package by changing its installation status and clicking on the **Apply package modifications** button.

<img alt="Conda environment - right sidebar2" src="https://cdn.bioturing.com/documentation/md/dev_packages2.png" class="lazy"  width="100%">
</br>
</br>

For more information, please contact us at <a href="mailto:support@bioturing.com">support@bioturing.com</a>.
