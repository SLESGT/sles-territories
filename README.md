# sles-territories
This script is a lighter version of the qb-territories, I isolated the territories part of his script to create a configurable zone that will trigger a notification and a drawtext to warn you that you are in a "hostile zone"


# Update

- Multi-Languages support
- Config blips for each zone
- GangName on Blips

# How to add zone ?

to add zone you have to go in shared/zones.lua line 7 and add your zone like this =
```
[1] = {
            centre = vector3(37.38, -1880.71, 22.34),
            radius = 120.0,
            winner = "Yakuza",
            blip = 437
        },
[2] = {
            centre = vector3(x, y, z),
            radius = 90.0,
            winner = "Vagos",
            blip = 437
}
```

Remember that the winner variable is the color of the gang that you configure line 46 =

```
["Colours"] = {

        ["Ballas"] = 27,
        ["the gang color/name"] = 10

}
```
You can find color id here -> https://wiki.rage.mp/index.php?title=Blip::color

# Requirements

- qb-drawtext
- PolyZone

