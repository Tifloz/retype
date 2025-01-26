# ▶️Utilisation du bot

### 🛠️ Initialisation

La fenêtre Dofus sera automatiquement redimensionnée, **n'y touchez pas !**
![Capture d'écran](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/capture-decran-2025-01-04-182557.png)

> 💡 **Note :** Voici l'interface du bot une fois connecté.

---

### ⚙️ Configuration

#### 🤖 Configuration du trajet

- Sélectionnez votre trajet dans le menu déroulant. > Pour en créer un vous-même : **[Création de trajet](https://docs.jitsuri.xyz/books/premieres-etapes/page/creation-de-trajets)**
- Cochez les cases **IA-Combat** et **IA-Icon**.

**🎯 Résultat :**
![Capture d'écran](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/capture-decran-2025-01-04-182557.png)

---

#### ⛏️ Configuration des ressources

> 💡 **Note :** Une fois votre trajet chargé, les ressources référencées dans celui-ci seront automatiquement sélectionnées.

Pour ajouter d'autres ressources, sélectionnez-les dans l'onglet "Ressources" du bot.

**🎯 Résultat :**
![Image](https://docs.jitsuri.xyz/uploads/images/gallery/2024-12/scaled-1680-/6hwimage.png)

---

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

<details id="bkmrk-%F0%9F%94%94-configuration-des-"><summary>🔔 Configuration des notifications</summary>

**Sur le bot**

Sélectionnez le type de notifications voulues

[![image.png](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/scaled-1680-/iRRimage.png)](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/iRRimage.png)

**Sur Discord**

Faites attention à bien activer vos MP en provenance du serveur Jitsuri, voici comment vérifier :

1. **Paramètres Utilisateurs &gt; Contenu et Social &gt; Permissions sociales**
2. **Dans le menu déroulant, sélectionnez le serveur "Jitsuri - Early Access"**
3. **Vérifiez que "Messages privés" est bien activé**

[![image.png](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/scaled-1680-/G2Eimage.png)](https://docs.jitsuri.xyz/uploads/images/gallery/2025-01/G2Eimage.png)

</details>---

#### ⚔️ Combat

Pour recevoir des notifications en cas de combat :

1. Configurez un webhook dans le bot.
2. Une fois configuré, les notifications seront envoyées :
    - 📲 Sur Discord
    - 🛡️ Directement sur le bot

> 💡 **Note :** Cette configuration permet d'être alerté automatiquement lorsqu'un combat commence.

**🎯 Résultat :**
![Notification 1](https://docs.jitsuri.xyz/uploads/images/gallery/2024-12/scaled-1680-/notif1.png)
![Notification 2](https://docs.jitsuri.xyz/uploads/images/gallery/2024-12/scaled-1680-/notif2.png)

---

#### 💰 Retour en banque

Le bot est capable de retourner seul pour déposer toutes ses ressources à la banque.

**🔎 Vérifications avant lancement :**

- Utiliser le **Havre Sac de Kerubim** par défaut.
- Ne pas avoir de zaap en favoris.
- Avoir débloqué le **zaap d'Astrub**.

> ⚠️ **Attention :** Le bot utilisera le bouton **"Transférer les objets visibles"**. Prenez cela en compte à votre reconnexion.