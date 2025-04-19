---
label: Fonctions et paramètres
icon: square-fill
order: 18
---

#### 🛠️ Fonctions

Les fonctions sont des parties de code qui **peuvent être appelées** et qui doivent la plupart du temps réaliser **une tâche bien précise**.

==- 🔀 Fonction move

```lua
function move()
    return {
    -- Votre logique de déplacement
    }
end
```

==-

#### 🌍Fonctions globales

Afin de vous aider dans vos trajets avancés, vous avez à votre disposition plusieurs fonctions globales, les voici :

==- printMessage

### 🧩 Méthode

---

```lua
printMessage(text)
```

### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| text | string | Message à envoyer dans la console |
| color | string | Couleur du message (red, green, blue, yellow, purple, white) |

==- delay

### 🧩 Méthode

---

```lua
delay(number)
```

### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | ----------------------------------- |
| time | number | Temps de pause en milliseconde (ms) |

==- jobLevel

### 🧩 Méthode

---

```lua
getJobLevel(text)
```

### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | ----------------------- |
|job id| text | Identifiant du métier |

### ↪️ Retour

---

{.compact}
| Types | Description |
| ------ | ------------------------- |
| number | Niveau du métier spécifié |
==- getPods

### 🧩 Méthode

---

```lua
getPods()
```

### ↪️ Retour

---

{.compact}
| Types | Description |
| ------ | ------------------------------------ |
| number | Nombre de pods actuellement utilisés |
==- getPodsMax

### 🧩 Méthode

---

```lua
getPodsMax()
```

### ↪️ Retour

---

{.compact}
| Types | Description |
| ------ | -------------------- |
| number | Nombre de pods total |

==- currentPos

### 🧩 Méthode

---

```lua
getCurrentPos()
```

### ↪️ Retour

---

{.compact}
| Types | Description |
| ---------- | ------------------------------ |
| posX, posY | Coordonnées de la map actuelle |
==- currentMapId

### 🧩 Méthode

---

```lua
getMapId()
```

### ↪️ Retour

---

{.compact}
| Types | Description |
| ------ | --------------------- |
| number | Mapid actuelle du bot |

==- getInventoryItemCount
### 🧩 Méthode

---

```lua
getInventoryItemCount(itemId)
```

### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| itemId | number | Identifiant de l'objet à vérifier |
### ↪️ Retour

---

{.compact}
| Types | Description |
| ------ | --------------------- |
| number | Nombre d'objets dans l'inventaire |
==- useInventoryItem
### 🧩 Méthode

---

```lua
useInventoryItem(itemId)
```
### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| itemId | number | Identifiant de l'objet à utiliser |

==- goToCellId
### 🧩 Méthode

---

```lua
goToCellId(cellId)
```
### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| cellId | number | Identifiant de la cellule à atteindre |

==- goToMapId
### 🧩 Méthode

---

```lua
goToMapId(mapId)
```
### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| mapId | number | Identifiant de la map à atteindre |

==- goUseInteractive
### 🧩 Méthode

---

```lua
goUseInteractive(interactiveId)
```
### 📜 Arguments

---

{.compact}
| Paramètres | Types | Description |
| ---------- | ------ | --------------------------------- |
| interactiveId | number | CellID de l'élément interactif à utiliser |

==-

#### ⚙️Fonction custom

Pour ajouter une fonction custom à votre trajet **qui s’exécutera après l'action sur la map spécifiée mais avant l'instruction** `path`, voici comment faire :

```lua
function move()
    return {
    -- Votre logique de déplacement
          { map = "-31,-56",
      -- Action que le bot fera APRES avoir fait son action custom
      path = "bottom",

      gather = false, custom="takeZaapi" }, -- Map du zaap de bonta
    }
end


function takeZaapi()
    printMessage("Je prends le Zaapi")
    delay(1000)
    printMessage("J'appuie sur hôtel de vente")
    delay(1000)
end
```

Une fonction custom vous permet d'ajouter une logique complexe à votre trajet, comme par exemple un aiguillage, un déchargement en maison, etc ..

!!!info Info
Vous devez garder en tête que ce que vous spécifiez dans l'instruction path sera **exécuté après** votre custom
!!!

#### 📋 Paramètres du trajet

{.compact}
| **Nom du paramètre** | **Description** | **Exemples de valeurs possibles** |
| -------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------- |
| ELEMENTS_TO_GATHER  | Nom des ressources à récolter | "ble", "frene", "ortie", "sauge", ... |