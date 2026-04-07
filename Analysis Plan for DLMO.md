# Analysis Plan for DLMO Dataset
## 1. Data Cleaning and Quality Control(Data Preprocessing)

Before calculating the onset, I will address three specific data quality issues to ensure the baseline is accurate:

• **LOD (Limit of Detection) Handling**: Values recorded as "0" are not true zeros but represent levels below the machine's detection limit. I will replace these with a constant (e.g. LOD/2) to prevent a **floor effect** from distorting the evening baseline.

• **Outlier & Artifact Removal**: I will identify and exclude initial high readings (like the 8.6 pg/mL in FD200) as **Initial artifact**. Additionally, sudden temporary drops in concentration (likely due to brief light exposure, like the 2.25 pg/mL in PB10) will be smoothed using a Median Filter to preserve the overall secretion trend.

• **Baseline Normalization**: Since peak melatonin varies significantly between individuals (e.g., 7.5 vs. 17.5 pg/mL), I will normalize the data to focus on the relative rate of rise rather than absolute concentration.

## 2. Adaptive Modeling Strategy
  
I will use a two-track modeling approach based on the sampling density and noise level of each profile:

• **Segmented (Hockey-stick) Regression**: For clean, fixed-interval laboratory data (like the PB series), this model is preferred. It clearly identifies the **inflection point** where the horizontal baseline shifts into a linear rise, offering high clinical interpretability.

• **GAMM (Generalized Additive Mixed Models)**: For irregular field data (like the FD series), I will use GAMM to fit a smooth spline. This handles non-linearities and uneven time gaps without the biases of simple linear interpolation, providing a more robust fit for **messy real-world data**.

## 3. DLMO Determination & Validation
**Threshold Setting**: To ensure fairness across all subjects, DLMO will be defined as the time when melatonin reaches 25% of the individual’s nightly peak. I will also calculate a standard 2 pg/mL onset as a benchmark for comparison.
+ Derivative-Based Detection (for GAMM): For profiles fitted with GAMM, I will analyze the first derivative (slope) of the curve. This identifies the point of maximum acceleration in melatonin secretion, capturing **the biological surge** regardless of absolute concentration.

## 4. Validation & Uncertainty Quantification
For ambiguous or low-signal profiles (e.g., civibe_melatonin_FD210), I will report Bayesian credible intervals to show the uncertainty of the estimate. 
Finally, I will overlay the estimated onset onto the original plots for a **sanity check** to ensure the mathematical output aligns with biological plausibility.
