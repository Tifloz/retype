---
label: Paramètres du bot
icon: square-fill
order: 9
---


# ⚙️ Paramètres

L’onglet **Paramètres** de Jitsuri permet de configurer le comportement global du bot, notamment la gestion des combats, les options automatiques et les notifications. Il est divisé en plusieurs sections :

---

## 🌐 Langue

Permet de sélectionner la langue d'affichage de l'interface.

---

## 🔁 Options générales

Ces options définissent le comportement automatique du bot :

- **Passer automatiquement les tours** : le bot passe son tour s’il n’a aucune action à effectuer.
- **Se mettre prêt automatiquement** : dans un groupe, le bot clique automatiquement sur "Prêt".
- **Réanimer automatiquement au phénix** : si le personnage meurt, il est réanimé automatiquement.
- **Combattre automatiquement** : le bot engage automatiquement les combats selon les règles définies.

---

## 🔔 Paramètres de notification

Active ou désactive les différentes notifications envoyées par le bot, notamment via Discord :

- **Notification Discord**
- **Notification de messages privés**
- **Notification Trésor**
- **Notification Forgemagie**
- **Notification Récolte**
- **Notification Archimonstre**

==- Configuration des notifications sur Discord

Faites attention à bien activer vos MP en provenance du serveur Jitsuri, voici comment vérifier :

1. **Paramètres Utilisateurs &gt; Contenu et Social &gt; Permissions sociales**
2. **Dans le menu déroulant, sélectionnez le serveur "Jitsuri - Early Access"**
3. **Vérifiez que "Messages privés" est bien activé**

![Activer les DM](/static/usage/notifs-discord-dm.png)

!!!info
Pensez à autoriser les MPs de la part des membres du serveur Jitsuri dans vos paramètres Discord pour recevoir les notifications.
!!!

1. **Faites un clic droit sur le serveur Jitsuri dans votre liste de serveurs**
2. **Cliquez sur "Paramètres de confidentialité"**
3. **Assurez-vous que l'option "Autoriser les MP des autres membres de ce serveur" est activée.**

![Activer les DM](/static/usage/notifs-discord-dm-users.png)

==-
---

# ⚔️ Paramètres de combat

Cette section permet de configurer les sorts que le bot utilise automatiquement pendant les combats.

## ➕ Ajouter un sort

Pour ajouter un sort automatisé :

1. Sélectionner un sort dans la liste déroulante.
2. Configurer les options suivantes :
   - **Appliquer sur moi** : le sort est lancé sur le personnage lui-même.
   - **Nombre de fois par tour** : nombre maximum d’utilisations du sort par tour.
   - **Temps de recharge** : nombre de tours à attendre avant de réutiliser le sort.
   - **Délai** : nombre de tours à attendre après le début du combat avant la première utilisation.
3. Cliquer sur **Ajouter à la liste**.

---

## 📋 Gestion de la liste des sorts

Une fois ajoutés, les sorts apparaissent dans une liste consultable et modifiable.

{.compact}
| Champ                  | Description |
|------------------------|-------------|
| **#**                 | Ordre d'exécution du sort |
| **Sort**              | Nom et icône du sort |
| **Appliquer sur moi** | Indique si le sort est lancé sur soi-même |
| **Nombre de fois par tour** | Limite d’utilisation par tour |
| **Temps de recharge** | Nombre de tours avant une nouvelle utilisation |
| **Délai**             | Tour à partir duquel le sort devient actif |
| **Actions**           | Modifier l’ordre (⬆️/⬇️) ou supprimer (🗑️) un sort |

---

🔧 **Astuce** : L’ordre des sorts est crucial. Les sorts en haut de la liste sont exécutés en priorité.
