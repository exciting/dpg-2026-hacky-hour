**Resources:** [abstract](https://www.dpg-verhandlungen.de/year/2026/conference/dresden/part/akjdpg/session/1/contribution/4?lang=en), [webpage](https://exciting-code.org/dpg-hacky-hour-2026), [github]()

Instructions for participants of the DPG-hacky hour session "An exciting approach to electronic structure theory":

**Step 0 - Cloning this repository**
```bash
git clone https://github.com/exciting/dpg-2026-hacky-hour.git
``` 

**Step 0.1 - Installing required libraries**
```bash
pip install excitingscripts
```

These notebooks/hands-on tutorials are designed to provide a brief overview of the methodology and workflow for their respective methods. Due to time contraints, we do not perform the actual simulations but rather fetch results from precomputed datasets, published on [NOMAD](https://nomad-lab.eu). However, it must be noted that the commands remain mostly the same for actual exciting runs, we just refer to a 'mock' exciting-program rather than calling the actual binary; this 'mock' program still downloads results in the exact same way as you would obtain with the actual binary.

In our experience, each of these 'methods' takes about 15-20 minutes to go-through, and hence we recommend participants to be aquainted with one notebook of their choice in this session and checkout the others at their own leisure later. You have the opportunity to choose a notebook based on the following methods:

1. 3-in-1: Calculating ground state properties using **GGA**, **metaGGA** and **hybrid** functionals -- recommended for beginners
2. Calculation of excited-state properties using one-shot **GW** approximation
3. Calculation of optical spectra using the **Bethe-Salpeter equation** 
4. Studying the optical response using **RT-TDDFT**
5. Calculation of phonon mode using **density-functional perturbation theory**

<details>
<summary><strong>Helpful instruction for step 0.1 – setting up a python environment and jupyter kernel (using conda)</strong></summary>

```bash
conda create -n DPG_env python=3.11
conda activate DPG_env

pip install excitingscripts

python -m ipykernel install --user --name DPG_env --display-name "Python (DPG_env)"
```
</details>
