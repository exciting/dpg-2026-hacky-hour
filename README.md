# An exciting approach to electronic structure theory

### Resources: [abstract](https://www.dpg-verhandlungen.de/year/2026/conference/dresden/part/akjdpg/session/1/contribution/4?lang=en), [webpage](https://exciting-code.org/dpg-hacky-hour-2026), [github page](https://github.com/exciting/dpg-2026-hacky-hour)

## Cloning this repository
In your terminal, please type:
```bash
git clone https://github.com/exciting/dpg-2026-hacky-hour.git
``` 

## Running the tutorials
These hands-on tutorials are designed to provide an overview of different methods implemented in the [`exciting`](https://exciting-code.org/) code and how they can be used. Due to time contraints, we do not perform the actual simulations but rather fetch results from precomputed datasets, published on [NOMAD](https://nomad-lab.eu). However, it must be noted that the commands remain mostly the same for actual exciting runs, we just refer to a 'mock' exciting-program instead of calling the actual program. It still downloads results in the exact same way as you would obtain with the actual program.

In our experience, each of the tutorials takes about 15-20 minutes to complete. We therefore recommend you to focus on one notebook your choice and check the other ones at a later point. You have the opportunity to choose a notebook based on the following methods:

1. 3-in-1: Calculating ground state properties using **GGA**, **metaGGA** and **hybrid** functionals -- recommended for beginners
2. Calculation of excited-state properties using the **G<sub>0</sub>W<sub>0</sub>** approximation
3. Calculation of optical spectra using the **Bethe-Salpeter equation** 
4. Studying the optical response using **RT-TDDFT**
5. Calculation of phonon modes using **density-functional perturbation theory**

<details>
<summary><strong>Installation using python venv</strong></summary>
Make sure you use a Python version >= 3.12. 

Afterwards, in the folder where this README file is, type:

```bash
python -m venv DPG_env
source DPG_env/bin/activate

pip install excitingscripts jupyter

jupyter notebook
```
</details>

<details>
<summary><strong>Installation using uv</strong></summary>
If you don't have it installed, you can download and install uv by following the instructions here:  

https://docs.astral.sh/uv/  
Afterwards, in the folder where this README file is, type:

```bash
uv venv -p 3.12

uv pip install excitingscripts jupyter

uv run jupyter notebook
```
</details>

<details>
<summary><strong>Installation using conda</strong></summary>
If you don't have it installed, you can download and install conda by following the instructions here:  

https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html  
Afterwards, in the folder where this README file is, type:

```bash
conda create -n DPG_env python=3.12
conda activate DPG_env

pip install excitingscripts jupyter

jupyter notebook
```
</details>

