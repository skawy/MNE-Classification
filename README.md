# MNE-Classification
This models classify the sleep stage to the person based on his brain`s signal

> MMN Is An Open-source Python package for exploring, visualizing, and analyzing human neurophysiological data
>
> I am using only EEG signal 

### Used Feature File 

- Describing the data used from the MNE

- Plotting the features we extract from the epoch

  >  **Epoch**: a period of time in the signal 

- I classify any epoch to know at what is the current sleep stage in the given period or *epoch*
- We have 2 EEG signals that is why any feature has 2 plots

### Models File

- I am using the epochs of 16 persons as a train data and 5 persons  as a test data

- Every person signal has 714 epoch but in 2 EEG channels 

  > we are cutting the signal into epochs 
  >
  > the 2 channels at any given have the same sleep stage

- Then we flatting the epochs from the 2 channels to get 1 array of 1428 
- Calculating 8 feature then we get  ( 1428 * 8 ) for the single person 
- Like I said before at any epoch the 2 channels have the exact sleep stage or **label** then I duplicated it

### ![labels](E:\Faculty\FCAI\4th Year\First Semester\BCI\Assignments\Assignment 2\Github Version\MNE-Classification\Images\labels.jpg)

now I am having features and labels for any person then I can train any model and predict the sleep stage of any epoch

