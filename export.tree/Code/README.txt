 

I'm trying to figure out where to start here so I can build my own MEG pipeline for the PD project:

Y:\EEG_Data\REWARD_RO1\Data\Aim_2\scripts\MEG_Scripts\For_Upload

Many of these look like CARC batch scripts.   

Which MNE script do I start on?
---------------------------------------------

Either ERF_preprocess.py or source_preprocess.py.  

ERF* aligns to the device origin so that the sensor ERF can be taken and also generates an individual ERF.  

source* leaves the head where it is and the whole individual ERF section is removed. 

It's easy enough to merge the two scripts, or there's a toggleable version from the TMS project at: /Volumes/crcl/EEG_Data/CAVANAGH/REWARD_TMS/scripts/MEG_scripts/STEP1_MEG_preproc_REWARD_TMS.py