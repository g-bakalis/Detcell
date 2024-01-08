## General Information
Detcell is an Artificial Neural Network Model trained to predict the detonation cell size.
The model was trained and tested using experimental detonation cell size data, combined with the corresponding 1-D ZND parameters.

For further information on the model and to cite this code, please refer to: https://www.sciencedirect.com/science/article/pii/S2666052022000346.

Newer versions of the original 3 input feature ANN model or models with different input features can be found at:
- https://github.com/g-bakalis/detcell
- https://users.encs.concordia.ca/~hoing/index.html

## Running the code
There are currently two jupyter notebooks (.ipynb) that are provided to run the code. For the V1_ANN_manual, the user provides the 3 input features to the relevant field in the notebook to  get a single prediction. For the V1_ANN_csv, the user has to provide the input features in a .csv file, simply created from an excel file saved as .csv. Multiple rows of data can be used to get to get multiple predictions at the same time. An example csv is provided. It is required to keep the first row with the column titles.  The output is located at the jupyter notebook.

It is also possible to run this code online without installing any code using mybinder: 
https://mybinder.org/v2/gh/g-bakalis/detcell/HEAD

## Model Inputs and outputs
### Inputs
As inputs, the following ZND parameters are necessary:
- The Mach number
- The Induction length(cm)
- The maximum thermicity Sigma (1/sec)

### Output
- The detonation cell size (mm)
