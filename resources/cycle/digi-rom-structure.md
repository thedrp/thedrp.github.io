# The Structure of the Pendulum Cycle's Digi-ROMs
-----
### DMOG Ruleset System
-----
The Pendulum Cycle can receive OG System battles, as well as initiate them (by pressing A on the VS screen).  
Each Digimon corresponds to a slot in the DMOG, as expected, with evolution stages loosely matching up.
- Rookie = Rookie
- Champion = Champion
- Ultimate = strong Champion or weak Ultimate
- Mega = 1st or 2nd Ultimate
- "Secret Mega" = Monzaemon

"Effort" is calculated based on Strength Hearts and the Count shaken before the connection.  
If a MegaHit Count is shaken, then Effort starts at 2, otherwise it starts at -2.  
Add 1 to Effort for each Strength Heart, then cap Effort off at 4, and if it's below 0 it becomes 0.

#### MegaHit Effort Values:
- `0 Strength = 2 Effort`
- `1 Strength = 3 Effort`
- `2 Strength = 4 Effort`
- `3 Strength = 4 Effort`
- `4 Strength = 4 Effort`

#### MegaHit Effort Values:
- `0 Strength = 0 Effort`
- `1 Strength = 0 Effort`
- `2 Strength = 0 Effort`
- `3 Strength = 1 Effort`
- `4 Strength = 2 Effort`

Another way to explain it is that the Effort formula comes out as follows:  
`X = # of Strength Hearts`  
If MegaHit, then `Effort = 2 + X`  
    else `Effort = X - 2`  
With the reminder that Effort can't be higher than 4. If it would be higher than 4, it just sets to 4 instead.
