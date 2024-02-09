This repository shows how we can predict seasonal trends using ARIMA. ARIMA stands for AutoRegressive Integrated Moving Average.
## Installation
First step in installing is
```bash
git clone https://github.com/DamianBisewski/ProjektProgramowanieDane
```
After that, in order to install all the required dependencies, the user has to run
```bash
pip3 install -r requirements.txt
```
or
```bash
pip install -r requirements.txt
```
## Running the code
As the code is written in a Jupyter notebook, it's most convenient to use such a notebook.
```bash
jupyter lab
```
After that, in the left-hand bar there will be the **arima_temperature_forecasting.ipynb** file. We open this file.
Firstly, we read the provided CSV dataset and start with choosing the country for which we want to display and predict average monthly temperatures.
After that, two graphs are displayed - the first showing average temperatures of months belonging to the period we want to see (by default Jan 2003 - Aug 2013), the second showing differences between months and the same months a year prior.
Ultimately, there comes the ARIMA predicting itself. The user can customize the displayed graph. By default, the graph shows actual data from January 1990 to December 2011 and predictions with actual data from January 2012 to August 2013.
There are several parameters of the seasonal ARIMA, they are all described in the notebook below the cell with the ARIMA predicting. All of them are customizable. By changing the values of them, the user can try to find the optimal values of these parameters. The mean RSME value is displayed alongside the graph with the ARIMA prediction. It shows us how accurate the prediction is.
