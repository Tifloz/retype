---
label: Guide de conversion
icon: square-fill
order: 2
---

# Guide de conversion

## 🔄 Outils de conversion

Ces outils peuvent être utiles pour convertir ou générer des trajets à partir d’autres formats :

- **ChatGPT** : Génération rapide de trajets en Lua.
- **Perplexity** : Pour des recherches et suggestions sur les formats de trajet.


## 🔄 Conversion entre formats

### 🛠️ De FlatyBot vers Jitsuri

+++ FlatyBot

```lua
{ map = "9,0", gather = true, changeMap = "top" },
{ map = "9,-1", gather = true, changeMap = "left" }
```

+++ Jitsuri

```lua
{ map = "9,0", path = "top", gather = true, fight = false },
{ map = "9,-1", path = "left", gather = true, fight = false }
```
+++

### ⚠️ Points importants

1. **Conserver l’ordre des cartes** : Le bot interprète les instructions ligne par ligne.
2. **Utiliser les paramètres exacts** : Les identifiants des ressources ou directions doivent être exacts.

#### Exemple de boucle

```lua
ELEMENTS_TO_GATHER = { "261" }

function move()
  return {
    { map = "5,-18", path = "bottom", gather = false, fight = false },
    { map = "5,-17", path = "left", gather = true, fight = false },
    { map = "4,-17", path = "top", gather = false, fight = false },
    { map = "4,-18", path = "right", gather = false, fight = false },
  }
end
```

**Prochaines étapes** : Consultez les conseils pratiques pour tester et optimiser vos trajets.
