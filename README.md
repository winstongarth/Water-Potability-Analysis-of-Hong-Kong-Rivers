Water Potability Analysis of Hong Kong Rivers.

This project analyzes water quality metrics from different water bodies and applies a machine learning model (Random Forest) to predict the potability of water samples taken from various rivers in Hong Kong.

Setup.
The following R packages are required:

dplyr,ggplot2,tidyr,lubricate, caret, lattice, and randomForest
The datasets used in this project are:

water_potability.csv: A global water quality dataset containing water quality metrics for 3276 different water bodies.
river-historical-1986_2020-en.csv: A dataset containing  water samples data from rivers in Hong Kong from 1986 to 2020.

Data Exploration and Visualization.
The script includes a comprehensive data exploration and visualization section. Histograms are generated for various water quality metrics such as pH, Hardness, Solids, Chloramines, Sulfate, Conductivity, Organic Carbon, Trihalomethanes, and Turbidity. Each of these metrics is visualized against the Potability variable to identify potential patterns or trends.

Random Forest Model.
A random forest model is trained to predict the potability of water using the variables pH, Solids, Turbidity, Conductivity, and Organic Carbon. The model is evaluated using a confusion matrix.

Local Hong Kong River Water Analysis.
Lastly, the trained model is used to predict the potability of water samples from rivers in Hong Kong. The data is first filtered for the year 2020 and then variables that match with the global water quality dataset are selected. After matching the variable names and data types, the random forest model is applied to predict the potability. The number of potable water samples is then counted.

Usage.
To run this analysis, clone the repository, ensure the required R packages are installed, and execute the script in an R environment. Make sure the path to the datasets is correct.

Results.
The result of this analysis will be a prediction of potability for each water sample in the Hong Kong dataset, which can be used for further research or water management purposes. The count of potable samples is also printed at the end of the script execution.

Note.
This project is for educational purposes and the results should not be used for making actual decisions regarding water quality or consumption.
