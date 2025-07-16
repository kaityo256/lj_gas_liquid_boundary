# Gas-Liquid Phase Boundary of Lennard-Jones System

## Summary

This dataset provides the temperature-dependent gas-liquid phase boundary of the Lennard-Jones system. The cutoff radius is set to 3.0 sigma. Since we adopted a somewhat uncommon method for implementing the cutoff, please refer to our paper for details.

## Data

[Data Directory](data)

Alternatively, you can download a ZIP archive:

[ljphasediagram.zip](ljphasediagram.zip)

Each data file contains seven columns:
temperature, gas density, error of gas density, liquid density, error of liquid density, interface thickness (lambda), and error of interface thickness, respectively.

The filename indicates the system size. For example, `gl_L128.dat` corresponds to a system with dimensions (128, 128, 256).

You can plot the gas-liquid binodal line using Gnuplot as follows:

```txt
p "gl_L128.dat" u 2:1:3 w e,"gl_L128.dat" u 4:1:5 w e
```

This will generate the following graph:

![ljphasediagram.png](ljphasediagram.png)

## Reference

For details of the simulation method, see the following paper:

* Phase diagram and universality of the Lennard-Jones gas-liquid system
    * Hiroshi Watanabe, Nobuyasu Ito, and Chin-Kun Hu
    * [J. Chem. Phys. 136 204102 (2012)](https://doi.org/10.1063/1.4720089)
    * [arXiv:1202.5369](https://arxiv.org/abs/1202.5369)

## LICENSE

This work is licensed under [CC BY](https://creativecommons.org/licenses/by/4.0/).
