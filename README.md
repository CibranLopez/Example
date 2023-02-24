# Collective diffusions

The following project is aimed to extract diffusive paths from molecular dynamics simulations of solids.
python3 cli.py identify_diffusion --MD_path examples

<img src=./Ion.svg width="20%">

**PLEASE NOTE:** the present code is under active development and is still in beta versions 0.x.x. In general changes to the patch version (the third number) indicate backward compatible beta releases, but please be aware that file formats and APIs may change. Bug reports are also welcomed in the GitHub issues!

## Installation

Required modules:

* Python >= 3.7

To install:

```bash
$ git clone https://github.com/group-name/ColectiveDiffusions.git
```

## Tutorial 

The best way to learn how to use NequIP is through the [Colab Tutorial](https://bit.ly/mrs-nequip). This will run entirely on Google's cloud virtual machine; you do not need to install or run anything locally.

### Basic network training

To train a network, you run `nequip-train` with a YAML config file that describes your data set, model hyperparameters, and training options. 

```bash
$ python3 cli.py identify_diffusion --MD_path examples
```

A simulation of non-stoichiometric LLZO at 400K is provided to run an example:
 - [`examples/INCAR`](examples/INCAR): Basic parameters of the simulation (only **POTIM** and **NBLOCK** flags are considered).
 - [`examples/XDATCAR`](examples/XDATCAR): Concatenation of all simulated configurations (recorded each **NBLOCK** simulation steps).
 - [`examples/README.md`](examples/README.md): More specific information regarding these files.

## References & citing

The theory behind NequIP is described in our preprint (1). NequIP's backend builds on e3nn, a general framework for building E(3)-equivariant neural networks (2). If you use this repository in your work, please consider the following citation:

 1. some-DOI

## Authors

NequIP is being developed by:

 - Cibrán López Álvarez
 - Claudio Cazorla Silva

## Contact, questions, and contributing

If you have questions, please don't hesitate to reach out at cibran[dot]lopez[at]upc[dot]edu.
