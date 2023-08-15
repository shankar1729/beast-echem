---
layout: page
navtitle: Workshops
title: BEAST Workshop setup instructions
description: "Jupyter and environment setup instructions"
permalink: /workshops/2023/setup/
---

# Accessing and setting up Jupyter Lab environment on Perlmutter

## Set up your NERSC training account

If you have not already made your training account, please refer to the email instructions sent to you on 8/15/2023 or follow the instructions here:

1. Go to https://iris.nersc.gov/train
2. Fill out the form using e32Q as the Training Code
3. Immediately <b>note your username and password</b>. NERSC will NOT email this to you, so make sure you save this information off line.
4. Please enter your training account information into [this form](https://forms.gle/byv8CNSygzDqVSx19) (so that we know who is ready to attend)

Once you have noted your training account username and password, please proceed to the next section.
While the page indicates that the login will be available within 30 seconds, it seems to be taking 10-15 minutes to propagate to all systems.
So please wait 10 minutes before retrying if your login below fails.

## Access Perlmutter with Jupyter Lab

To access Perlmutter, please enter the following URL into your favorite browser: https://jupyter.nersc.gov/ and enter your training account username and password. Once you have logged in, you should see JupyterHub in the top left corner with options to start kernels on Perlmutter on CPUs and GPUs. 

![Perlmutter Jupyter log-in page](perl-jupyter-login.png)

Please start a kernel on the Perlmutter shared CPU nodes by clicking on the button. 

Now you should see a user interface with a file navigator on the left and new file selection screen on the right.

![Perlmutter Jupyter Hub home](perl-jupyterhub-home.png)

See [these slides from a previous NERSC workshop](https://drive.google.com/file/d/1JXbzoP3OQH7qMJ5n4pxwYLgpzC0ittH9/view) for more detailed instructions to familiarize yourself with the Jupyter environment,

## Optional: adjust settings to open Markdown in preview

Let's adjust settings to view documentation more easily. 
Click Settings -> Advanced Settings Editor and select Document Manager.
![Settings Document Manager](settings-document-manager.png)

Scroll down to the bottom of that section, click Add,
and set markdown files to be viewed with Markdown Preview:
![Settings Document Manager](settings-add-markdown-preview.png)


## Prepare your environment

Click on $HOME in the upper left corner, which will bring your file browser in the lower left corner to your home directory.

Select `View -> Show Hidden Files` on the menu, which will reveal a number of new files starting with `.` in the file browser.

Open `.bashrc.ext` by double-clicking on it from the file browser.
Copy the following lines to it (under where it says `User additions to .bashrc go in this file`):

    module use /global/cfs/cdirs/m4025/Software/Perlmutter/modules
    module load beast-tutorial
    python -m ipykernel install --user --name beast_pyenv --display-name "BEAST Python"
    alias ls="ls --color"
    alias sq="squeue -u $USER"
    export PS1="\[\033[01;32m\]\u@\h\[\033[00m\](\[\033[01;31m\]\t\[\033[00m\]):\[\033[01;34m\]\w\[\033[00m\]\$ "

and then save (`Ctrl+S`) and close this file.
This will make sure that every terminal you open will load a module that puts all the required codes in your PATH.
It will also make the output of `ls` colorful, define `sq` to view only the jobs you launched within `squeue`,
and change your terminal prompt to be more colorful and informative.

You can now unselect `View -> Show Hidden Files` on the menu, so as to reduce clutter in the file browser.


## Copy the tutorials

Click on $PSCRATCH in the upper left corner. This is a hyperlink to your scratch directory. This is the directory where you should copy tutorials to and run them.

Next, look at the Launcher window to right and click on "Terminal" (under the "Other" header) to open a new terminal in your scratch directory. If you ever forget the path to this directory you can hover your cursor over the $PSCRATCH hyperlink in the top right to get it.

Within the terminal, run the following commands to **copy the tutorials** into your scratch:

```bash
cd $PSCRATCH
cp -a /global/cfs/cdirs/m4025/BEAST_TUTORIAL-23/Calculations-clean/ .
```

Also click $PSCRATCH on the top left again if your file browser is not in the same path.

You should see `Calculations-clean` within your file browser now.
Double click on it to view the tutorial files (including these instructions in `SETUP.md`).

Open the top-level README.md file by double-clicking on it. It should open in Markdown Preview with the settings change above,
(If you did not change the settings, it will open in edit mode by default, and you can right-click the Markdown file and select "Show Markdown Preview".)

Any .ipynb files (Jupyter notebook files with Python code) can be opened in a new tab by double-clicking on them in your file tree to the left. Each code block can be run by clicking inside the code block and typing "Shift + Enter".

**Important**: remember to work only within the copy of the tutorials within your $PSCRATCH directory made above.
Trying to work directly in the source directory will lead to permissions errors!
