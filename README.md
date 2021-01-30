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
- v2.1 Minor updates to wording, some code simplifications, improvements to readme file, versioning added
- v2.0 Released October 2020
- v1.0 Released some time in May 2020
