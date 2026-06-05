## **Week 1**

#### Tasks completed:
- Read up on Solar Orbiter, STIX, and the major flare campaigns
- Set up miniforge and install Stixpy and Sunpy
- Set up a Github repo
- Completed Sunpy tutorial and practiced getting lightcurves from STIX and GOES
- Used the STIX flare list to select interesting events and compare their STIX and GOES lightcurves

#### Results/Figures:
- I practiced getting a lightcurve for two different flares, on using STIX data and one using GOES

<figure>
    <img src="/figures/week 1/stix_20200607_2130.png"
         alt="stix flare 2020 june 7th">
</figure>

<figure>
    <img src="/figures/week 1/goes_20240514_singleflare.png"
         alt="goes flare 2024 may 14th">
</figure>
  
- I loaded the STIX flare list and filtered it to only include those seen by GOES, and selected the largest flare, the smallest flare, an M class flare, and a flare which I noticed didn't have a GOES class for further examination.
- I got both STIX and GOES lightcurves for each flare.
    - Large Flare:
      
    <figure>
        <img src="/figures/week 1/stix_flarelist_largeflare.png">
    </figure>
    
    <figure>
        <img src="/figures/week 1/stix_flarelist_largeflare_goes.png">
    </figure>
    
    - Medium Flare:
      
    <figure>
        <img src="/figures/week 1/stix_flarelist_mflare.png">
    </figure>
    
    <figure>
        <img src="/figures/week 1/stix_flarelist_mflare_goes.png">
    </figure>
      
    - Small Flare:
      
    <figure>
        <img src="/figures/week 1/stix_flarelist_smallflare.png">
    </figure>

    <figure>
        <img src="/figures/week 1/stix_flarelist_smallflare_goes.png">
    </figure>
 
    - No GOES Class:
      
    <figure>
        <img src="/figures/week 1/stix_flarelist_nogoesclass.png">
    </figure>
    
    <figure>
        <img src="/figures/week 1/stix_flarelist_nogoesclass_goes.png">
    </figure>
 

- Plotting the GOES data for the unclassed flare, it looks like it should be in the X7-X8 range
- For the three larger flares, I noticed sudden very sharp increases in the lower energy ranges shortly after the main flare event - this is due to the presence of the attenuator affecting how the lower energy ranges are detected
- The smallest flare does not have a clear peak in the GOES data - this means it was probably too small to be clearly distinguished from background solar radiation by GOES
- I also marked in vertical lines where the peak time was given by the STIX flare list. This shows the time offset in the two data sets -  the peak line from the STIX data appears in the range of a few minutes earlier than the GOES peak due to the distance from Solar Orbiter to Earth
