This repository contains the data, notebook and outputs for the Optical Detector assignment.
The repository is structured as follows:
- _hst-aligned_: this folder contains the aligned fits files of the 3 F336W observation, which were compared to the one calibrated by the _hst-assignment.ipynb_ pipeline.
- _hst-calibration_: this folder contains three subfolders
  - _ubai2505m_
  - _ubai2507m_
  - _ubai2508m_
  Each of these folders contains all the fits (atodfile, biasfile, blevfile, darkfile, flatfile, maskfile, rawfile) files for the corresponding observation, used by _hst-assignment.ipynb_ for the calibration pipeline.
- _hst-processed_: used to store the output of the _hst-assignment.ipynb_ calibration as side by side plots.
- _sentinel-data_: stores all the data used for the  _sentinel-assignment.ipynb_ computations, which are stored in four separate subfolders:
  - _S2_2017-07-12_
  - _S2_2018-07-12_
  - _S2_2019-07-12_
  - _White-light_
  Three of the folders contain the TIFF files from Sentinel2, one for each of the observation, which were used to compute the vegetation area as a function of time; the _White_light_ contains the Google Earth images, used for the land area over time computation.
- _sentinel-processed_: conntains the output plots from _sentinel-assignment.ipynb_.
- _hst-assignment.ipynb_: Jupyter notebook with the functiosn and pipeline to run the calibration of the hst observation and compare the calibrated output to the aligned files.
- _sentinel-assignment.ipynb_: Jupyter notebook with the functions and pipeline to calculate the land and vegetaion area over time for the Google Earth and Sentinel2 images.
