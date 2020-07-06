# Jupyter_with_Virtualenv

## Install Jupyter and set it up

### Install

open your terminal and type:

```
pip install Juperter

```

### Setup

#### Base setup


open your terminal and type:

```
jupyter notebook --generate-config
# This command can automatically genrate jupyter config file in "C:\Users\<your user name>\.jupyter" when you use windows as Operating System
# will genrate jupyter_notebook_config.py and jupyter_notebook_config.json

jupyter notebook --ip=your-ip --port=your-port

Example: jupyter notebook --ip=0.0.0.0[1] --port=12345
```

And set your password if you want.

```
jupyter notebook password
and follow the follow the command in terminal.

That password will be a key when somebody try to connect to your jupyter notebook.

[1]
0.0.0.0 mean it allow all host to connect this jupyter notebook like your ip or a domain name that direct to your ip.
So your URL will be https://your-ip||:your-port/
```

#### Bonus! when you try to change notebook directory

```
Go to C:\Users\<your user name>\.jupyter in windows system

open jupyter_notebook_config.py with text editor.

find c.NotebookApp.notebook_dir 
# you can use ctrl+f to find more faster
Uncomment that line and type the directory path you want to use.
```


## Install Virtualenv and use the kernel in jupyter

### Install

open your terminal and type:

```
pip install virtualenv
```

### Setup

#### Base setup

And go to a directory you want to setup Virtualenv.
In this example is D:\Jupyter_with_Virtualenv.

```
# Go to D:\Jupyter_with_Virtualenv
cd D:\Jupyter_with_Virtualenv

D:\Jupyter_with_Virtualenv> virtualenv For_jupyter
```

And you can see the directory tree will be like:

```
1week_class
|-- 1_week_env
```

