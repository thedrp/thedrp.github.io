# The Structure of the Pendulum Cycle's Digi-ROMs
-----
## DMOG Ruleset System
-----
### Slots  
The Pendulum Cycle can receive OG System battles, as well as initiate them (by pressing A on the VS screen). So far, no devices seem incompatible.  
Each Digimon on the Cycle corresponds to a slot in the DMOG, as expected, with evolution stages loosely matching up.
- Rookie = Rookie
- Champion = Champion
- Ultimate = strong Champion or weak Ultimate
- Mega = 1st or 2nd Ultimate
- "Secret Mega" = Slot L (ie, Monzaemon)

One note of interest is that, so far, it seems that if a species of Digimon in a Cycle existed on a DMOG version, it will use that slot within the OG Ruleset on the Cycle. As an example, since Devimon existed on the DMOG v1 in Slot E, a Devimon on the Cycle will be Slot E when battling using the OG Ruleset. (Examples can be found at the bottom of this page.) I'm still working on collecting DMOG serials from Cycles for the few other Digimon that existed on the DMOG in order to confirm if this is always the case.

### Effort  
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
With the reminder that Effort can't be higher than 4, or lower than 0. If it would be higher than 4, it just sets to 4 instead, and if lower than 0 it becomes 0.

### Digi-ROMs  
Finally, a short list of Digi-ROMs pulled from my PenCycle v8 Nightmare Soldiers:
- `DB24-2DD2` Candlemon (slot B, 4 Strength, 0 Count, Loss)
- `DB24-2DD2` DemiDevimon (slot B, 4 Strength, 0 Count, Loss)
- `D728-2DD2` Meramon (slot F, 4 Strength, 0 Count, Loss)
- `D827-2ED1` Devimon (slot E, 4 Strength, 0 Count, Win)
- `DA25-2ED1` Phantomon (slot C, 4 Strength, 0 Count, Win)
- `F30C-2ED1` Piedmon (slot J, 0 Strength, 0 Count, Win)
- `E31C-2ED1` Piedmon (slot J, 3 Strength, 0 Count, Win)
- `F10E-2ED1` MaloMyotismon (slot L, 0 Strength, 0 Count, Win)
- `E11E-2ED1` MaloMyotismon (slot L, 3 Strength, 0 Count, Win)
- `D12E-2ED1` MaloMyotismon (slot L, 4 Strength, 0 Count, Win)
- `D12E-2ED1` MaloMyotismon (slot L, 0 Strength, MegaHit Count, Win)
- `C13E-2ED1` MaloMyotismon (slot L, 1 Strength, MegaHit Count, Win)
- `B14E-2ED1` MaloMyotismon (slot L, 2 Strength, MegaHit Count, Win)
- `B14E-2ED1` MaloMyotismon (slot L, 3 Strength, MegaHit Count, Win)
- `B14E-2ED1` MaloMyotismon (slot L, 4 Strength, MegaHit Count, Win)
