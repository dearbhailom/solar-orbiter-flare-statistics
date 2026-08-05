## **Week 9**

#### Tasks completed:
- Improved flare duration/start and end time estimations
- Repeated SEA with improved start times, also did aligning first peak in flare
- Remade correlation plots with improved durations

#### Results/Figures:
- ##### Improved duration method:
  - Smoothing with window size = 75
  - For start - finding difference >0.2 counts *and* following 20 points must be monotonically increasing
  - For end - when flare goes below mean count value (in *entire* flare timeseries file)
    
  - Examples:

    ![Flare duration example](./figures_for_reports/week_9/flare0.png)

    ![Flare duration example](./figures_for_reports/week_9/flare13.png)

    ![Flare duration example](./figures_for_reports/week_9/flare16.png)

    ![Flare duration example](./figures_for_reports/week_9/flare21.png)

    ![Flare duration example](./figures_for_reports/week_9/flare78.png)

- ##### Remade duration plots:

    ![Histogram of improved durations](./figures_for_reports/week_9/improved_durations_hist.png)

    ![Correlation plot of improved durations and peak counts](./figures_for_reports/week_9/improved_durations_peak_counts_vs_duration.png)

  - Spearman correlation coefficient = 0.2

    ![Correlation plot of improved durations and peak ratios](./figures_for_reports/week_9/improved_durations_peak_ratios_vs_duration.png)
    
  - Spearman correlation coefficient = -0.1

- ##### SEA:
  - SEA aligned to *first* peak in flare (using Scipy find_peaks with a prominence of 5% of the peak counts)
  - Start-aligned SEA redone with improved start times
  - All 3 methods extended to include 160 of the top 400 flares from flare list by 25-50 keV counts
    
  - Comparison of the three SEA methods:
   
    ![SEA for 25-50 keV energy range with three different methods of alignment](./figures_for_reports/week_9/sea_comparison.png)


[Back to list](index)
