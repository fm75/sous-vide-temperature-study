# sous-vide-temperature-study
Analysis of Temperatures of Meat Being Cooked Sous Vide

# Sous Vide Cooking
In sous vide cooking, meat is cooked in a container in which most or all of the air
has been eliminated, either via vacuum sealing or using the water displacement method.

# Data Exploration and Data Wrangling
The experimental data comes from experiments performed by Rick Garcia. In the experiments, 
some food was cooked sous vide in a water bath. Temperatures of the food and the water
bath were recorded using a Tappeque four probe wifi thermometer. The raw data included
many columns of data that was not needed, including the experimenter's email addres
Each row in the source CSV file included the results from a single probe. 

For privacy purposes, the raw data has not been included in this repo.

The DataWrangling notebook was used to transform time and temperature data into elapsed time
and temperatures, merging the data from the "meat" probe and the water bath probe. These
data were stored in a CSV file containing the elapsed time and the two temperatures. 
The transformed data are stored in a file with a naming convention:

    foodtype-thickness-units.txt

For example: TBone-1.inch.txt

# Experimental Analysis
* AnalyseGraphically-bqplot - Graphical display of results using `bqplot`.
* AnalyseGraphically-matplotlib - Graphical display of results using `matplotlib`.
