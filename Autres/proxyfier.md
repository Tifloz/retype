---
label: Proxifier
icon: square-fill
order: 4
---

# Installation et utilisation de Proxifier sur une VM avec Jitsuri et Dofus

## 📥 Installation de Proxifier

1. **Téléchargement**
   - Rendez-vous sur le site officiel de [Proxifier](https://www.proxifier.com/).
   - Téléchargez la version adaptée à votre système.
   - Installez le logiciel en suivant les instructions.

2. **Configuration de Proxifier**
   - Ouvrez Proxifier après l’installation.
   - Allez dans `Profile` > `Proxy Servers` et ajoutez un nouveau proxy :
     - **Adresse** : IP du proxy ou de la VM
     - **Port** : `5555`
     - **Type** : SOCKS5 ou HTTPS selon votre proxy
   - Appliquez les modifications.

## ⚙️ Configuration pour Jitsuri et Dofus

1. **Ajout des règles de redirection**
   - Dans Proxifier, allez dans `Profile` > `Proxification Rules`.
   - Cliquez sur `Add` et configurez comme suit :
     - **Nom** : Dofus
     - **Application** : Ajoutez `Dofus.exe`
     - **Action** : Rediriger vers le proxy configuré

2. **Vérification du fonctionnement**
   - Lancez Proxifier et assurez-vous qu'il fonctionne en arrière-plan.
   - Ouvrez Dofus et connectez-vous.
   - Vérifiez que les connexions passent bien par Proxifier via le `Log` de l’outil.

## 🛠 Dépannage

- **Aucune connexion via le proxy** : Vérifiez l’adresse et le port.
- **Dofus ne se connecte pas** : Testez la connexion proxy dans Proxifier.

::: tip
Avec cette configuration, vous pourrez utiliser Jitsuri et Dofus via un proxy de manière transparente sur votre VM.
:::
