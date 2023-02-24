# Collective diffusions

<img src=./Ion.svg width="20%">

The following project is aimed to extract diffusive paths from molecular dynamics simulations of solids.

Code is under active development, please be aware that file formats and folders distributions may change. Bug reports are also welcomed in the GitHub issues!

## Installation

Required modules:

* Python >= 3.7

To install:

```bash
$ git clone https://github.com/group-name/ColectiveDiffusions.git
$ pip3 install -r requirements.txt
```

### Basic network training

To extract diffusion paths from a simulation XDATCAR file located at examples folder from the ColectiveDiffusions folder run:

```bash
$ python3 cli.py identify_diffusion --MD_path examples
```

A simulation of non-stoichiometric LLZO at 400K is provided to run an example:
 - [`examples/INCAR`](examples/INCAR): Basic parameters of the simulation (only **POTIM** and **NBLOCK** flags are considered).
 - [`examples/XDATCAR`](examples/XDATCAR): Concatenation of all simulated configurations (recorded each **NBLOCK** simulation steps).
 - [`examples/README.md`](examples/README.md): More specific information regarding these files.

## References & citing

The theory behind ColectiveDiffusions code is described in our preprint (1). If you use this repository in your work, please consider the following citation:

 1. some-DOI

## Authors

ColectiveDiffusions is being developed by:

 - Cibrán López Álvarez
 - ...
 - Claudio Cazorla Silva

## Contact, questions, and contributing

If you have questions, please don't hesitate to reach out at cibran[dot]lopez[at]upc[dot]edu.
