# SpurHacks June 2025 - Qiskit Workshop

## Installing Qiskit

It is recommended that you use Python enviroments for installing Qiskit. You can facilitate this in one of two ways:

- Use the Python Virtual Environments package (```venv```)
- Use Anaconda or Miniconda Python, and the ```conda``` command

NOTE: Mac computers with M-series CPUs may find difficulty when installing Python packages needed for Qiskit. Notably, this includes the ```scipy``` package, which may invoke the installation commands to compile this module from source code. This is a long process and requires that C/C++ development tools are installed on your system. It is recommended that Mac M-series users use the Anaconda/Miniconda route for setting up their Python/Qiskit programming environment, and use the ```conda``` command to install ```scipy``` prior to installing Qiskit packages.

### Install with Virtual Environments (```venv```)

Check that Python is installed on your system by running the ```python --version``` command. If it is not installed, then download the latest version of Python from: https://www.python.org/downloads/ . If Python is already installed, verify that the version is v3.9 or higher.

Create a Python virtual environment:
```
python3 -m venv /path/to/virtual/environment
```

Activate this new environment:
```
source /path/to/virtual/environment/bin/activate
```

Now, skip to the Install Qiskit packages section for further instructions.

### Install Anaconda Python or Miniconda.

Install Anaconda from here: https://www.anaconda.com/download, OR
install Miniconda from here: https://docs.anaconda.com/miniconda/miniconda-other-installer-links/

Create a conda environment and activate:
```
conda create -n qiskit python=3
conda activate qiskit
```

NOTE: For Mac M-series computers, install the ```scipy``` packages as follows:
```
conda install scipy
```

Now, go to the next section Install Qiskit packages section for further instructions.

### Install Qiskit packages:
```
pip install qiskit qiskit-ibm-runtime
```

Install additional Qiskit packages:
```
pip install qiskit-aer 
```

Install Jupyter and other tools:
```
pip install jupyter matplotlib pylatexenc
```
