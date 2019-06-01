# Anaconda Environment

This directory contains a description of our Anaconda environment that you can use to recreate it for consistency.

We noticed that there are idiosyncrasies in the `Qt` available via the Anaconda distribution channels. Most notably, only version 5.9 of `pyqt` is available and, even then, some builds seem to have trouble finding some modules e.g., `ModuleNotFoundError: No module named 'PyQt5.QtMultimedia'`.

(See <https://github.com/ContinuumIO/anaconda-issues/issues/10250> for details of others' problems.)

We reverted to the most recent `pyqt` we could find without this problem.

## Recreating our environment

You can recreate the environment in your Conda-verse using ---

```bash
conda env create -f environment.yml
```

This will create a new environment `qcsf` that you can activate using the usual mechanism ---

```bash
conda activate qcsf
```
