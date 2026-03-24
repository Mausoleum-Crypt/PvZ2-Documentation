Calculate total points in a level
```
=SUM(
ARRAYFORMULA(
	(
		InitialPoints + (
			SEQUENCE(
				Waves * Flags, 1, 0
			)
		) * PointIncrement
	) *
	IF(
		MOD(
			SEQUENCE(
				Waves * Flags, 1, 1
			), Waves
		) = 0, 2.5, 1
	)
))
```

```
=SUM(ARRAYFORMULA(
	(InitialPoints + (SEQUENCE(Waves * Flags, 1, 0)) * PointIncrement) *
	IF(MOD(SEQUENCE(Waves * Flags, 1, 1), Waves) = 0, 2.5, 1)
))
```