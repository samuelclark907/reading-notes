## Data Visualization

### Matlibplot

- matplotlib is probably the single most used Python package for 2D-graphics.

- It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.

#### Simple Plot

- In this section, we want to draw the cosine and sine functions on the same plot. Starting from the default settings, we'll enrich the figure step by step to make it nicer.

The first step is to get the data for the sine and cosine functions:

import numpy as np

X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
C, S = np.cos(X), np.sin(X)
X is now a NumPy array with 256 values ranging from -π to +π (included). C is the cosine (256 values) and S is the sine (256 values).

To run the example, you can download each of the examples and run it using:

$ python exercice_1.py

[Bokeh Tutorial](https://mybinder.org/v2/gh/bokeh/bokeh-notebooks/master?filepath=tutorial%2F00%20-%20Introduction%20and%20Setup.ipynb)
[Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)
