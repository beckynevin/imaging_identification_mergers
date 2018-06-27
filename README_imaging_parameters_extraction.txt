June 27, 2018
Rebecca Nevin

The purpose of this code is to extract various imaging predictors from simulated images. I will also post the code that generalizes this to observed MaNGA galaxies.

It extracts the following seven parameters in additional to projected separations (if there are >1 stellar bulges) and places them nicely in a data table along with the galaxy ID:

Gini
M20
Concentration
Asymmetry
Clumpiness/Smoothness
Sersic index
Shape Asymmetry

It uses the following software packages:
1. Galfit
2. Source Extractor
3. Statmorph
