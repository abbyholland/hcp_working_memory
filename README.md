# hcp_working_memory
This features my work for neuromatch academy! The open-source hcp dataset was used to identify the regions responsible for working memory in fMRI data.

The biggest challenge with the hcp data was understanding the data structure and how to work with the data at a basic level. The second main obstacle was that this big of a dataset uses a considerable amount of space and is therefore challenging to run on a computer (I have a mac which is undesirable in this context). 

A few important things: 
- The rest data in this dataset is only from 1/4 runs so is significantly less than we'll actually be using! Dante is working on the averages for the rest data so that they are directly comparable with the wm data! 
- The structure of the code has changed such that one of the code parcels, hcp_load, is just doing a basic loading and processing of the data to then be saved into a csv (this section can be done by people who's computers can handle it). The second script is hcp_analyze and that is where the pca is done, graphs are printed, processing is applied, etc! 

The goal is that the load data can handle separating the data into trial/test sets, conduct initial processing, and save the dataframe. The second script can then be worked on separately with lesser data, so work can be done with a lesser quality dataset while the data is being worked on by other people in the first script. 
