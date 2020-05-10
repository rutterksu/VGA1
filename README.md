# VGA1
Author: Bryan Rutter
Date: 10-May-2020
Email: rutter@ksu.edu

# Description

Implementation of Van Genutchen and Alves analytical solution to the 1-D convective-dispersive solute transport equation.

This function evaluates the solution:

$$
C(z,t)=C<sub>i</sub>+(C<sub>o</sub>-C<sub>i</sub>)A(z,t)
$$

where

$$
A(z,t) = \frac{1}{2} erfc \left( \frac{Rz</sub>-vt}{\sqrt{4DRt}} \right) + \frac{1}{2} exp \left( \frac{vz}{D} \right) erfc \left( \frac{Rz+vt}{\sqrt{4DRt}} \right)
$$

where

__z__ = the soil depth (L)  
__t__ = elapsed time (T)  
__v__ = the mean pore velocity  
__R__ = the _retardation factor_ (dim); defined as $R = 1+ \frac{\rho<sub>b<\sub> K<sub>d</sub>}{\theta}$  
__D__ = the apparent, or effective, dispersion coefficient (L<sup>2</sup> s<sup>-1</sup>); defined as $D = \xi \left( \theta \right) D_0 + \lambda v^{n}$
__\xi(\theta)__ = the tortuosity factor; defined as $\xi \left( \theta \right) = \frac{\theta^\frac{7}{3}}{\theta^2_s}


