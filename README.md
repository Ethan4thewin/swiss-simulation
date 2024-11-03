# Swiss Format Tournament Simulation
This project simulates the Swiss format being used in the League of Legends World Championship, starting in 2023. 
The goal of the simulation is to observe how 8 professional teams perform compared to 8 semi-professional teams in a 16-team Swiss-style tournament. 
The simulation evaluates whether professional teams generally qualify over semi-professional teams under this format.

## Tournament Format Overview
<p align="center">
  <img src="https://github.com/user-attachments/assets/7ae5537d-58e0-40df-a079-d8e4d1a845b5" alt="Worlds 2023 Swiss Format"/>
</p>

- Swiss Format: Teams are placed in a single group, but do not play against all other teams. Instead, they are matched against opponents with the same win-loss record in each round.
- Matchups: After each round, teams with identical records (e.g., 1-0 vs. 1-0) face each other. This ensures more even matchups as the tournament progresses.

### Advancement/Elimination:

- Teams play up to 5 matches.
- A team qualifies for the knockout stage with 3 wins.
- A team is eliminated after 3 losses.

### Match Types:

- Early rounds are best-of-1 matches.
- Matches switch to best-of-3 when a team reaches match point (either 2 wins or 2 losses).

## Simulation Objective
This simulation aims to determine whether the 8 professional teams typically qualify over the 8 semi-professional teams in a Swiss-style tournament of 16 teams.

## How the Simulation Works
Teams: The simulation considers 16 teams, divided into two groups:

- 8 professional teams
- 8 semi-professional teams

Rounds: Teams are paired according to the Swiss format rules, and the results of each match are simulated based on pre-determined skill levels.

Qualification: The simulation tracks how often professional teams qualify for the knockout stage compared to semi-professional teams.

## Simulation Methodology
This Monte Carlo simulation:
- Runs N independent tournament simulations (N ranging from 100 to 1,000,000)
- For each simulation:
  * Randomly pairs teams according to Swiss format rules
  * Simulates match outcomes based on team skill levels
  * Tracks qualification results
- Aggregates results across all simulations to estimate:
  * Expected number of qualified teams from each skill tier
  * Qualification probabilities for pro vs semi-pro teams
  * Confidence intervals for these estimates

## Results
### 8 teams are drawn in swiss format randomly against each other without initial restrictions
Multiple runs from 100 - 1000000 simulations concurrently reveals:
- Average pro teams qualified: 5.8 ± 0.2
- Average semi-pro teams qualified: 2.13 ± 0.2
- Average pro qualification rate: 72% - 76%
- Average semi-pro qualification rate: 24 - 28%

This means:
- The ratio of qualified teams is approximately 3:1 in favor of pro teams, which can be acceptable since the stronger teams are not automatically qualified, whereas the semi-pro teams have a reasonable chance to qualify.
- The Swiss format seems to be a suitable options for rewarding skill (a clear seperation of skill between 2 levels of teams) while maintaining uncertainty (there's still room for "upsets" or strong performances from semi-pro teams).

## Future Work
- Fine-tuning the skill gap between professional and semi-professional teams.
- Testing with different scenarios, such as varying the number of teams or the number of rounds.
- Adding more detailed statistics tracking for each simulation run.

## License
This project is licensed under the MIT License.
