# VGA1
Author: Bryan Rutter
Date: 10-May-2020
Email: rutter@ksu.edu

# Description

Implementation of Van Genutchen and Alves analytical solution to the 1-D convective-dispersive solute transport equation.

This function evaluates the solution:

![C(z,t)=C_{i}(C_{o}-C_{i})A(z,t)](https://render.githubusercontent.com/render/math?math=C(z%2Ct)%3DC_%7Bi%7D(C_%7Bo%7D-C_%7Bi%7D)A(z%2Ct))

where

![A(z,t) = \frac{1}{2} \text{erfc} \left( \frac{Rz-vt}{\sqrt{4DRt}} \right) + \frac{1}{2} \text{exp} \left( \frac{vz}{D} \right) \text{erfc} \left( \frac{Rz+vt}{\sqrt{4DRt}} \right)](https://render.githubusercontent.com/render/math?math=A(z%2Ct)%20%3D%20%5Cfrac%7B1%7D%7B2%7D%20%5Ctext%7Berfc%7D%20%5Cleft(%20%5Cfrac%7BRz-vt%7D%7B%5Csqrt%7B4DRt%7D%7D%20%5Cright)%20%2B%20%5Cfrac%7B1%7D%7B2%7D%20%5Ctext%7Bexp%7D%20%5Cleft(%20%5Cfrac%7Bvz%7D%7BD%7D%20%5Cright)%20%5Ctext%7Berfc%7D%20%5Cleft(%20%5Cfrac%7BRz%2Bvt%7D%7B%5Csqrt%7B4DRt%7D%7D%20%5Cright))

where

__z__ = the soil depth (L)  
__t__ = elapsed time (T)  
__v__ = the mean pore velocity  
__R__ = the _retardation factor_ (dim); defined as R = 1+ \frac{\rho<sub>b<\sub> K<sub>d</sub>}{\theta}
__D__ = the apparent, or effective, dispersion coefficient (L<sup>2</sup> s<sup>-1</sup>); defined as $D = \xi \left( \theta \right) D_0 + \lambda v^{n}$
__\xi(\theta)__ = the tortuosity factor; defined as $\xi \left( \theta \right) = \frac{\theta^\frac{7}{3}}{\theta^2_s}


