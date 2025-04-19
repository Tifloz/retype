---
label: Utiliser Jitsuri
icon: square-fill
order: 5
---

# ▶️Utilisation du bot

### 🛠️ Initialisation

La fenêtre Dofus sera automatiquement redimensionnée, **n'y touchez pas !**  

![L'interface une fois connecté](/static/usage/connected-interface.png)

> 💡 **Note :** Voici l'interface du bot une fois connecté.

---

### ⚙️ Configuration

#### 🤖 Configuration du trajet
+++ Pack Découverte
Vous pouvez charger votre propre trajet en appuyant sur ce bouton puis en selectionnant un fichier lua

![L'interface principale](/static/usage/trajet-decouverte.png)

+++ Pack Premium
En tant que détenteur d'un pack premium, vous avez accès à un ensemble de trajets créés par nos **Concepteurs de Trajets**

Pour les charger voici comment faire :

![L'interface principale](/static/usage/trajet-premium-selection.png)

+++

==- 🎯 Résultat
![Interface avec trajet chargé](/static/usage/trajet-loaded.png)
==-

#### ⛏️ Configuration des ressources

!!!info Info
- Une fois votre trajet chargé, les ressources référencées dans celui-ci seront automatiquement sélectionnées.
- Si vous cochez la case **Tout récolter**, le bot récoltera tout ce qu'il peut en fonction de son niveau de métier.
!!!

Pour ajouter d'autres ressources, sélectionnez-les dans l'onglet "Ressources" du bot.

==- 🎯 Résultat
![Sélection des ressources](/static/usage/ressources-selection.png)
==-

### 🚀 Lancement et surveillance

#### 🟢 Démarrage

- Activez le **mode créature**.
- Cliquez sur **"Lancer le trajet"** pour commencer.
- Le bot prendra le contrôle de la souris.
- **⚠️ Important :** Vous devez être en mode créature.

> 💡 **Note :** Ne touchez ni au clavier ni à la souris pendant l'exécution.

---

#### 👀 Surveillance

- Gardez un œil sur les logs pour vérifier le bon fonctionnement.
- Le bot fonctionnera de manière autonome une fois lancé.

---

#### 🔔Notifications

Le bot peut vous envoyer des notifications sur Discord lors de certains événements :

- **Lancement / Fin d'un combat**
- **Message privé**
- **Retour en banque**

Voici comment les configurer

==- 🔔 Configuration des notifications

**Sur le bot**

Sélectionnez le type de notifications voulues

![Choix des notifications](/static/usage/notifs-config.png)

**Sur Discord**

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

#### 💰 Retour en banque

Le bot est capable de retourner seul pour déposer toutes ses ressources à la banque.

**🔎 Vérifications avant lancement :**

- Utiliser le **Havre Sac de Kerubim** par défaut.
- Ne pas avoir de zaap en favoris.
- Avoir débloqué le zaap le plus proche de la banque sélectionnée dans les paramètres du bot
