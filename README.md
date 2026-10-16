Restaurant Tips Dataset — Data Exploration

 Tips (restaurant tips dataset)
- Dataset URL:https://github.com/mwaskom/seaborn-data/blob/master/tips.csv
- Direct CSV URL: https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv
- Original-source documentation: https://rdrr.io/cran/reshape2/man/tips.html
- Brief description:The dataset records restaurant bills and tips, alongside information about the bill payer, whether the party included a smoker, the day of the week, the meal period, and party size. The dataset is commonly described as records from one food server at one restaurant over approximately two and a half months in the early 1990s.
- Time period covered: Approximately two and a half months in the early 1990s, according to a secondary description of the dataset. Individual calendar dates are not included in the CSV, so exact start and end dates cannot be established from this file.
- Geographic coverage: One restaurant in a suburban shopping mall in the United States; the specific city and restaurant are not identified in the CSV.
- Number of rows: 244 observations (each row represents one bill/tip record).
- Number of columns: 7.
- File format: CSV (comma-separated values).

Important variable types

- Numerical variables: total_bill, tip, size.
- Categorical variables:sex, smoker, day, time.
- Date/time variables: There is no calendar-date or timestamp column. day and time are categories only.
- Geographic variables: None. The CSV does not include coordinates, city, or restaurant address.
- Variables of greatest interest: total_bill and tip can be compared directly; size, day, time, and smoker can be used to investigate whether the relationship varies between groups.


Observations:
- The middle 50% of bills fall between $13.35 and $24.13.
- The middle 50% of tips fall between $2.00 and $3.56.
- The mean tip as a percentage of the bill is approximately 16.08% when each bill's tip percentage is calculated first and those percentages are then averaged.
- There are 244 records and the commonly used CSV version has no missing values in its seven columns.

Potential data problems and limitations

- This is a small sample from one server and one restaurant, not a representative survey of all restaurant customers.
- The dataset does not identify the restaurant, city, customers, or exact dates.
- sex describes the recorded bill payer, not necessarily every member of the party.
- smoker indicates whether the party included a smoker; it does not tell us how many people smoked.
- There are no fields for service quality, food/drink type, payment method, tax, discounts, or customer income. These factors could affect tipping but cannot be tested here.
- The dataset can show associations, not prove that one variable causes another.
- Counts are uneven across days and meal periods. Group averages can be unstable for categories with fewer observations, especially Friday.
- The original source's license should be checked before reuse outside the classroom.


Three possible uses / visualization concepts

Idea A — “Does a bigger bill mean a bigger tip?”
-What it shows: Each point represents one bill. The horizontal axis is total bill and the vertical axis is tip. Hovering reveals bill, tip, tip percentage, party size, day, and meal period. Filters allow users to focus on a day or meal period.
- Who might use it: Students learning data visualization, restaurant managers, or anyone curious about tipping patterns.
- Why it matters: It makes the relationship between bill size and tip visible and helps distinguish tip amount from tip percentage.


Idea B — “How does tipping vary across the week?”
- What it shows: A bar chart comparing average tip percentage by day, with the number of records shown in each category. A selector can switch between average tip amount and average tip percentage.
- Who might use it: People exploring service patterns or learning how categorical comparisons work.
- Why it matters: It compares days while making sample sizes visible, so a small Friday sample is not mistaken for a definitive pattern.
-
Idea C — “What changes when party size changes?”
- What it shows: A chart comparing total tip and tip per person by party size (1–6 people), with optional lunch/dinner filtering.
- Who might use it: Students, restaurant operators, or people curious about group dining.
- Why it matters: A large party may leave a larger total tip simply because more people are eating. Showing per-person values adds context.

Chart selected
Does a Bigger Bill Mean a Bigger Tip?  with variables in days of the week
244 restaurant bills; each point represents one dining party.


