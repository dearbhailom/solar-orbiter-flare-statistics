# solar-orbiter-flare-statistics

Statistical exploration of Solar Orbiter STIX flare observations. Summer internship at DIAS, June to August 2026. 

## Goal 
Work towards a picture of what a typical STIX flare looks like, using the STIX science flare list, quicklook lightcurves and science spectrogram data. Build up general statistics for the flare list, and focusing on hard X-ray signals for the largest flares in HXR, look at flare shape, properties and an 'average' STIX flare using superposed epoch analysis.

## Structure 
- notebooks/
    - code testing + analysis/ rough testing and evolving analysis notebooks
    - reference code/ tidied functions and important workflows
- figures/ saved plots 
- data/ local data (flare list), not tracked by git 
- docs/ weekly reports & other documentation

## Data 

- STIX science flare list: https://github.com/hayesla/stix_flarelist_science 
- STIX quicklook lightcurves and science spectrogram data via stixpy 
- GOES XRS lightcurves via sunpy
