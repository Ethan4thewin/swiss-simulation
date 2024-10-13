# Swiss Format Tournament Simulation
This project simulates the Swiss format being used in the League of Legends World Championship, starting in 2023. 
The goal of the simulation is to observe how 8 professional teams perform compared to 8 semi-professional teams in a 16-team Swiss-style tournament. 
The simulation evaluates whether professional teams generally qualify over semi-professional teams under this format.

## Tournament Format Overview
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

## Future Work
- Fine-tuning the skill gap between professional and semi-professional teams.
- Testing with different scenarios, such as varying the number of teams or the number of rounds.
- Adding more detailed statistics tracking for each simulation run.

## License
This project is licensed under the MIT License.
