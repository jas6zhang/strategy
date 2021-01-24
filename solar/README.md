# Solar

Directory for solar models which predict and calculate energy obtained from solar panels based on API data.

## In this directory

+ `tests` directory
+ `calculation-angles-cell.py`: Script to calculate the angle per cell from the solar array, as given by keyboard inputs and written into `MSXIV-Strategy-Cell-Angles.csv`
+ `cell.py`: Class for a single Solar Cell, tracking efficiency of energy conversion from solar to electrical
+ `MSXIV-Strategy-Cell-Angles.csv`: Generated by `calculation-angles-cell.py`
+ `solar_array.py`: Class for Solar Array, reading from `MSXIV-Strategy-Cell-Angles.csv` for cell information and calculating energy for each for some solar day (see `solar.py`)
+ `solar.py`: Class for Solar day, representing a day given latitutde, longitude, timezone, and cloudiness and calculating energy obtained