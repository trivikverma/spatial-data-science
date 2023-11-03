# Comprehensive Installation

## 3) A comprehensive approach: the GDS Docker container (slightly more advanced and complicated installation)

If meet the following requirements, [Docker](https://www.docker.com/) is a stable alternative and works out of the box:

1. You have admin rights over your machine
1. You are running either Windows 10 Pro, macOS, or Linux distributions that are supported by Docker.

It provides a stable platform to run complex software setups like that required in this context. Docker is a containerisation technology that allows to run pre-packaged (containerised) software under controlled environments. Relying on Docker, the [`gds_env`](https://github.com/darribas/gds_env) project provides a containerised platform for Geographic/Urban Data Science.

This resource provides step-by-step descriptions on how to install and run Python from your own computer for all operating systems. See instructions below.

## <mark> **MacOS Installation** </mark>


If you want to install miniconda (recommended approach, go [here](../software_index.md).)

## 1. Installation

### Requirements

To be able to complete this guide, your machine will need to meet the following requirements:

1. A stable internet connection
2. ~10GB of space on your hard drive
3. MacOS version 10.13 or newer i.e. High Sierra, Mojave or Catalina. If you are unsure what version you are running click on the Apple icon in the top left of the screen and then **About this Mac**.
4. Mac hardware must be a 2010 model or newer

### Docker install steps

1. Go to the [dockerhub website](https://hub.docker.com/editions/community/docker-ce-desktop-mac/).
2. Select the version according to your Apple chip.

  ![Select Version](figs/chp1/Figure1.png)


3. After you have installed the program and started it, the whale icon will appear in your taskbar as follows:

![Whale Icon](figs/chp1/Figure4.png)


<br/>

You have successfully downloaded Docker!

### Using Docker

Now we have Docker installed we can use it to access Python and all the associated packages we need for the labs of this course.



**Note**: With this installation process, you will not be able to install other packages if you wish to experiment. However, this will be enough for the course.



### Installing the GDS environment

1. Access your terminal: **Launchpad** > **Other** > **Terminal**
2. In a fresh line in the terminal type the following to install the GDS environment container:

```shell
docker pull darribas/gds:6.1
```

![Docker Pull GDS](figs/chp1/Figure5.png)


<br/>

3. This should now prompt a long download process that looks a bit like this:

![Downloading](figs/chp1/Figure6.png)


Dont be alarmed if it seems to take a very long time.

<b>*IMPORTANT*</b>: <br/>
Make sure you are connected to the internet and it is a stable connection. This step involves the download of large amounts of data (~ 10GB) so it might take a while. However, it only needs to run once.


### Check success

You will know the process has completed successfully when each line says 'Pull complete' and the new line shows your machine name.

If everything has gone according to plan, you should see `darribas/gds:6.1` show up on your terminal when you type `docker image ls` (note in the image below there are other containers that are not required, do not worry if you don't have those or slightly different values on the ID and the "CREATED" columns, the important bit is having `darribas/gds:6.1` listed):

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

![Command](figs/chp1/Figure8.png)


## 2. Running Python

The following sections cover how to start a python session using the docker container image you just installed, use it, and shut it down when you are done.

(running-the-container)=
### Running the container

1. In the new terminal line type the following command to run the container: `docker run --rm -ti -p 8888:8888 -v ${PWD}:/home/jovyan/work darribas/gds:6.1`

![Commandline](figs/chp1/Figure7.png)


<br/>

You have now started a Python session.


<b>*IMPORTANT*</b>: <br/>
Please do NOT close the terminal window until you are finished in this Python session.


2. To access this session go to your chosen web browser (e.g. Safari/Chrome) and type: `localhost:8888` into the search bar

![Token](figs/chp1/Figure10_new.png)


3. The page that loads will prompt you for a password or a token. This can be found in the text in the terminal following the last command you ran (step 9). A long series of numbers and letters will be preceded by `?token=`. Copy this long series of characters and paste into the password box in your browser.

![Login](figs/chp1/Figure9.png)


<br/>

4. Now that you are in Jupyter Lab you can open up a Python 3 notebook

![Jupyter Lab](figs/chp1/Figure11.png)


<br/>

### Using Jupyter Notebook

- This notebook is where you will run your code. Each shaded box is called a kernel. To test this out you can type `print('test')` into one of these kernels. To run the code use the shortcut `Ctrl + Enter`.

![Notebook](figs/chp1/Figure12.png)


<br/>


<b>*IMPORTANT*</b>: <br/>
Make sure you save files you want to keep **ONLY** _within_ the `work` folder, as this will ensure they are saved on your machine.

Everything saved outside the `work` folder will be _destroyed_ as soon as you shut down the session.



- You can access other files on your machine through the `work` folder in the File Browser. From here you can navigate to your Documents and designated folder for this module. For example, see below (this will depend on where you have stored the lab notebooks/data/other material for this course)

![Navigation0](figs/chp1/Figure15a_new.png)

![Navigation1](figs/chp1/Figure15b.png)

![Navigation2](figs/chp1/Figure15c.png)


Here I am navigating to the folder that I have created for this module in my Documents. You can replace this with the pathway to the folder you create for this module.

<br/>

- You can save your notebook here using **File** > **Save notebook as**
![Saving Notebook](figs/chp1/Figure13_new.png)

<br/>

- And you can create new folders to organise your work
![Organisation](figs/chp1/Figure14_new.png)

<br/>

### Ending your session
- Once you have finished in your Jupyter session and have saved all your work, you can end the session from the terminal.

- Using `Ctrl + C` will prompt a `y/n` option. Either type `y` or `Ctrl + C` again to end the session.

- You can now safely shut the terminal window.

<br/>

Next time you go to run a Jupyter Notebook you will not need to repeat the whole process as you have already installed Docker and the GDS environment. Instead you can start from [Running the container](running-the-container) and carry on from there.

<br/>


***
<br/>

## <mark> **Linux Installation** </mark>

If you want to install miniconda (recommended approach, go [here](../software_index.md).)

## 1. Installation

### Requirements

To be able to complete this guide, your machine will need to meet the following requirements:

1. A stable internet connection
2. ~10GB of space on your hard drive
3. A Linux distribution supported by Docker. You can check available distributions for ready installation on [this page](https://hub.docker.com/search?q=&type=edition&offering=community&operating_system=linux).

**NOTE** If you are running a different distribution (e.g. Arch Linux), there is a good chance Docker _will_ work, but you will have to source your own instructions for installation. Once you have Docker up and running on your machine, you can move to [Installing the GDS container](installing-the-gds-container).

### Docker install steps

1. Select the page for your distribution from the [Docker Hub list of supported distributions](https://hub.docker.com/search?q=&type=edition&offering=community&operating_system=linux)

![Docker Distros](figs/chp2/docker_distros.png)

<br>

For this example, we will use Ubuntu.

2. Make sure that you meet the requirements to install Docker:

![Ubuntu](figs/chp2/ubuntu.png)

<br>

3. Follow the steps specified on the official install guide:

> [https://docs.docker.com/engine/install/ubuntu/](https://docs.docker.com/engine/install/ubuntu/)

Once you complete these steps successfully, you will have Docker ready to go on your computer!

(installing-the-gds-container)=
### Installing the GDS container

Once you have Docker installed and running on your machine, installing everything you need to run Python and associated libraries boils down to the following two steps:

1. Open your terminal app of choice (for example, Gnome Terminal)
2. Run the following command:

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

```shell
docker pull darribas/gds:6.1
```

![Terminal Pull](figs/chp2/terminal_pull.png)

<br>

You will know this has completed when each line says 'Pull complete'.

<b>IMPORTANT</b>: <br>
Make sure you are connected to the internet and it is a stable connection. This step involves the download of large amounts of data (ca. 10GB) so it might take a while. However, it only needs to be run once.


### Check success

If everything has gone according to plan, you should see `darribas/gds:6.1` show up on your terminal when you type `docker image ls` (note in the image below there are other containers that are not required, do not worry if you don't have those or slightly different values on the ID and the "CREATED" columns, the important bit is having `darribas/gds:6.1` listed):

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

![Docker Image](figs/chp2/docker_image_ls.png)

<br>

## 2. Running Python

The following sections cover how to start a python session using the docker container image you just installed, use it, and shut it down when you are done.

### Running the container

To start up Python through Docker, follow these steps:

1. In a new terminal line, type the following command to run the container and hit enter:

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

```shell
docker run --rm -ti -p 8888:8888 -v ${PWD}:/home/jovyan/work darribas/gds:6.1
```

![Docker Run](figs/chp2/docker_run.png)

<br>

You have now started a Python session.


<b>IMPORTANT</b>: <br>

Please do NOT close the terminal window until you are finished in this Python session

2. To access this session go to your chosen web browser (e.g. Firefox/Chrome) and type: `localhost:8888` into the search bar

<br>

![Browser Access](figs/chp1/Figure10.png)


3. The page that loads will prompt you for a password or a token. This can be found in the text in the terminal following the last command you ran. A long series of numbers and letters will be preceded by `?token=`. Copy this long series of characters and paste into the password box in your browser.

![Docker Token](figs/chp2/docker_token.png)


4. Now that you are in Jupyter Lab you can open up a Python 3 notebook

![Python Notebook](figs/chp1/Figure11.png)

<br>

### Using Jupyter Notebook

- This notebook is where you will run your code. Each shaded box is called a kernel. To test this out you can type `print('test')` into one of these kernels. To run the code use the shortcut `Ctrl + Enter`.

![Jupyter Notebook](figs/chp1/Figure12.png)


<br>

<b>IMPORTANT</b>: <br>

Make sure you save files you want to keep **ONLY** _within_ the `work` folder, as this will ensure they are saved on your machine.

Everything saved outside the `work` folder will be _destroyed_ as soon as you shut down the session.


- You can save your notebook using **File** > **Save notebook as**

![Saving notebook](figs/chp1/Figure13.png)

<br>

- You can create new folders to organise your work
![New Folders](figs/chp1/Figure14.png)

<br>

- And you can access other files on your machine through the 'work' folder in the File Browser. From here you can navigate to your Documents and designated folder for this module

![Saving 1](figs/chp1/Figure15a.png)

![Saving 2](figs/chp1/Figure15b.png)

![Saving 3](figs/chp1/Figure15c.png)

<br>

### Ending your session

- Once you have finished in your Jupyter session and have saved all your work, you can end the session from the terminal.

- Using `Ctrl + C` will prompt a `y/n` option. Either type `y` or `Ctrl + C` again to end the session.

- You can now safely shut the terminal window.

<br>

Next time you go to run a Jupyter Notebook you will not need to repeat the whole process as you have already installed Docker and the GDS environment. Instead you can start from [Running Python through Docker](running-the-container) and carry on from there.

<br/>


***
<br/>

## <mark> **Windows** </mark>

If you want to install miniconda (recommended approach, go [here](../software_index.md).)

## 1. Installation

### Requirements

To be able to complete this guide, your machine will need to meet the following requirements:

1. A stable internet connection
2. ~10GB of space on your hard drive
3. Microsoft Windows 10 Professional, Education, Enterprise 64-bit, or Windows 10 Home 64-bit with WSL 2. You can see the full requirements on the official [Docker for Windows page](https://docs.docker.com/docker-for-windows/install/).

### Docker install steps

Once you have everything required ready to go, the first step is to install the Docker Desktop App for Windows. Here are the steps you can follow:

1. Head over to [Docker Hub](https://hub.docker.com/editions/community/docker-ce-desktop-windows/) to download a copy of Docker for Windows:

![Docker Hub](figs/chp3/docker_hub.png)

2. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.

You can check if the process has completed successfully by following these steps:

1. Open PowelShell from the "Start Menu"

![Powershell](figs/chp3/powershell.png)

<br>

2. Check Docker is available by printing out the version you have installed:

```shell
docker --version
```
![Docker Version](figs/chp3/docker_version.png)

<br>

Note that you might have installed a slightly different version and that is totally okay. What you want to make sure is that it successfully prints out a version instead of a warning/error message (usually in red).

### Installing the GDS container

Once you have Docker installed and running on your machine, installing everything you need to run Python and associated libraries boils down to the following two steps:

1. Open PowerShell following the same steps as above (you can use the same window as before or a fresh new one).
2. Run (type and hit "Enter") the following command:

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

```shell
docker pull darribas/gds:6.1
```

![Pull GDS](figs/chp3/pull_gds.png)

<br>

You will know this has completed when each line says 'Pull complete'.

<b>IMPORTANT</b>: <br>

Make sure you are connected to the internet and it is a stable connection. This step involves the download of large amounts of data (ca. 10GB) so it might take a while. However, it only needs to run once.

### Check success

If everything has gone according to plan, you should see `darribas/gds:6.1` show up on your terminal when you type `docker image ls` (note in the image below there are other containers that are not required, do not worry if you don't have those or slightly different values on the ID and the "CREATED" columns, the important bit is having `darribas/gds:6.1` listed):

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

![Docker Success](figs/chp3/docker_success.png)

<br>

## 2. Running Python

The following sections cover how to start a python session using the docker container image you just installed, use it, and shut it down when you are done.

### Running the container

To start up Python through Docker, follow these steps:

1. In a new PowerShell window, type the following command to run the container and hit enter:

**NOTE**: please ignore the version showing in the screenshot, follow that in
the command below

```shell
docker run --rm -ti -p 8888:8888 -v ${PWD}:/home/jovyan/work darribas/gds:6.1
```

![DockerRun](figs/chp3/docker_run.png)


You have now started a Python session.



<b>*IMPORTANT*</b>: <br>

Please do NOT close the PowerShell window until you are finished in this Python session


2. To access this session go to your chosen web browser (e.g. Firefox/Chrome) and type: `localhost:8888` into the search bar. You should see something similar to:

<br>

![Jupyter Token](figs/chp3/jupyter_token.png)

3. The page that loads will prompt you for a password or a token. This can be found in the text in the terminal following the last command you ran. This will be a long series of numbers and letters will be preceded by `?token=`. Copy this long series of characters and paste into the password box in your browser.

![Docker Token](figs/chp3/docker_token.png)


4. Now you are in Jupyter Lab, it should look like this, more or less:

![Jupyter Lab](figs/chp3/lab.png)

<br>

### Using Jupyter Notebook

- This notebook is where you will run your code. Each shaded box is called a kernel. To test this out you can type `print('test')` into one of these kernels. To run the code use the shortcut `Ctrl + Enter`.

![Using notebook](figs/chp1/Figure12.png)


<br>


<b>IMPORTANT</b>: <br>

Make sure you save files you want to keep **ONLY** _within_ the `work` folder, as this will ensure they are saved on your machine.

Everything saved outside the `work` folder will be _destroyed_ as soon as you shut down the session.

- You can save your notebook using **File** > **Save notebook as**
![Saving Notebook](figs/chp1/Figure13.png)

<br>

- You can create new folders to organise your work

![Organisation](figs/chp1/Figure14.png)

<br>

- And you can access other files on your machine through the 'work' folder in the File Browser. From here you can navigate to your Documents and designated folder for this module


![Navigation3](figs/chp1/Figure15a_new.png)

![Navigation4](figs/chp1/Figure15b.png)

![Navigation5](figs/chp1/Figure15c.png)
<br>

### Ending your session

- Once you have finished in your Jupyter session and have saved all your work, you can end the session from the terminal.

- Using `Ctrl + C` will prompt a `y/n` option. Either type `y` or `Ctrl + C` again to end the session.

- You can now safely shut the terminal window.

<br>

Next time you go to run a Jupyter Notebook you will not need to repeat the whole process as you have already installed Docker and the GDS environment. Instead you can start from [Running Python through Docker](running-the-container) and carry on from there.

<br>

This resource is adapted from Arribas-Bel, Dani. 2019. gds_env: A Containerised Platform for Geographic Data Science (version 6.1). https://darribas.org/gds_env.
