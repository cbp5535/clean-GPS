# clean-GPS
Purpose: A systematic method for cleaning GPS device data for studies and data collection efforts in tourism and recreation destinations. 

**Background:** Over recent years, there has been substantial growth in the use of GPS devices for research in recreation and tourism, but there is no standardized, published procedure for cleaning that data. Typically, these projects involve recruiting hundreds of visitors at destinations to carry GPS devices with them throughout their trip that record waypoints at regular intervals. Recruited participants then drop those devices off, either with a researcher or at a dropbox. While the data from these studies is valuable, cleaning that data can be difficult and time-consuming

**Purpose and file structure:** We present open-source Python code that automates downloading GPS device data to ArcGIS Pro, establishes boundaries for excluding data, and provides parameters for extracting erroneous points (labeled "Clean_GPS_Tracks.ipynb"). This repository includes example code, which was used to clean data from a random sample of visitors to Grand Canyon National Park (labeled "GRCA_Clean_Tracks") and supporting shapefiles (GRCA_Boundaries.zip). Unfortunately, no GPS data can accompany this code due to privacy concerns, but you may test the code with simulated data or simply try it with your own GPS data in your own study site. 

The code is not tailored for maximum efficiency, however, it runs in 20 minutes on a 16GB i7 processor on dataset of 246 tracks and 7,373,971 waypoints. Instead, the code is meant to be easy to follow for a non-technical audience who has familiarity with using ArcGIS and is comfortable navigating Jupyter notebooks for Python. If you are not familiar with using Python/Jupyter notebooks, I recommend using the built-in "notebooks" function in ArcGIS to run the code.

**Versioning:** This code is intended to be run in Python 3.9 using dependencies for ArcGIS (2.3.0.3). It relies heavily on Arcpy (3.1.2) and Pandas (1.4.4). 

**Authorship:** This code was written by Colby Parkinson based on a procedure by Dr. Will Rice with supervision from Dr. Bing Pan. If you use the code or publish analysis that you performed informed by the code or procedure provided in this GitHub, please cite:

Parkinson, C., Rice, W. L., & Pan, B. (2024). Standardizing the Procedure for Cleaning GPS Device Data for Recreation and Tourism Research Travel and Tourism Research Association 54th Annual International Conference, Burlington, VT. 


Below is the published paper that provided the most helpful information for creating this code and informing the overall procedure:

Hallo, J. C., Beeco, J. A., Goetcheus, C., McGee, J., McGehee, N. G., & Norman, W. C. (2012). GPS as a Method for Assessing Spatial and Temporal Use Distributions of Nature-Based Tourists. Journal of Travel Research, 51(5), 591-606. https://doi.org/10.1177/0047287511431325 
