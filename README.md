# Roseau Load Flow Solver Tutorials

## Overview

Welcome to the _Roseau Load Flow Tutorials_. This series of tutorials provides a comprehensive
overview of the steps needed to model and analyze electrical networks using the _Roseau Load Flow_
solver.

The tutorial is designed for power system engineering students, professionals, researchers and
consultants. It requires a basic level of Python skills. Whatever your background, this tutorial
will be valuable for understanding the intricacies of the _Roseau Load Flow_ solver.

## Pre-Requisites

To follow the tutorials, you will need the following:

1. Clone this repository to your local machine
   ```sh
   git clone https://github.com/RoseauTechnologies/Roseau_Load_Flow
   ```
2. Move to the tutorials directory
   ```sh
   cd Roseau_Load_Flow/tutorials
   ```
3. Install the required packages. It is highly recommended to use
   [uv](https://docs.astral.sh/uv/getting-started/installation/)
   ```sh
   uv sync
   ```
   If for any reason you are unable to use `uv`, you can install the required packages using `pip`.
   In this case you have to create a virtual environment and activate it manually:
   ```sh
   # Create a virtual environment
   python -m venv .venv
   # Activate the virtual environment
   source .venv/bin/activate  # On windows, use `.venv\Scripts\activate` instead
   # Install the required packages
   python -m pip install -r requirements.txt
   ```
4. Open the project in your favorite IDE or in Jupyter Notebook and get started.

## OpenDSS

This directory is designed to help _OpenDSS_ users to use _Roseau Load Flow_.

### Tutorial 1

This tutorial involves modelling a simple LV network and is designed to familiarize the user with
the basic workflow of _Roseau Load Flow (RLF)_. You will learn the following:

1. How to model common network components such as buses, lines, transformers, etc. in _RLF_ as well
   as RLF-specific components.
2. How to build a network and run power flow simulations in _RLF_.
3. How to access different types of results for various network elements

### Tutorial 2

This series of tutorials focuses on the modelling flexibility of _RLF_ as well as benchmarking _RLF_
with _OpenDSS_, a popular power flow solver. It will also demonstrate the interoperability of RLF
with OpenDSS. In this tutorial, you will learn the following:

1. How to convert OpenDSS parameters into _RLF_ parameters
2. How to model networks with a single-wire earth return systems in _RLF_

## Contributing

We welcome contributions form the community. If you have an idea for a new tutorial, bug fixes or
improvements to existing tutorials, please feel free to submit a pull request.

## Support

If you encounter any issues or have questions, please open an issue on GitHub. We are here to help
and ensure that you have a smooth learning experience.

## License

The tutorials are licensed under the MIT License.
