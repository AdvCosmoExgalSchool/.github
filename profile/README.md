# ACES

...

## Repos

The repositories containing the hands-on workshop materials are all contained in this GitHub organisation. Make yourself a directory for the summer school and clone each of these into it.

- Simulations: UNDER CONSTRUCTION
- Cosmology: UNDER CONSTRUCTION
- Observations: https://github.com/AdvCosmoExgalSchool/Synthesizer-SED-Workshop

## Prerequistes

For most of the summer school, you will only need a Python installation and some easily installed Python packages. We will cover this below in the **Python Environment** section. You will need some extra software for the simulations portion, which we'll walk you through in the **Simulation Dependencies** section.

HOWEVER, if you are a Windows user you will need to do some extra work. A few pieces of software will not run on Windows reliably but run without issue on Linux. If you are not a Windows user you can skip the following section.

### Windows Subsystem for Linux

Microsoft have made it much easier to run a Linux virtual machine on your Windows machine. You can use this to ensure you can take part in the hands-on workshops that are part of this summer school.

To run Linux we will use the [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/about). To install WSL simply follow the instructions detailed [here](https://learn.microsoft.com/en-us/windows/wsl/install#install-wsl-command). It's a simple process that involves a few command line commands, let us know if you have any trouble.

Once you have Linux up and running simply open the terminal and you can clone the repositories into a location of your choosing and move on to the next sections.

### Python Environment

Firstly you will need Python `>=3.10`. To check which version of Python you are using you can run `python --version` on the command line. There are various ways to install specific Python versions including your Linux software provider and homebrew. `pyenv` is a very good way of keeping track of multiple Python installations if you want to install a tool to help manage Python versions.

Although this step isn't 100% required it's recommended to set up an isolated environment for the summer school to ensure there are no version clashes. To do so navigate to the location you want to keep the environment and run:
```bash
python -m venv aces-env
```
This will create a directory called `aces-env` which contains the python environment. To activate the environment run:
```bash
source aces-env/bin/activate
```
Note that the above is different on Windows but you shouldn't be using Windows if you got this far...

Once you have ascertained you have a compatible Python version and setup your environment you can install the Python packages you will need. These are listed, along with installation instructions, below.

- `Synthesizer`: A forward modelling python package. To install first clone the repo with `git clone https://github.com/flaresimulations/synthesizer.git`, enter the repo and then run `pip install .`.
- `Bagpipes`: A Bayesian SED fitting code. Install with `pip install bagpipes`.
- `MulitNest`: Bayesian inference tool. Instructions can be found [here](https://bagpipes.readthedocs.io/en/latest/index.html) but if these don't work, `nautilus` should work instead.
- `CAMB`: Code for Anisotropies in the Microwave Background - Install with `pip install camb`.
- `cobaya`: Code for Bayesian analysis. Install with `pip install cobaya`.
- `swiftsimio`: A tool for interacting with SWIFT outputs. Install with `pip install swiftsimio`.
- `notebook`: Jupyter notebooks. Install with `pip install notebook` (once installed you can invoke `notebook` on the command line to open a jupyter notebook session in the browser).

### Simulation Dependencies

For the simulation workshop, the setup is a little bit more involved. You will need some software packages required by the code and will need to compile the simulation code itself.

This setup is described in detail in the workshop [README](https://github.com/AdvCosmoExgalSchool/SWIFT-Workshop/blob/main/README.md).
