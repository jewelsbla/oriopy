<p align="center">
  <img src="https://github.com/jewelsbla/oriopy/blob/main/images/oriopy_logo.png">
</p>

***
[![PyPI version](https://badge.fury.io/py/oriopy.svg)](https://badge.fury.io/py/oriopy)
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

OrioPy is a Python package to interpolate fiber orientation tensors (or tensors of any kind for that matter) of second or fourth order. Both methods make use of the fact that symmetric positive definite tensors can be decomposed into eigenvalues and eigenvectors in spectral decomposition. In terms of the visualization of tensors in the form of tensor glyphs, the eigenvalues are responsible for the shape, while the eigenvectors are resposible for the orientation of the tensor in space.

In case of the tensors of fourth order, these eigenvalues and eigenvectors (in the form of the rotation matrix R) are directly weighted according to Shepard's inverse distance weighting, interpolated separately and then recomposed into a tensor.

In case of the orientation tensors of second order, instead of the eigenvalues another group of invariants, so-called orthogonal invariants, are used. The eigenvectors are also recalculated to quaternions and then interpolated. The reasons for this 
detour is explained in the paper mentioned above.



This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg