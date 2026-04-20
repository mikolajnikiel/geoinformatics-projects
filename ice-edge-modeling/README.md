# Antarctic Sea Ice Extent Modeling

A project developed as part of the Geoinformatics degree program at AGH University. The script analyzes daily sea ice extent data and uses the `SciPy` library to fit trigonometric functions, creating a continuous mathematical model for each meridian.

##  Technologies and Tools
* **Python** (Pandas, NumPy)
* **Spatial Analysis & Mapping:** GeoPandas, Shapely, Cartopy
* **Mathematics:** SciPy (`curve_fit`)
* **Visualization:** Matplotlib (including `.gif` animation generation)

##  How the Model Works
For each of the 360 meridians, the script fits a sinusoidal curve to historical data using the following function:

$f(t) = A \cdot \sin(B \cdot t + C) + D$

Where `t` is time, and the fitted parameters allow for simulating and predicting ice extent over time. The modeled coordinates are then transformed into polygons (Shapely) and projected onto a map using an orthographic projection via Cartopy.



