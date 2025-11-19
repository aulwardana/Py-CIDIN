# Py-CIDIN
Python-based Collaborative Intrusion Detection Simulation in Integrated Networks

## Setup

This simulator was developed and tested on the Ubuntu operating system. Therefore, we recommend using this operating system for the best results. If you want to used other operating system you can used linux based, Mac OS, o Windows Subsystem for Linux (WSL) on Windows OS.  

We also suggest utilizing a package and environment management system. For this simulator, we recommend using Miniconda.

However, if you prefer not to use a package and environment management system, you can skip the "Miniconda installation" and "prepare environment using Miniconda" sections.

### Miniconda Instalation

Create folder to download miniconda installation

```bash
mkdir -p ~/miniconda3
```

Download miniconda installation

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```

Run miniconda installation

```bash
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
```

Remove miniconda instalation folder

```bash
rm -rf ~/miniconda3/miniconda.sh
```

Load miniconda

```bash
~/miniconda3/bin/conda init bash
```

```bash
~/miniconda3/bin/conda init zsh
```

After that, close the terminal and open again, then you can continue to "Prepare Environment using Miniconda" part.

### Prepare Environment using Miniconda

Create environment with python 3.12 and install libraries

```bash
conda create --name pycidin_env python=3.10
```

Then activate the environment

```bash
conda activate pycidin_env
```

After that, install jupyter notebook

```bash
conda install notebook
```

### Clone Repositories

Now you need to clone this repositories. Run the command below, make sure that `git` is already installed.

```bash
git clone https://github.com/aulwardana/Py-CIDIN.git
```

Then open the cloned repositories

```bash
cd Py-CIDIN
```

Next, you need to install the requirement for the library.

### Install Requirements

Run this command to installs all the packages for simmulator needs.

```bash
pip install -r requirements.txt
```

### Run Jupyter Notebook

Run this command to open Jupyter Notebook in browser.

```bash
jupyter notebook
```

This will display information about the notebook server in your terminal, including the URL for the web application, which is typically `http://localhost:8888` by default.

After all the setup done, you can open "src" folder in github page for the next instruction.

## Development Tool

This simulator is develop using Python programming language with Jupyter Notebook as code editor.

To develop the simulator, a server with specific technical specifications was utilized: a AMD EPYC 7713 64-Core processor coupled with 64 GB of RAM.