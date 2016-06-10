# Compliant Joint Toolbox (CJT)
The Compliant Joint Toolbox (CJT) for MATLAB is being developed to ease the modelling and design of (compliant) robotic joints. The goal is to provide rapid iteration of different models and control architectures by providing a number of pre-built components with consistent interfaces, together with a set of tools to build new ones.

<a href="https://github.com/geez0x1/CompliantJointToolbox" target="_blank">https://github.com/geez0x1/CompliantJointToolbox</a>

**Authors:**

Jörn Malzahn

Wesley Roozing

## Getting started
1. To set up the required paths, run `setSEApaths.m`.
2. In the root of the toolbox, you will find the following directories:

    - `lib`: Simulink blocks that come with the library - controllers, models and observers;
    - `model`: Mathematical description of the various models and their components;
    - `param`: Parameter files for several example actuators;
    - `templates`: Templates used by the joint builder to build actuator classes;
    - `tools`: Various tools for calculating observers, gains, transfer functions and plotting;
    - `unit_tests`: Unit tests to verify correct functioning of the library.

3. The joint builder works using the well-known factory design pattern. This means it builds (almost) self-contained joint models with the requested parameters, models, and nonlinear components. Built joints are placed in the `build/` folder, and generated by the `jointBuilder` class. Try the joint builder by running `testJointBuilder.m`. This will build a number of joints based on various combinations of parameters and models.
4. Go to the wiki for a detailed description of the classes and to try some examples in both MATLAB and Simulink.