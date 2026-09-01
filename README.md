# Modeling and Simulation of Damage Caused by Needle Insertion

## Overview
This repository serves as the central hub for the research project Modeling and Simulation of Damage Caused by Needle Insertion.

The research focuses on modeling needle insertion into human-like tissue and investigating the resulting tissue damage. The numerical simulations are based on the finite element method (FEM) and are implemented using FEniCSx.

## Installation
The following setup instructions are intended for Windows.

1. Install Ubuntu
    - Open Powershell and run:
        - `wsl --install -d Ubuntu-24.04 --name MB-21`
    - Exit and start WSL via:
        - `wsl -d MB-21 --cd ~`
        - `exit`
2. Clone this repository
    - `git clone https://github.com/course-mb21/research-hub.git`
3. Install Docker Desktop
    - Go to Settings -> Resources -> WSL integration -> check MB-21
4. Create the Container
    - In Ubuntu navigate to the my-dolfinx-lab folder and run:
        - `docker build -t my-dolfinx-lab .`
    - Create the container:
        - `sh run-mylab.sh`
5. Run the Container
    - In Docker Desktop go to the Containers tab
    - Start the fenicsx-dev container
    - Go to the Logs tab and paste this URL in your Browser:
        - `http://127.0.0.1:8888/lab?token=...`

JupyterLab should now open, and the Python scripts and notebooks can be executed inside the FEniCSx development environment.
