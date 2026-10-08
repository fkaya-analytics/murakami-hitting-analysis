# Munetaka Murakami: MLB Batting Analytics (2026)

An independent sports analytics project using Tableau to explore Munetaka Murakami's batting performance with the Chicago White Sox.

---

## Project Overview
This project analyzes Munetaka Murakami's 2026 MLB batting data to explore his offensive performance, batted-ball quality, home-run production, and interactions with different pitch types.

Using Tableau, I developed interactive dashboards to examine performance from multiple perspectives, including home-run trends, exit velocity, launch angle, spray direction, hard-hit rate, and pitch-type outcomes.

Rather than focusing exclusively on traditional batting statistics, this project aims to understand the underlying patterns behind his offensive production and identify questions that warrant further investigation.

---
**Research Questions**

This project explores five main questions:

1. How has Murakami's home-run production changed over the available 2026 season?
2. Which pitch types have accounted for the largest number of his home runs?
3. What do exit velocity and launch angle suggest about his batted-ball quality?
4. How are his batted balls distributed across pull, center, and opposite fields?
5. What potential strengths, weaknesses, and areas for further investigation emerge from these patterns?

**Tools and Technologies**

Tableau: Interactive dashboards, data visualization, calculated fields, and exploratory analysis.
CSV / Excel: Data organization and preparation.
GitHub: Project documentation, versioned project files, and portfolio presentation.

---
**Dashboard Structure**
**1. HR Profile**

Examines home-run production through:

Home-run trends over time
Home runs by pitch type
Home-run rate by pitch type

This dashboard helps distinguish the frequency of home runs from the rate at which they occur against different pitch types.

**2. Contact Quality**

Examines the quality and distribution of batted balls through:

Exit Velocity Histogram
Launch Angle Histogram
All Batted Balls
Statcast Contact Map
Barrel Map
Hard Hit % by Pitch Type

These visualizations help explore how frequently Murakami makes hard contact, how his batted balls are launched, and how contact characteristics vary across pitch types.

**3. Pitch Matchup**

Examines the relationship between pitch characteristics and batting outcomes through:

Exit Velocity vs. Pitch Velocity
Pitch Velocity Histogram
Pitch-type comparisons

The objective is to investigate how pitch characteristics relate to contact quality, while recognizing that pitch velocity alone cannot explain a batting outcome.

---
**Preliminary Findings**

The following observations are based on the available dataset used for this project. They should be interpreted as descriptive findings rather than definitive evaluations of Murakami's overall MLB performance.

**1. Power is an important part of his offensive profile**

The available records contain 35 home runs. Home runs account for approximately 6.3% of 553 plate appearances with recorded outcomes.

This suggests that power production is a central feature of the observed offensive profile. However, home-run frequency alone does not capture overall offensive value, which also depends on reaching base, strikeout frequency, and other outcomes.

**2. The recorded batted balls show substantial contact quality**

Among 258 records with a positive exit-velocity measurement, average exit velocity was approximately 93.9 mph, while the maximum recorded exit velocity was 114.1 mph.

Approximately 57.8% of these recorded batted balls were classified as hard-hit in the dataset.

These measurements are consistent with a profile capable of producing high-impact contact. Further comparison with league benchmarks would be needed to determine how exceptional these values are relative to other MLB hitters.

**3. Home runs have been produced to all fields**

Of the 35 recorded home runs:

Pull field: 14
Center field: 12
Opposite field: 9

Although the pull field accounts for the largest share, the distribution indicates that home-run production is not limited to pulled balls.

This raises an interesting question: to what extent can Murakami maintain power production when driving the ball toward center and opposite fields? A larger sample and more detailed pitch-location data would help investigate this further.

**4. Home-run totals vary by pitch type**

The largest number of recorded home runs came against four-seam fastballs (13), followed by sinkers (6) and changeups (5).

However, these are counts, not measures of pitch-specific vulnerability. The number of opportunities against each pitch type differs, and the observed results may also reflect pitch location, count, pitcher quality, and sample size.

For this reason, home-run counts should be interpreted alongside home-run rates and the number of opportunities against each pitch type.

**5. Strikeout frequency deserves further investigation**

