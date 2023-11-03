# Standard Installation

## A standard approach: `anaconda` installer (easiest to work with)

Follow the instructions on the [Anaconda](https://www.anaconda.com/products/distribution) website and install a distribution which contains Python 3.9. Once the software is installed, double click on it, and confirm that you have something called JupyterLab already installed within it. You are done!

- Once you have anaconda installed, we need to set up an independent virtual environment that isolates all the functionality we need.

```{important}
But first, **what are environments and do you need them?**
```

Environments in Python are like sandboxes that have different versions of Python and/or packages installed in them. You can create, export, list, remove, and update environments. Switching or moving between environments is called activating the environment. When you are done with an environment, you may deactivate it.

For this course, we want to have a bit more control on the packages that will be installed with the environment so we will create an environment with a so-called YAML file called `install_gds_stack.yml`.

To learn more about virtual environments, you can also go [here](environment.md).

### Creating an environment from an environment.yml file

Get the installer file from [here](../resources/install_gds_stack.zip) and unzip it.

Open up the anaconda navigator:
* Go to "Environments"
* Click on "Import"
* From your local drive, import the installer file you just downloaded
* Give the environment a name, like "gds"
* Remeber to keep the option "Overwrite exisiting environment" unchecked


```{tip}
Depending on the speed of your connection, this step will take a while (but no less than 15-30 minutes). Grab a *cuppa* and be patient!
```

This has created the `gds` environment, congratulations! We are _almost_ there. Now we need to _activate_ the environment. For this, just  select the right environment and open a jupyter lab notebook.
