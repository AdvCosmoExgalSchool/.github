# ACES

...

## Repos

The repositories containing the hands-on workshop materials are all contained in this GitHub organisation. Make yourself a directory for the summer school and clone each of these into it.

- Simulations: UNDER CONSTRUCTION
- Cosmology: UNDER CONSTRUCTION
- Observations: UNDER CONSTRUCTION

## Prerequistes

For most of the summer school, you will only need a Python installation and some easily installed Python packages. We will cover this below in the **Python Environment** section. You will need some extra software for the simulations portion, which we'll walk you through in the **Simulation Dependencies** section.

HOWEVER, if you are a Windows user you will need to do some extra work. A few pieces of software will not run on Windows reliably but run without issue on Linux. If you are not a Windows user you can skip the following section.

### Windows Subsystem for Linux

Microsoft have made it much easier to run a Linux virtual machine on your Windows machine. You can use this to ensure you can take part in the hands-on workshops that are part of this summer school.

To run Linux we will use the [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/about). To install WSL simply follow the instructions detailed [here](https://learn.microsoft.com/en-us/windows/wsl/install#install-wsl-command). It's a simple process that involves a few command line commands, let us know if you have any trouble.

Once you have Linux up and running simply open the terminal and you can clone the repositories into a location of your choosing and move on to the next sections.

### Python Environment

Firstly you will need Python `>=3.10`. To check which version of Python you are using you can run `python --version` on the command line. There are various ways to install specific Python versions including your Linux software provider and homebrew. `pyenv` is a very good way of keeping track of multiple Python installations if you want to install a tool to help managing Python versions.

Once you have ascertained you have a compatible Python version you can install the Python packages you will need. These are listed, along with installation instructions, below.

- `Synthesizer`: A forward modelling python package. To install first clone the repo with `git clone https://github.com/flaresimulations/synthesizer.git`, enter the repo and then run `pip install .`.
- `CAMB`: Code for Anisotropies in the Microwave Background - Install with `pip install camb`.
- `cobaya`: Code for bayesian analysis. Install with `pip install cobaya`.

### Simulation Dependencies
