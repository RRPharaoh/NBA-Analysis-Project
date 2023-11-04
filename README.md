# Midterm-Project
## Project/Goals
 - Analyze the correlation between NBA players and the colleges they attended
 - Does the school an NBA player attend impact the success of their professional career?

## Process
 1. Collect historical information on NBA players along with their respective colleges
 2. Establish Github repository with the relevant data, connect with collaborators 
 3. Conduct exploratory data analysis through Python and Tableau
 4. Transform, parse and clean data
 5. Create models and generate regressions in Python to analyze relationship between colleges and desired variables
 6. Interpret results
 7. Create visualizations within Tableau
 8. Present findings from Tableau story


## Results
### MAIN QUESTION: Does the college an NBA player attend impact the success of their professional career?

### RESULTS

When analyzing the correlation between colleges and NBA player career success, assumptions must be created regarding what constitutes a top school. By the looking at the players each college produced, most notably their total number of minutes played, a system had been created which ranked colleges based on their aggregated total number of minutes played by said school’s alumni. The top five colleges in terms of NBA career success, in descending order, consisted of Kentucky, Duke, UNC, Arizona and UCLA. 

In order to analyze the success of any given player’s career, four distinct measures had been created with variables from the data serving as proxies. 
The metrics included:
- Longevity 
    - The number of years a player is active within the organization
- Performance
  - Their average points per game
- Team contribution
  - Win shares per 48 minutes which essentially measures a player’s overall contribution to their team’s win
- Desirability 
  - Their position within the overall pick

Utilizing exploratory data analysis and regression models, a visible correlation may be seen between any given college’s rank and the proposed metrics. Regressions of college rank on the distinct measure all proved to statistically significant, all possessing p-values < 0.05. Points per game, years active and win shares per game all exhibited a negative correlation whereas the correlation between college rank and overall pick proved to be positive; as college rank increase, i.e., the colleges decrease in quality, a player’s average performance, longevity and contributions to the team decrease.

Note: The variables for college rank and overall pick function inversely – a lower value for these variables is actually better in terms of scaling.

In regards of interpretation, once a student transfers from the 10th ranked school to 1st, the model predicts said player would, on average, score 0.4 more points per game and play in the NBA for an additional 110 days. In terms of the remaining variables, the model indicates that students from better colleges possess higher win shares per game and a higher likelihood of being a top pick for the draft. 

Some outliers were found and analyzed to gain a better understanding of schools that were over and underrepresented. 
utilizing historical draft data with selection positions as metric, we were able to differentiate a school with sheer volume of drafted players (Kentucky) vs a school with consistently higher selected players (Duke) when you account for the lottery pick system utilized by the NBA. While Kentucky has the most drafted players in NBA history, Duke has nearly 3 times the amount of lottery picks while simultaneously having fewer overall players drafted. While we might be able to assert that this proves that Duke produces more "desirable" prospects, more analysis is necessary to support this assessment.

## Challenges 
- Time constraints were one of our major constraints as there were instances when we wanted to explore certain aspects of the data but had to reassess the viability of being able to completely flesh out and explore a hypothesis.

- Deciding on what to exclude from the data set to keep our explorative data within scope of our analysis.

- Volume of the data was large, and it provided us with a variety of information. However, we had to decide what to include and what to exclude from the data.

 The inability to legitimately deduce the cause-and-effect relationship between our data analysis and the performance/ value of a player.
 A way to conceptualize this would be trying to deduce whether a player was recruited to a school’s program because they were elite or did they became elite after attending the school’s program.

## Future Goals
-In the future we'd like to take a deeper dive into individual NBA team's recruitment process, and the intricacies of College Basketball Programs.
Analysis of factors that were excluded from the dataset, such as:
- Trades
- Injuries
- Championship wins.
These are factors that can affect the data in various ways and potentially change the outcome of some of our findings. 

