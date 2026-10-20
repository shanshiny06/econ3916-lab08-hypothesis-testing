# econ3916-lab08-hypothesis-testing
# Hypothesis Testing — Is Job Training Worth It?

## Objective
I tested whether the National Supported Work (NSW) job training program raised participants' 1978 earnings, and whether the effect still holds in subgroups after correcting for multiple comparisons.

## Methodology
- I loaded the LaLonde NSW job training experiment, which covers 445 people: 185 trainees and 260 controls.
- I ran a one-sample t-test and a two-sample Welch's t-test on 1978 earnings.
- I wrote Welch's t-statistic as my own function, `welch_t()`, and checked its results against scipy on the full sample and on five subgroups.
- I computed Cohen's d to judge how large the effect is, not only whether it is significant.
- I ran a power analysis to find the power of this study and the sample size needed to detect an effect of d = 0.3.
- I tested the treatment effect in 5 overlapping demographic subgroups, then applied Bonferroni and Benjamini-Hochberg corrections.
- I simulated p-value distributions for a true null and for a false null to see how p-values behave in each case.

## Key Findings
Trainees earned $[YOUR VALUE] more in 1978 than controls (Welch's t = [YOUR VALUE], p = [YOUR VALUE]). This is a Cohen's d of [YOUR VALUE]. Across the 5 subgroups, [YOUR VALUE] effects were significant before correction, and [YOUR VALUE] remained significant after Bonferroni.
