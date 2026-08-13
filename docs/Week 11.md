## **Week 11**

#### Tasks completed:
- Categorisation of flares by peak number and Pearson r
- Found approx. FWHM of pulses (Scipy peak_widths), rise/decay times, peak separations
- More flare statistics and correlation plots

#### Results/Figures:
- ##### Flare categorisation: 
  - Categorising flares into **simple** (<3 peaks or Pearson r with SEA median >0.7) or **complex** (3+ peaks or Pearson r with SEA  median <0.7), there are ~90/150 flares that both methods agree on.
 
  - *An agreed simple flare:*
    
  ![An agreed simple flare](./figures_for_reports/week_11/simple_flare.png)

  - *An agreed complex flare:*
  
  ![An agreed simple flare](./figures_for_reports/week_11/complex_flare.png)

  - *A mixed flare: High correlation, but many peaks*

  ![A not agreed flare](./figures_for_reports/week_11/mixed_flare1.png)

- ##### Pulse FWHM and separation:
  - I used Scipy peak_widths at a relative height of 0.5 as the simplest way to assess a proxy FWHM over a large sample of pulses, and took the pulse separation as simply the distance between peaks found by Scipy find_peaks. 

    ![Example of pulse widths and separation](./figures_for_reports/week_11/flare_fwhm_example.png)

  - Using this method gives a mean peak width across all flares of 32.5 seconds, which agrees well with the FWHM of the SEA median flare of 29.4 seconds.
 
- ##### Statistics and correlation plots:
  - I collected flare duration, rise and decay time, peak counts, peak ratio, mean peak separation and FWHM, number of peaks, and Pearson r correlation with the SEA into a dataframe and made some plots with this.
  - *Number of peaks*:

    ![Histogram of number of peaks per flare](./figures_for_reports/week_11/peak_hist.png)
    
  - *High correlation:* The following three plots showed some of the highest levels of correlation, and similar plots were included in Alexander Warmuth's slides for the STIX workshop, showing very similar results for a different set of flares.

    ![Peak separation vs flare duration](./figures_for_reports/week_11/peak_dist-duration.png)
    
    ![Peak FWHM vs flare duration](./figures_for_reports/week_11/fwhm-duration.png)

    ![Peak FWHM vs peak separation](./figures_for_reports/week_11/fwhm-peak_dist.png)

  - *Other plots:* 

    ![Rise vs decay time](./figures_for_reports/week_11/rise-decay.png)

    ![Rise:decay vs duration](./figures_for_reports/week_11/rise_decay-duration.png)

    ![Duration vs number of peaks](./figures_for_reports/week_11/duration-peak_no.png)

    ![Maximum flare counts vs number of peaks](./figures_for_reports/week_11/peak_max-peak_no.png)

[Back to list](index)
