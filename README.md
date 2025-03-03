# shark_attack_week2_group2:  Building a Shark Attack Resistant Swimsuit Business


## Dataset and Hypothesis

. Dataset: The dataset contains historical records of shark attack incidents, including details such as date, year, type of attack, country, state, location, activity, species involved, sex, age of the victim, and the outcome of the attack.
. Hypothesis: Shark attacks are influenced by factors such as age, activity type, and location. Designing swimsuits targeting high-risk demographics and activities could reduce risks.
## Process Overview
Data Cleaning: Addressed missing, inconsistent, and duplicate data to ensure the dataset was reliable for analysis.
Analysis: Conducted exploratory data analysis (EDA) to identify patterns in attack frequency, demographics, and environmental factors.
Visualizations: Used data visualizations to communicate findings and support the hypothesis.

# Data Wrangling and Cleaning

## Challenges Encountered:
Missing Data: Critical columns like "Age," "Sex," and "Species" had a significant number of null values.
Inconsistent Formats: Columns such as "Country" and "Date" had inconsistent capitalization, typos, and formatting issues.
Duplicates: Detected and removed duplicate rows that inflated the dataset.
Undefined Categories: "Fatal Y/N" and "Sex" contained undefined or ambiguous categories.

## Solutions:
Age: Replaced missing values with group-based medians (e.g., by country or activity type) to preserve trends.
String Cleaning: Used Python libraries like str.lower() and regular expressions to standardize text columns.
Dropped Irrelevant Columns: Removed columns irrelevant to the objective (e.g., "Name").
Handling Undefined Values: Grouped unknown categories into "Unknown" to maintain clarity while avoiding bias.
Regex-Based Function for Cleaning Age DataTo address inconsistencies in the Age column of the dataset, a custom function leveraging regular expressions (regex) was developed. The primary goal was to handle entries representing age ranges (e.g., "20 and 30", "15 to 20") by replacing them with their average, ensuring a uniform numerical format for analysis.

# Exploratory Data Analysis

## Methods Used:
Frequency Distribution: Counted shark attack cases by country, year, and type to identify hotspots and trends.
Pivot Tables: Used pivot tables to analyze the relationship between species and the type of attack or location.
Visualizations: Created bar charts, line graphs, and heatmaps to communicate findings effectively.
## Key Insights:
Hotspot Countries: The USA and Australia accounted for the majority of shark attacks, making these key markets for the swimsuit.
Activity Type: Surfing and swimming were the most common activities during attacks, suggesting target demographics.
Demographics: Young males (15–35 years) were disproportionately affected, with most incidents involving male victims.
Fatality Rates: Although shark attacks were frequent, fatal incidents were relatively rare (less than 20%).

# Major Obstacle
## Biggest Challenge:
Ambiguous Age Data: A significant portion of the dataset had missing or inconsistent age data, making it difficult to draw reliable demographic conclusions.
Resolution: Combined statistical imputation with domain-based assumptions (e.g., assigning "adult" based on activity type like surfing or diving).
## Lessons Learned:
Anticipating data quality issues is critical when working with real-world datasets.
Establishing a structured approach to handle missing and inconsistent data can prevent time loss later in the project.

# Conclusion and Insights
## Hypothesis Outcome:
Shark attacks indeed varied by location, age, and activity type, confirming that certain groups are at higher risk.
However, some unexpected findings (e.g., low fatality rates) contradicted common perceptions about shark attacks.
## Surprising Insights:
The majority of shark attacks occurred near popular beaches in the USA and Australia.
The "Species" column revealed that most attacks were attributed to Great White Sharks, but other species like Bull Sharks and Tiger Sharks also posed significant risks.
## Potential Implications:
Market Targeting: Focus marketing efforts for the swimsuit on high-risk groups (e.g., surfers, swimmers, and young males) in regions like the USA and Australia.
Product Development: Incorporate research on shark species' hunting behaviors to design effective deterrents for the swimsuit.
Awareness Campaigns: Educate the public about the low fatality rate and ways to avoid encounters with sharks.
