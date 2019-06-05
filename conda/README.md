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

## PC Errors

ResolvePackageNotFound: 
- sip==4.19.8=py37h0a44026_0
- mkl_fft==1.0.12=py37h5e564d8_0
- ncurses==6.1=h0a44026_1
- libiconv==1.15=hdd342a3_7
- dbus==1.13.6=h90a0687_0
- libedit==3.1.20181209=hb402a30_0
- sqlite==3.28.0=ha441bb4_0
- freetype==2.9.1=hb4e5f40_0
- intel-openmp==2019.3=199
- icu==58.2=h4b95b61_1
- pyqt==5.9.2=py37h655552a_0
- tornado==6.0.2=py37h1de35cc_0
- libpng==1.6.37=ha441bb4_0
- libcxx==4.0.1=hcfea43d_1
- xz==5.2.4=h1de35cc_4
- numpy-base==1.16.4=py37h6575580_0
- numpy==1.16.4=py37hacdab7b_0
- kiwisolver==1.1.0=py37h0a44026_0
- glib==2.56.2=hd9629dc_0
- expat==2.2.6=h0a44026_0
- openssl==1.1.1c=h1de35cc_1
- libgfortran==3.0.1=h93005f0_2
- tk==8.6.8=ha441bb4_0
- mkl_random==1.0.2=py37h27c97d8_0
- matplotlib==3.1.0=py37h54f8f79_0
- python==3.7.3=h359304d_0
- jpeg==9b=he5867d9_2
- qt==5.9.7=h468cd18_1
- zlib==1.2.11=h1de35cc_3
- pcre==8.43=h0a44026_0
- libffi==3.2.1=h475c297_4
- libcxxabi==4.0.1=hcfea43d_1
- readline==7.0=h1de35cc_5
- mkl==2019.3=199
- gettext==0.19.8.1=h15daf44_3