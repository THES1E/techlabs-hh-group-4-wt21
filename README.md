# Crime in London

## Data
- Which data did we use?
 We used the London Crime data: https://data.police.uk/data/
  - We used the datasets from Metropolitan Police Service, City of London Police and British Transport Police. 
  - Which data? The time frame is set from November 2020 to November 2021. and then downloaded to the local machine.
  - Which format? The data was downloaded as a .csv file and stored as such.

## Execute Code
- What should be done to execute the code? 
  To execute the code, install Jupyter Notebook with Pandas 3.0. Ensure to have the following libraries installed:
  - Pandas
  - Matplotlib
  - NumPy
  - Seaborn
  - Glob
  - Folium
 
Run the code in a kernal that supports these libraries.

First, clone our repository with the folder structure onto your machine. The data download from the website of the British Police Service will produce one folder for each month downloaded. So after downloading the data, make sure, to copy all subfolders (13 folders) into the data folder of our project that you have cloned from GitHUb to your local machine. After this step run the notebook "prepocessing_data" that you find in the src folder of our project. This will add all .csv files into one dataframe, clean the data of spelling mistakes, add a location type and a season to the dataframe and produce a new .csv file. This .csv file called "preprocessed_data" will be automatically saved in a subfolder called preprocessed in the data folder when you run the code.

Next, open the notebook "analysis". There as a first step the previously created .csv file "preprocessed_data" will be read in as the dataframe. Then run all cells in an environment with the same specifications as above. This will filter, group and anlyse the data and will produce pivot tables, graphs and plots that can help to draw conclusions from the data and find new ways to look at the data, ask new questions and further investigate.

The last notebook you need to run is called "map" and it reproduces our final solution, an interactive map that is created with folium. IMPORTANT: Make sure that at the beginning you have to trust this notebook otherwise the code that is producing the map won't go through. When you use Jupyter you have to go to File and then click Trust Notebook. Also don't be alarmed when it takes some time to run the code, the dataset is - although there are some filtering steps before again - quite big for folium. In the end you should see a zoomable map with markers that you can click on to find out the crime type of that crime spot. The last code in that notebook creates an .html file to open the map in a browser instead of showing it in a notebook.

  
## Graphs/Results
The graphs and plots that are created with the "analysis" notebook give already a good understanding about the crime situation in Greater London, e.g. how the number of crimes varies during the different seasons, which crime types are committed more in which locations and which last outcomes were more common than others. Our final solution is the interactive map that shows the crime locations on street level and therefore gives people the opportunity to avoid those areas.