Among the 553 recorded plate appearances with known outcomes, the two strikeout categories in the dataset account for 196 outcomes, or approximately 35.4%.

This is a potentially important area for further analysis. However, the current dataset does not establish whether these strikeouts resulted from chasing pitches outside the strike zone, missing pitches within the zone, two-strike approach, or other factors.

Pitch-level data would be required to distinguish these explanations.

---
**Potential Implications for Batting Approach**

The current findings suggest several questions worth investigating rather than immediate conclusions about what Murakami should change.

Preserve power while evaluating swing decisions: His recorded home-run and contact-quality metrics support investigating how power production relates to strikeout frequency.
Examine pitch-specific performance using rates: Pitch-type counts should be evaluated alongside opportunities, pitch location, and count context.
Investigate contact across the field: The distribution of home runs across pull, center, and opposite fields provides a basis for studying whether his approach adapts to different pitch locations.
Study launch-angle outcomes: Launch angle should be analyzed jointly with exit velocity and batted-ball outcomes, rather than treating a single ideal angle as universally optimal.
Separate descriptive patterns from causal explanations: The current dashboard identifies relationships and distributions, but does not establish why a particular outcome occurred.

---
**Methodology and Definitions**
The analysis uses plate-appearance records and associated batted-ball and pitch information. Tableau calculated fields and filters are used to summarize and visualize the available data.

Key metrics include:

Home Runs: Count of records classified as Home Run.
Average Exit Velocity: Average exit velocity among records with exit velocity greater than zero.
Maximum Exit Velocity: Maximum recorded exit velocity.
Hard-Hit Rate: Percentage of records with a positive exit-velocity measurement that are flagged as hard-hit in the dataset.
Home-Run Rate: Home-run outcomes divided by the number of plate appearances with recorded outcomes.
Pitch-Type Home Runs: Number of home-run outcomes associated with each recorded pitch type.

---
**Barrel Classification**

The current Tableau workbook uses the following operational rule:

Exit velocity greater than or equal to 95 mph
Launch angle between 20° and 35°, inclusive

This is a simplified project-specific classification. It should not be interpreted as an exact reproduction of MLB's official Statcast Barrel definition.

---
**Limitations**

Several limitations should be considered when interpreting the results:

Data coverage: The findings reflect the records available in the dataset at the time of analysis, not necessarily every game or plate appearance in the 2026 season.
Sample size: Pitch-type comparisons can be sensitive to small numbers of opportunities.
Missing or unrecorded measurements: Exit velocity and launch angle are not available for every plate appearance. Calculations using these metrics exclude records without a positive exit-velocity measurement.
Limited pitch-level context: The current analysis does not fully capture pitch location, swing decisions, count leverage, or the sequence of pitches within each plate appearance.
Descriptive analysis: The observed patterns do not establish causation or prove that a particular batting adjustment would improve performance.
Comparison benchmarks: Without a consistent league-wide comparison dataset, the project cannot establish a definitive percentile or ranking for every metric.

---
**Future Improvements**

Potential extensions include:

Comparing Murakami's metrics with MLB league averages and selected comparable hitters.
Analyzing strikeout and walk rates alongside swing decisions and pitch locations.
Investigating performance by pitch location, count, pitcher handedness, and game situation.
Evaluating home-run rate and hard-hit rate using clearly defined denominators.
Adding automated data updates and a reproducible data-cleaning workflow.
Expanding the analysis with Python or SQL and documenting the workflow.
Updating the dashboard as additional season data becomes available.

---
**What I learned**

This project gave me practical experience with Tableau, data preparation, calculated fields, dashboard design, and analytical communication.

It also reinforced the importance of distinguishing what a dataset directly shows from what an analyst might infer from it. A visualization can reveal a pattern, but interpreting that pattern responsibly requires clear definitions, appropriate denominators, and an understanding of data limitations.

Through this project, I aim to continue developing the technical and analytical skills needed to transform raw data into useful, evidence-based insights.

---
**Data and Attribution**

The analysis is based on the data files used to build this project. Data provenance, source links, update dates, and any applicable usage restrictions should be documented here.

This is an independent educational and portfolio project. It is not affiliated with or endorsed by Major League Baseball or the Chicago White Sox.

Player and team names are used for identification and analytical context.


