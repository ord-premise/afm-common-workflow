# D4.3 - Release demonstrator implementation for selected AiiDA common workflows of use in WP2

This repository serves as a central reference for the various components involved in implementing the AFM common workflow in AiiDA.

## Authors

- Edan Bainglass (PSI)

## Goal

The purpose of this deliverable is to provide a demonstrator implementation of the AFM common workflow in AiiDA used by the Empa lab in WP2.
To do so, we implement the following components in AiiDA common workflows (ACWF):

1. A common workflow for post-processing of DFT simulation results
2. A composite common workflow for AFM simulations, with a concrete implementation for the Quantum ESPRESSO code, leveraging common workflows for DFT and post-processing

The composite AFM common workflow uses the Probe-Particle AFM (ppafm) code as the backend for AFM simulations.

## Achievement

The references in this repository point to contributions in the relevant repositories.
Here we also provide a notebook (`afm_workflow_demo.ipynb`) to test out the new AFM common workflow (see instructions below).

### Instructions to run the notebook

1. Create a Python environment
2. Install the Python dependencies with `pip install -r requirements.txt`
3. Install Quantum ESPRESSO (**QE v7.4**), if not already installed - see note below
4. Create a new AiiDA profile with `verdi presto`
5. Register the Quantum ESPRESSO codes with AiiDA - see note below
6. Import the pseudopotential into AiiDA - see note below
7. Start a Jupyter notebook server with `jupyter notebook`
8. Open and run the notebook `afm_workflow_demo.ipynb`

#### Note regarding Quantum ESPRESSO installation

The notebook uses the Quantum ESPRESSO (**QE v7.4**) implementation of the AFM common workflow.
To run the notebook, you need to have Quantum ESPRESSO installed, and its `pw.x` and `pp.x` executables available.
Instructions for this part are outside the scope of this repository.
However, we note that a QE installation is available in Conda (conda-forge channel), and thus recommend using Conda as your Python environment manager.

Once installed, you need to register the codes with AiiDA.
Finally, you need to install the pseudopotential.
Instructions on this can be found [here](https://aiida-quantumespresso.readthedocs.io/en/stable/get_started/installation.html#codes).

## External links

- [AiiDA common workflow for post-processing of DFT results](https://github.com/aiidateam/aiida-common-workflows/pull/342)
- [AiiDA common workflow for AFM simulations](https://github.com/aiidateam/aiida-common-workflows/pull/343)
- [Probe-Particle AFM code](https://github.com/Probe-Particle/ppafm)

## Acknowledgements

The author acknowledges Dr. Xing Wang, Dr. Miki Bonacci, Dr. Carlo Pignedoli, and Timo Reents for their time and support during the development of the common workflow.

The [PREMISE](https://ord-premise.org/) project is supported by the [Open Research Data Program](https://ethrat.ch/en/eth-domain/open-research-data/) of the ETH Board.

![image](https://ord-premise.org/assets/img/logos/PREMISE-logo.svg)

![image](https://ethrat.ch/wp-content/uploads/2021/12/ethr_en_rgb_black.svg)
