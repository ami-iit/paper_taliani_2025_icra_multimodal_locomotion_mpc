<h1 align="center">
Online Nonlinear MPC for Multimodal Locomotion
</h1>


<div align="center">


S. Taliani, G. Nava, G. L'Erario, M. Elobaid, G. Romualdi, D. Pucci, "Online Nonlinear MPC for Multimodal Locomotion" in 
2025 IEEE International Conference on Robotics and Automation (ICRA), Atlanta, USA, May 2025.

</div>

<p align="center">

https://github.com/user-attachments/assets/14686435-7e4e-45d6-93d5-540ffdd34f39

</p>




<div align="center">
  <a href="#installation"><b>Installation</b></a> |
  <a href="https://ieeexplore.ieee.org/"><b>Paper</b></a>
</div>


## Abstract

Aerial humanoid robots can enhance the efficiency and safety of rescue operations in disaster scenarios. The control of such complex machines presents many challenges, for instance, the control of the different locomotion strategies and the stabilization of the transition maneuvers.
In this article, we present an online nonlinear Model Predictive Controller and the relative prediction model to stabilize walking and flying trajectories. The controller uses a reduced model to generate feasible base link references, thrust profiles, and contact forces while dealing with different locomotion strategies and transition maneuvers. The control algorithm is tested in a simulated environment using our aerial humanoid robot iRonCub under the effect of external disturbances. The proposed control strategy demonstrates to effectively stabilize the desired trajectories while keeping the problem still treatable online.

## Installation

A quick way to install the dependencies is via [conda package manager](https://docs.conda.io) which provides binary packages for Linux, macOS and Windows of the software contained in the robotology-superbuild. Relying on the community-maintained [`conda-forge`](https://conda-forge.org/) channel and also the `robotology` conda channel.

Please refer to [the documentation in `robotology-superbuild`](https://github.com/robotology/robotology-superbuild/blob/master/doc/conda-forge.md) to install and configure a conda distribution. Then, once your environment is set, you can run the following command to install the required dependencies.

1. Clone the repository:
    ```sh
    https://github.com/ami-iit/paper_taliani_2025_icra_multimodal_locomotion_mpc.git
    ```
2. Install conda dependencies:
    ```sh
    cd paper_taliani_2025_icra_multimodal_locomotion_mpc
    mamba env create -n <conda-environment-name> --file environment.yml
    mamba activate  <conda-environment-name>
    ```
3. Specify the number of threads used by the optimiser:
   ```sh
   mamba env config vars set OMP_NUM_THREADS=1
   ```
4. Install python repository:
    ```sh
    pip install -e .
    ```

> [!WARNING]
> Note that to replicate the paper results, you need to install the HSL solvers (here we use `ma97`), which can be downloaded but not redistributed. Please check [here](https://licences.stfc.ac.uk/product/coin-hsl).

> [!NOTE]
> The installation procedure has been tested on `Ubuntu 22.04`.

## Usage


### Maintainer

This repository is maintained by:

| | |
|:---:|:---:|
| [<img src="https://github.com/user-attachments/assets/077ed5f4-4691-45dc-b9b0-80af434896c5" width="40">](https://github.com/STaliani) | [@STaliani](https://github.com/STaliani) |

