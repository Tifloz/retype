---
label: Bot chasse
icon: square-fill
order: 8
---

## 🏹 Interface Chasse — Vue d'ensemble

Cette section présente l’interface utilisateur dédiée au **Bot chasse au trésor**. Elle permet d’automatiser les déplacements, de suivre les indices en temps réel et de consulter l’historique des sessions.

![Interface Chasse](/static/MITM/chasse.png)

==- 📋 Logs détaillés

Affiche en temps réel les actions entreprises par le bot, telles que :

- 🏁 Le démarrage de la chasse
- 🚶 Les déplacements vers chaque salle ou indice
- 🗺️ Le passage par un zaap s’il est plus optimal
- 📍 La validation des drapeaux d’indices

Fonctionnalités utiles :
- **Copier les logs** pour les partager facilement
- **Effacer les logs** pour repartir d’un affichage propre

==- 🧩 Indices en cours

Affichage des indices à résoudre pendant la chasse.

- Chaque indice est représenté avec une icône visuelle (flèche, point d’interrogation)
- Les indices déjà trouvés sont **barrés**
- Une barre de progression indique l'avancement général (ex: `1/6 Indices`)
- Le nombre d'étapes de la chasse est également précisé (ex: `1/3 Étapes`)

🧠 *Ce module est utile pour vérifier la progression de la chasse sans avoir à lire tous les logs.*

==- 📈 Historique des chasses

Affiche les statistiques des dernières chasses effectuées :

- Une barre temporelle montre la durée
- Un bouton permet d’**accéder à l’historique complet**
- Les informations sont triées par jour

🔁 *Idéal pour suivre vos performances et repérer les chasses particulièrement rapides ou lentes.*

==- 🎮 Contrôle de la chasse

Permet de choisir le **mode de chasse** :

- **Mode automatique** : le bot gère tout de A à Z.
- **Mode manuel** : pour garder le contrôle des déplacements tout en bénéficiant d’assistances.

Options disponibles :
- ✅ **Notification Discord** : pour recevoir des updates pendant la chasse
- ⛔ Bouton rouge pour **arrêter la chasse** à tout moment
==-