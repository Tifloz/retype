---
label: Structure des trajets
icon: square-fill
order: 19
---

##  📂Structure des fichiers
 
### 📑 Format de base

==- 📝 Exemple de trajet

```lua
ELEMENTS_TO_GATHER  = { "frene","ortie" }

function move()
  return {
   { map = "5,-18", path = "bottom", gather = false, fight = false },
   { map = "5,-17", path = "bottom", gather = false, fight = false },
   { map = "5,-16", path = "bottom", gather = false, fight = false },
   { map = "5,-15", path = "left", gather = false, fight = false },
   { map = "4,-15", path = "left", gather = false, fight = false },
   { map = "3,-15", path = "left", gather = false, fight = false },
   { map = "2,-15", path = "left", gather = false, fight = false },
   { map = "1,-15", path = "left", gather = true, fight = false },
   { map = "0,-15", path = "left", gather = true, fight = false },
   { map = "-1,-15", path = "left", gather = true, fight = false },
   { map = "-2,-15", path = "left", gather = true, fight = false },
   { map = "-3,-15", path = "top", gather = true, fight = false },
   { map = "-3,-16", path = "right", gather = true, fight = false },
   { map = "-2,-16", path = "right", gather = true, fight = false },
   { map = "-1,-16", path = "right", gather = true, fight = false },
   { map = "0,-16", path = "right", gather = true, fight = false },
   { map = "1,-16", path = "top", gather = true, fight = false },
   { map = "1,-17", path = "left", gather = true, fight = false },
   { map = "0,-17", path = "left", gather = true, fight = false },
   { map = "-1,-17", path = "left", gather = true, fight = false },
   { map = "-2,-17", path = "left", gather = true, fight = false },
   { map = "-3,-17", path = "top", gather = true, fight = false },
   { map = "-3,-18", path = "right", gather = true, fight = false },
   { map = "-2,-18", path = "right", gather = true, fight = false },
   { map = "-1,-18", path = "right", gather = true, fight = false },
   { map = "0,-18", path = "right", gather = true, fight = false },
   { map = "1,-18", path = "top", gather = true, fight = false },
   { map = "1,-19", path = "left", gather = true, fight = false },
   { map = "0,-19", path = "left", gather = true, fight = false },
   { map = "-1,-19", path = "left", gather = true, fight = false },
   { map = "-2,-19", path = "left", gather = true, fight = false },
   { map = "-3,-19", path = "top", gather = true, fight = false },
   { map = "-3,-20", path = "right", gather = true, fight = false },
   { map = "-2,-20", path = "right", gather = true, fight = false },
   { map = "-1,-20", path = "right", gather = true, fight = false },
   { map = "0,-20", path = "right", gather = true, fight = false },
   { map = "1,-20", path = "right", gather = true, fight = false },
   { map = "2,-20", path = "top", gather = true, fight = false },
   { map = "2,-21", path = "left", gather = true, fight = false },
   { map = "1,-21", path = "left", gather = true, fight = false },
   { map = "0,-21", path = "left", gather = true, fight = false },
   { map = "-1,-21", path = "left", gather = true, fight = false },
   { map = "-2,-21", path = "left", gather = true, fight = false },
   { map = "-3,-21", path = "top", gather = true, fight = false },
   { map = "-3,-22", path = "right", gather = true, fight = false },
   { map = "-2,-22", path = "right", gather = true, fight = false },
   { map = "-1,-22", path = "right", gather = true, fight = false },
   { map = "0,-22", path = "right", gather = true, fight = false },
   { map = "1,-22", path = "right", gather = true, fight = false },
   { map = "2,-22", path = "top", gather = true, fight = false },
   { map = "2,-23", path = "left", gather = true, fight = false },
   { map = "1,-23", path = "left", gather = true, fight = false },
   { map = "0,-23", path = "left", gather = true, fight = false },
   { map = "-1,-23", path = "left", gather = true, fight = false },
   { map = "-2,-23", path = "top", gather = true, fight = false },
   { map = "-2,-24", path = "right", gather = true, fight = false },
   { map = "-1,-24", path = "right", gather = true, fight = false },
   { map = "0,-24", path = "right", gather = true, fight = false },
   { map = "1,-24", path = "right", gather = true, fight = false },
   { map = "2,-24", path = "top", gather = true, fight = false },
   { map = "2,-25", path = "left", gather = true, fight = false },
   { map = "1,-25", path = "left", gather = true, fight = false },
   { map = "0,-25", path = "left", gather = true, fight = false },
   { map = "-1,-25", path = "left", gather = true, fight = false },
   { map = "-2,-25", path = "top", gather = true, fight = false },
   { map = "-2,-26", path = "right", gather = true, fight = false },
   { map = "-1,-26", path = "right", gather = true, fight = false },
   { map = "0,-26", path = "right", gather = true, fight = false },
   { map = "1,-26", path = "right", gather = true, fight = false },
   { map = "2,-26", path = "top", gather = true, fight = false },
   { map = "2,-27", path = "left", gather = true, fight = false },
   { map = "1,-27", path = "left", gather = true, fight = false },
   { map = "0,-27", path = "left", gather = true, fight = false },
   { map = "-1,-27", path = "left", gather = true, fight = false },
   { map = "-2,-27", path = "top", gather = true, fight = false },
   { map = "-2,-28", path = "right", gather = true, fight = false },
   { map = "-1,-28", path = "right", gather = true, fight = false },
   { map = "0,-28", path = "right", gather = true, fight = false },
   { map = "1,-28", path = "right", gather = true, fight = false },
   { map = "2,-28", path = "top", gather = true, fight = false },
   }
  end

```
==-

