Title: Data for "Simulating Land Use Change with Neural Cellular Automata"

1. Folder description:
01_Raw_Data: The source of the original dataset. The data includes 2000, 2005, 2010, 2015, and 2020 land use and driving factors (DEM (extracting Slope and Elevation), GDP, POP, Rain, Tem, Way (extracting Highway and Railway)) raster data. These were obtained from the Resource and Environmental Science Data Platform (https://www.resdc.cn/) and OpenStreetMap (https://www.openstreetmap.org/)
02_Processed_Data: The cleaned dataset for analysis. Data processing was conducted to obtain raster data of land use and various driving factors for Guangdong Province over multiple years. The "Guangdong-Boundary" folder contains boundary elements of Guangdong Province, the "Guangdong-driving" folder contains eight types of driving factor data for Guangdong Province over multiple years as well as the processing process, and the "Guangdong-LU" folder contains land use change data for Guangdong Province and the processing process.
03_Model_Input: Driving factor raster. Contains the ".txt" data corresponding to the land use and driving factors of Guangdong Province over multiple years after processing in step 02_Processed_Data.
04_Model_Output: Simulation results. The "model_parameters" contain the corresponding optimal parameters of ST-NCA and all other models; the "Simulation prediction results-txt" folder contains the results of all model simulations of LUCC in 2020".txt" data, and also includes the prediction results of LUCC in 2025 achieved by ST-NCA. The "Confusion matrix" contains the confusion matrices of the simulation results of different models.
05_Code: Model implementation code. The main dependent libraries are as follows,
 - tensorflow
- tensorflow.keras
- numpy
- scipy
- pandas
- scikit-learn (sklearn)
- spectral
- geopandas
- Pillow (PIL)
- matplotlib
- plotly - argparse
- random
- time
- sys
- os

2. Data description:
As the input data for the model, the ".txt" format data in the "driving" folder of the "03_Model_Input" folder represents various driving factors for the corresponding year. The ".txt" format data in the "LU" folder represents LUCC in different periods.

3. Coordinate system:
All raster data are in the WGS84 coordinate system with a resolution of 1 kilometer.

4. How to reproduce:
All model operations are the same. Run the files with the suffix ".ipynb" in the "05_Code" folder using Jupyter Notebook.

5. Contact:
houk431@nenu.edu.cn