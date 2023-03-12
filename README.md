# GMD-classification
Galician Muiñeira Dataset: The only (as of 1/03/2023) dataset of muiñeiras

Hello!

Short summary of the csv files here:

The csv files with id and name of the score (id corresponds to the name of the corresponding xml file)
for galician_musicxml_located we also have the location available 

* galician_musicxml_full.csv
* galician_musicxml_located.csv

Inside features folder:

* data.csv
* data_located.csv

These are the fully processed data files with all the features we extracted, both for the full dataset
and the subset we used for the located songs. These csv files contain this data:

* id: The int id that corresponds to the musicxml file in the data folder.
* name: The name of the muineira.z
* key: The key of the muiñeira.
* time_signature: The time signature of the muineira.
* ratio_negras_corcheas: The quarter to eighth ratio in the muiñeira.
* muiñeira_type: Value C1 or C2 depending on the structure of the muiñeira.
* location: The location of the muiñeira in only one row. (Only in data_located.csv)
* lat: Latitude coordinat of the location. (Only in data_located.csv)
* lon: Longitude coordinat of the location. (Only in data_located.csv)
* classification: The classification for the given muiñeira. Can be A Coruña, Rias Baixas, Ancares, Costa do Morte, Courel, A Fonsagrada or Not classified.



## Reproducibility
Now for reproducibility's sake:

To extract all the scores from Folkoteca Galega, you first want to run galician_scraping.ipynb
(make sure the folder you want to store the scores in doesn't contain the files already), after this, you want to move the
feature_extraction.ipynb to the data folder and run it, if you have the paths set up properly,
it will return data.csv and data_located.csv, move all these new files to the features folder (or prepare your own correct paths)

Now to get the final results, just run data_visualization.ipynb, you will get both the final
data_located.csv and the visualization of all the data.

Moitas grazas / Munches gracies!
