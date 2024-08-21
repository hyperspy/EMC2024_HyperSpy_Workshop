# EMC2024 HyperSpy Workshop

Training material used during the 2024 HyperSpy Workshop at the European Microscopy Congress 2024 in Copenhagen.


## Tutorial venue and schedule

### Venue

Haderup auditoriet, Panum Instituttet, Blegdamsvej 3, 2200 Kbh. N. (Careful, not CFIM, but Haderup auditoriet).

### Schedule

The workshop will take place from 9:00 to 17:00 CEST on Sunday the 25th of September.

| Time         | Activity                   | Presenter              |
|--------------|----------------------------|------------------------|
| 8:30-9:00    | Welcome coffee/tea         |                        |
| 9:00-9:15    | Introduction talk          | Francisco de la Peña   |
| 9:15-10:30   | Getting started            | Magnus Nord            |
| 10:30-10:45  | Coffee break               |                        |
| 10:45-11:30  | Decomposition and BSS      | Francisco de la Peña   |
| 11:30-12:15  | Curve fitting              | Francisco de la Peña   |
| 12:15-13:00  | EDX                        | Katherine MacArthur    |
| 13:00-13:45  | Lunch break                |                        |
| 13:45-14:30  | EELS                       | Francisco de la Peña   |
| 14:30-15:15  | LumiSpy                    | Gunnar Kusch           |
| 15:15-15:30  | Coffee break               |                        |
| 15:30-16:15  | Lazy signals for Big Data  | Magnus Nord            |
| 16:15-17:00  | Pyxem                      | Magnus Nord            |


## Software installation

To use the Jupyter Notebooks in this repository, you need to install some software packages first. It installation instructions for beginners and advanced users can be found below.


### Simple installation instructions (best for Python beginners)

The easiest way to install all the software required to run the Jupyter Notebooks in this repository is to [install the HyperSpy Bundle](https://hyperspy.org/hyperspy-bundle/install.html) that you can download from [here](https://github.com/hyperspy/hyperspy-bundle/releases/latest).


### Advanced installation instructions (for advanced users)

If you prefer to customize your installation, we suggest installing a conda distribution (we suggest [MiniForge](https://github.com/conda-forge/miniforge)) and install all the required Python packages in a dedicated environment executing the following commands in a terminal (the conda prompt in Windows):


```bash
conda install nb_conda_kernels jupyterlab start_jupyter_cm ipympl -c conda-forge
conda create -n hyperspy_EMC2024 python=3.11 hyperspy pyxem ipympl exspy lumispy ipykernel -c conda-forge
```

To add Jupyter to the context menu of your file browser execute the following command:

```bash
start_jupyter_cm
```

To use HyperSpy in JupyterLab, start Jupyter Lab and choose the `Python [conda env:hyperspy_EMC2024]` kernel. Alternatively, start JupyterLab from the `hyperspy_EMC2024` environment as follows:

```bash
conda activate hyperspy_EMC2024
jupyter lab
```