!!!warning
Au moins une ressource doit être listée.  
Utilisez les noms exacts comme affichés dans l'interface.  
La liste doit être sous cette forme `{"frene","ortie"}`
!!!  
Possibilité de modifier les ressources directement dans le bot.</p>

#### 🗺️ Contenu du trajet

Pour pouvoir se déplacer, le bot a besoin qu'on lui dise où aller et que faire sur telle ou telle carte, voici comment faire :

```lua
function move()
  return {
    -- Exemples possibles avec map
      { map = "-3,-18", path = "right", gather = true, fight = false },
      { map = 212601350, path = "right", gather = true, fight = false },

    -- Exemples simples possibles avec path
      { map = "-3,-18", path = "right", gather = true, fight = false },
      { map = "-3,-18", path = "bottom", gather = true, fight = false },
      { map = "-3,-18", path = "left", gather = true, fight = false },
      { map = "-3,-18", path = "top", gather = true, fight = false },
      { map = "-3,-18", path = "-3,-18", gather = true, fight = false },
      { map = "-3,-18", path = "212601350", gather = true, fight = false },

    
    -- Exemples avancés possibles avec path
      { map = "-3,-18", cell = "61", gather = true, fight = false },
      { map = "-3,-18", path = "zaap(<idDuZaap>)", gather = true, fight = false },

    -- Exemples possibles avec gather
      { map = "-3,-18", path = "right", gather = true, fight = false },
      { map = "-3,-18", path = "right", gather = false, fight = false },

    -- Exemples possibles avec fight
      { map = "-3,-18", path = "right", gather = true, fight = true },
      { map = "-3,-18", path = "right", gather = true, fight = false },
    }
  end
```
#### 📋 Paramètres
{.compact}
| **Nom du paramètre** | **Description**                                      | **Valeurs possibles**       | **Paramètre optionnel** |
|----------------------|------------------------------------------------------|-----------------------------|-------------------------|
| **map**              | Cordonnée de la position par position                | **-31,-56**                 | Non                     |
| **map**              | Cordonnée de la position par map id                  | 212600323                   | Non                     |
|                      |                                                      |                             |                         |
| **cell**             | Changement de map par cell ID                        | **-31,-56**                         | Non                     |
| **path**             | Changement de map par coordonnées                       | 212600323                         | Non                     |
| **path**             | Changement de map par map id                         | 123                         | Non                     |
| **path**             | Changement de map par direction simple                | top \| bottom \| right \| left | Non                     |
| **path**             | Rejoindre le zaap                                   | zaap(ID du Zaap)           | Non                     |
|                      |                                                      |                             |                         |
| **gather**           | Le bot doit-il récolter sur la carte                 | true \| false               | Non                     |
|                      |                                                      |                             |                         |
| **fight**            | Le bot doit-il gérer les combats                     | true \| false               | Oui                     |
