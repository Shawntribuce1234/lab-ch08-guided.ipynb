# Hypothesis Testing — Is Job Training Worth It?

## Objective
In this lab, I wanted to determine whether participating in a job training program led to higher earnings and whether the results were statistically significant.

## Methodology
- Loaded the LaLonde NSW job training dataset containing 445 participants, including 185 trainees and 260 controls.
- Performed a one-sample t-test and a two-sample Welch's t-test to compare earnings.
- Created my own `welch_t()` function and compared its results with SciPy.
- Calculated Cohen's d to measure the size of the training effect.
- Conducted a power analysis to understand how sample size affects the ability to detect an effect.
- Tested five demographic subgroups and applied Bonferroni and Benjamini-Hochberg corrections.
- Simulated p-values to explore false positives and statistical significance.

## Key Findings

The job training program showed a positive effect on earnings, with a Welch's t-statistic of **2.6741**. This suggests that participants who received training earned more on average than those who did not.

Before correcting for multiple comparisons, **2 of the 5 subgroups** showed statistically significant results. After applying Bonferroni and Benjamini-Hochberg corrections, only **1 subgroup** remained significant.

I also learned that statistical significance does not necessarily mean an effect is large. Cohen's d helps measure the size of the difference, while power analysis shows how sample size affects our ability to detect it.

## Conclusion

This lab helped me understand how hypothesis testing can be used to evaluate real-world programs. I learned that looking at p-values alone can be misleading, especially when testing multiple groups. Using effect sizes, power analysis, and multiple-testing corrections gives a better understanding of whether a program is actually making a difference.
