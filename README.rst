Timeflux Neurofeedback Inverse Gamepad
======================================

Overview
--------

This is an example Timeflux plugin that provides a few simple demonstration nodes. Use it as a template to develop your own plugins.

Installation
------------

First, make sure that `Timeflux <https://github.com/timeflux/timeflux>`__ is installed.

You can then install this plugin in the timeflux environment:

.. code-block:: shell

    $ conda activate timeflux
    $ pip install timeflux_example

Building the Timeflux Neurofeedback Inverse Gamepad
---------------------------------------------------

We have set up an autobuild process using GitHub Actions. You can download the pre-built executables from the GitHub Actions artifacts or the releases section of this repository.

Prerequisites
-------------

- `Conda <https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html>`__
- `Timeflux <https://timeflux.io/>`__
- `PyInstaller <https://www.pyinstaller.org/>`__

Instructions for Manual Build
-----------------------------

If you prefer to build the project manually, follow these steps:

1. Clone the repository:

.. code-block:: shell

    git clone https://github.com/YOUR_USERNAME/timeflux_neurofeedback_inverse_gamepad.git
    cd timeflux_neurofeedback_inverse_gamepad

2. Set up the environment:

.. code-block:: shell

    conda create -n timeflux python=3.8
    conda activate timeflux
    pip install timeflux

3. Install dependencies:

.. code-block:: shell

    # For Linux
    pip install -r requirements_linux.txt
    
    # For Windows
    pip install -r requirements_windows.txt

4. Build the executable:

.. code-block:: shell

    # For Linux
    ./pyinstaller_linux.sh
    
    # For Windows
    ./pyinstaller_windows.sh

Downloading Pre-built Executables
---------------------------------

For those who prefer to use the pre-built executables, follow these steps:

1. Go to the `Actions` tab of the repository on GitHub.

2. Select the latest successful workflow run from either `pyinstaller_build`, `pyinstaller_build_windows`, or any other relevant workflow.

3. Download the artifact from the workflow run.

Notes
-----

- Ensure you have the necessary permissions to run the scripts.
- Modify the `requirements.txt` and PyInstaller scripts as needed for your specific environment.

License
-------

This project is licensed under the AGPL-3.0 License - see the LICENSE file for details.
