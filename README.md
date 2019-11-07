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
- hit_location
- p_throws


Next steps...examine models with fewer inputs

- ignore home team (i.e. park effects)
- ignore hand of hitter and pitcher
- build a new feature that looks at whether the hitter and pitcher are opposite (L vs. R & R vs L)
