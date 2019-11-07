# statcast_data

Examining Statcast data


## Variables to consider to build a predicted hit model
- launch angle
- launch speed
- hc_x
- hc_y
- if_fielding_assignment
- of_fielding_assignment
- outs_when_up
- home_team
- stand
- hit_location; realized this variable carries a nan if it's a homerun, so I first tried replacing with a hit location of 10, but then realized that's giving the model a perfect signal for a homerun, so I figured the easiest thing to do is just remove it from the model for now. 
- p_throws


Next steps...examine models with fewer inputs

- ignore home team (i.e. park effects)
- consider fielding team (defensive factors)
- ignore hand of hitter and pitcher
- build a new feature that looks at whether the hitter and pitcher are opposite (L vs. R & R vs L)
- Randomized Grid Search to improve hyperparameters
