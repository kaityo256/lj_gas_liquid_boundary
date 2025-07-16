# Gas-Liquid Phase Boundary of Lennard-Jones System

This data provides temperature Gas-Liquid Phase Boundary of Lennard-Jones System.

- Cutoff is 3.0 sigma.
- Each file contains 7 columns, temperature, density of gas, its err, density of liquid , its err, lambda (thickness of gas-liquid phase interface), its err, respectively.
- File name corresponds to the system size. E.g, gl_L128.dat is the data of the system with L = 128, etc.

If you have gnuplot, then you can plot gas-liquid binodal line as follows,

```txt
p "gl_L128.dat" u 2:1:3 w e,"gl_L128.dat" u 4:1:5 w e
```
