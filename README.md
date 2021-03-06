"# BrainVisionRDA_numericalIdentifiers" 

This project addresses sync issues of markers from the BrainVision RDA interface streamed to LSL (https://github.com/sccn/labstreaminglayer) via the BrainVisionRDA app (https://github.com/sccn/labstreaminglayer/tree/master/Apps/BrainProducts/BrainVisionRDA) - namely the fact that those markers don't get de-jittered properly and, thus, are out of sync with the EEG data. 

This project part addresses the problem by introducing a temporary marker identifier channel in the EEG data allowing for the transmission of the corresponding EEG time stamps on to the markers in question. This post-processing is performed by an updated version of LSL's Matlab Importer (https://github.com/sccn/labstreaminglayer/tree/master/Apps/MATLABImporter) hosted here: https://github.com/otraupe/MATLABImporter_BVRDAnumericalIdentifiers.
