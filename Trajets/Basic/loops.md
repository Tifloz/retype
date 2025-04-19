---
label: Fin de trajet
icon: square-fill
order: 3
---

# 🚩Fin de trajet

##  🔁 Boucle


Si vous voulez que votre bot fasse une boucle, il faut que la dernière map de votre trajet dirige vers la première
Voici un exemple :

```lua
GATHERABLES = {"ortie"}
NEAREST_ZAAP = "Astrub"

function move()
    return {
        {map = "5,-18", path = "bottom", gather = false, fight = false}, -- Map de départ au zaap d'Astrub
        {map = "5,-17", path = "left", gather = true, fight = false},
        {map = "4,-17", path = "top", gather = false, fight = false},
        {map = "4,-18", path = "right", gather = false, fight = false}, -- Map finale qui va vers le zaap d'Astrub
    }
end

```
!!!warning Attention
Vous pouvez également faire des boucles non complètes (Qui ne reviennent pas à la première map) mais il faut qu'elles dirigent vers une map qui est déjà dans le trajet. Un message de recovery apparaitra, mais cela ne bloquera pas le bot
!!!

## ↔️ Mode inverse

Si vous souhaitez que le bot fasse le trajet à l'envers, il faut terminer votre trajet par une ligne contenant une instruction `end` comme ceci :

```lua
GATHERABLES = {"ortie"}
NEAREST_ZAAP = "Astrub"

function move()
    return {
        {map = "5,-18", path = "bottom", gather = false, fight = false}, -- Map de départ au zaap d'Astrub
        {map = "5,-17", path = "left", gather = true, fight = false},
        {map = "4,-17", path = "top", gather = false, fight = false},
        {map = "4,-18", path = "end", gather = false, fight = false}, -- Map finale, ensuite le bot va faire le chemin inverse
    }
end

```
