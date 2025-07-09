# Time-Series-Forecasting

Kristan Böttjer (11422684)


The repository is structured as follows:
For each model there is a notebook which consists of the model function and a basic evaluation with just a simple train test split.
In the end of each model notebook a cross validation is performed. Generally we tried to find one function which captures the design decisions one would make
manually. In the end we compare all models in the results notebook where you can see all models side by side.


General remarks:
For the Australian Electricity dataset. We used the data of the state of Victoria only. Also we aggregated it to daily data 
as hourly otherwise it was too much data. In Hindsight we could have also jsut reduced the number of data points to keep the diverstiy of frequencies. 
. The Car Parts dataset was also aggregated. Here we just used the sum of all shops so grouped by date.
