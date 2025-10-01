# D4.3 - Release demonstrator implementation for selected AiiDA common workflows of use in WP2

This repository serves as a central reference for the various components involved in implementing the AFM common workflow in AiiDA.
It provides a notebook (`afm_workflow_demo.ipynb`) demonstrating the usage of the AFM common workflow, along with links to the relevant contributions in the respective repositories.

## Authors

- Edan Bainglass (PSI)
- Carlo Pignedoli (Empa)

## Goal

The purpose of this deliverable is to provide a demonstrator implementation of the AFM common workflow in AiiDA used by the Empa lab in WP2.
To do so, we implement the following components in AiiDA common workflows (ACWF):

1. A common workflow for post-processing of DFT simulation results
2. A composite common workflow for AFM simulations, with a concrete implementation for the Quantum ESPRESSO code, leveraging common workflows for DFT and post-processing

The composite AFM common workflow uses the Probe-Particle AFM (ppafm) code as the backend for AFM simulations.

## Achievement

The references in this repository point to contributions in the relevant repositories.
The provided notebook (`afm_workflow_demo.ipynb`) demonstrates the new AFM common workflow in action.
The AFM common workflow was developed in collaboration with the Empa lab to ensure it meets their requirements and is suitable for their use cases.

## External links

- [AiiDA common workflow for post-processing of DFT results](https://github.com/aiidateam/aiida-common-workflows/pull/342)
- [AiiDA common workflow for AFM simulations](https://github.com/aiidateam/aiida-common-workflows/pull/343)
- [Probe-Particle AFM code](https://github.com/Probe-Particle/ppafm)

## Acknowledgements

The author acknowledges Dr. Xing Wang, Dr. Miki Bonacci, Dr. Carlo Pignedoli, and Timo Reents for their time and support during the development of the common workflow.

The [PREMISE](https://ord-premise.org/) project is supported by the [Open Research Data Program](https://ethrat.ch/en/eth-domain/open-research-data/) of the ETH Board.

![image](https://ord-premise.org/assets/img/logos/PREMISE-logo.svg)

![image](https://ethrat.ch/wp-content/uploads/2021/12/ethr_en_rgb_black.svg)
