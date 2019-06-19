# QuickCSF

A fast, adaptive approach to estimating contrast sensitivity function parameters.

This implementation is based on:

> Lesmes, L. A., Lu, Z. L., Baek, J., & Albright, T. D. (2010). Bayesian adaptive estimation of the contrast sensitivity function: The quick CSF method. *Journal of vision*, 10(3), 17-17.

Special thanks to Dr. Tianshi Lu at Wichita State University for providing a MATLAB implementation of the fundamental algorithm and Dr. Rui Ni at Wichita State University for the motivation.

## Dependencies

Dependencies are installed via the `conda env` command. They include ---

* `numpy` - numerical calculations
* `qtpy` - mystical py-glue
* `pyqt` - python bindings, right now at v 5.9 in Anaconda, 5.13 in the wild.

<!-- 
Requires:

* `numpy`
* `qtpy`
* Qt bindings (via `PySide2`, `PyQt5`, `PySide`, or `PyQt`)

Optional (for simulation visuals):

* `matplotlib` -->

## Installation

<!-- 
~~~~bash
pip3 install -e .
~~~~ -->

To install into a environment using Anaconda, use the description found in the `conda` directory.

When using Anaconda, you should **not** run the supplied `setup.py`, but instead, use the `conda env` command. See the `README.md` in the `conda/` directory for information.

## Usage

### Measuring CSF

Ensure you are using the `qcsf` environment in Anaconda, using:

~~~bash
conda activate qcsf
~~~

Run:

~~~bash
python -m QuickCSF.app
~~~

A settings dialog will appear; session ID and viewing distance are required. Arguments can also be specified on the command line. Use the `--help` flag to see all options:

~~~bash
python -m QuickCSF.app --help
~~~

### Simulate and visualize an evaluation

Run:

~~~bash
python -m QuickCSF.simulate
~~~

A settings dialog will appear; the number of trials is required. Arguments can also be specified on the command line. use the `--help` flag to see all options:

~~~bash
python -m QuickCSF.simulate --help
~~~
