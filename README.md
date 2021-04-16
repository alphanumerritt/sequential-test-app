# Sequential Testing Application
Use this application to plan and analyze sequential A/B tests. If you know what peeking is, you probably know you should not being doing it.

This application allows you to peek responsibly by adjusting test statistics to compensate for type 1 error inflation and then adjusting sample sizes to compensate for the corresponding loss in power.

## Features
- Sample size calculation
- Compare sample sizes with fixed horizon (non-sequential) test design
- Plot expected test duration by effect size
- Plot boundary crossing probabilities by effect size (like a power plot)
- Non-inferiority margin applied to control variant
- Adjusted boundary values for multiple testing scenarios (multiple variants or metrics)

## Version history
- v2.7 Apr 15, 2021
    - Fixed sample size reported when multiple comparisons is selected (reports by variant)
    - Power plot, sample plot, results table, and boundary plots now hide if multiple comparisons selected
    - Changed input for results checkpoint selector from a slider to a dropdown
    - Changed add2results and clear-results to buttons instead of text links
    - Fixed multiple comparison table...now displays all z-score columns instead of the ambiguous original only
- v2.6 Apr 14, 2021
    - Added fixed horizon sample size to plots 
- v2.5 Apr 14, 2021
    - Fixed bug with shortcut loading
    - Limited check-ins to 18, greater than 18 throws an error with gsDesign package (not certain why)
    - Optimization added for design creation code - no longer creates 2 designs by default, only when adding results
    - Added error message if there's ever a problem processing the test design, it won't crash the app
    - Added color to the boundary plot efficacy and futility areas
- v2.1 Minor updates to wording, some code simplifications, improvements to readme file, versioning added
  - Multiple comparisons input added to shortcut links, old links with results need to be updated
    - Old link without results: 95,80,10,10,1,0,10000,4,1000,7,
    - New link without results: 95,80,10,10,1,0,10000,4,1000,7,0,  Notice "0," added to end for the new input
    - Old link with results: 95,80,10,10,1,0,10000,4,1000,7,1|100|1000|110|1000|0.73
    - New link with results: 95,80,10,10,1,0,10000,4,1000,7,0,1|100|1000|110|1000|0.73  Notice "0," added mid-string
- v2.0 Released October 2020.  
- v1.0 Released some time in May 2020.  
