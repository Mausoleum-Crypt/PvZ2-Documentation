Stat scaling is edited under ScaledProps in ZombieProperties.

This can affect the HP, eatDPS and speed of a zombie.

Stat multiplier formula:
arg1^(level - 1) + arg2 x (level - 1)

Vanilla uses
arg1 = 1.3
arg2 = 0.05
for all zombie's HP and eatDPS.

...also apparently decimal and negative levels work