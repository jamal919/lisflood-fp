LISFLOOD-FP
===========

This repository contains the **LISFLOOD-FP model (version 5.9)** - forked from LISFLOOD-FP-BMI. 

LISFLOOD-FP
-----------

LISFLOOD-FP is a hydrodynamic model developed at the `University of Bristol`_. It solves the local inertia equation to simulate overland water flow using a regular grid.

.. _University of Bristol: http://www.bristol.ac.uk/geography/research/hydrology/models/lisflood/

Note: The here available LISFLOOD-FP model is based on version 5.9. The sole purpose of this repository is to study the model codes and functionalities. The BMI functionalities are not really intended at this moment, and thus turned off in the CMakeLists.txt. The source-code of the model, however, not the most up-to-date version. In case you are interested in using a open-source version of the model, this repositry may be suited for you. Otherwise, please consider contacting the `University of Bristol`. For LISFLOOD-FP related issues please contact `University of Bristol`. A reference to the recently published versoin can be found here - https://doi.org/10.5194/gmd-14-3577-2021.

Compilation
-----------

The learning purpose, the compilation of the model is changed from original gnu-make to Cmake. The basic compilation steps are following:

* Create a folder - `mkdir build && cd build`
* Run cmake - `cmake ../src`
* Build the - model `make`

Running models
--------------

The ``lisflood.exe`` (Windows) or ``lisflood`` (Linux) executable can be used to run the model from command line with ``lisflood [-v] model.par`` where ``model.par`` is your LISFLOOD-FP parameter file.

To run the model with the executable, shared object and the executable must be in the same directory as the model.par and all associated files.

License
-------

This specific LISFLOOD-FP version (v5.9) is licensed under GNU GPL 3.0. The LICENSE is copied over from original lisflood-fp-bmi repository. 

Referencing
-----------

If you are using this model or any derivation thereof for your work or research, please cite these two references.

.. [GLOFRIM] Hoch, J. M., Eilander, D., Ikeuchi, H., Baart, F., and Winsemius, H. C.: Evaluating the impact of model complexity on flood wave propagation and inundation extent with a hydrologic–hydrodynamic model coupling framework, Nat. Hazards Earth Syst. Sci., 19, 1723–1735, https://doi.org/10.5194/nhess-19-1723-2019, 2019.

.. [LISFLOOD-FP] Bates, P. D., de Roo, A. P. J.: A simple raster-based model for flood inundation simulation, Journal of Hydrology, 236, 54-77, https://doi.org/10.1016/S0022-1694(00)00278-X, 2000.

