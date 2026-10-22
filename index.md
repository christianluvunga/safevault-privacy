# Politique de confidentialité — SafeVault

*Dernière mise à jour : 22 octobre 2026*

[English version below](#english-version)

La présente politique décrit la manière dont l'application Android **SafeVault** (gestionnaire de mots de passe) traite vos informations. L'application est développée par Christian Luvunga Mayedi.

## 1. En résumé

SafeVault ne collecte aucune donnée personnelle, ne se connecte à aucun serveur et ne partage rien avec des tiers. Vos données restent chiffrées sur votre appareil. Le développeur n'y a aucun accès.

## 2. Fonctionnement hors ligne

- **Aucun serveur et aucun compte** : l'application n'a pas d'infrastructure serveur, pas d'API de stockage distante et ne vous demande aucune inscription.
- **Aucun envoi sur Internet** : vos identifiants, mots de passe, clés et secrets ne quittent jamais votre appareil. L'application est configurée pour bloquer toute connexion réseau et ne déclare aucune permission d'accès à Internet.
- **Aucun accès du développeur** : le développeur ne peut techniquement ni consulter, ni récupérer, ni réinitialiser vos données, votre mot de passe maître ou votre phrase de secours.

## 3. Chiffrement et stockage local

- Les données du coffre sont chiffrées sur votre appareil avec l'algorithme **AES-256-GCM**.
- La clé est dérivée de votre mot de passe maître avec **PBKDF2** (600 000 itérations) et un sel aléatoire propre à votre coffre.
- Le coffre se **verrouille automatiquement** après 3 minutes d'inactivité et lorsque l'application passe en arrière-plan. Les données déchiffrées sont alors retirées de l'écran et de la mémoire de l'application.
- Les captures d'écran de l'application sont bloquées.
- La sauvegarde automatique d'Android est désactivée pour SafeVault.

## 4. Phrase de secours

À la création du coffre, SafeVault vous remet une phrase de secours de 16 mots qui permet de retrouver l'accès si vous oubliez votre mot de passe maître. Elle n'est jamais stockée en clair et n'est transmise nulle part. Toute personne qui la possède, avec votre téléphone, peut ouvrir votre coffre : notez-la sur papier et gardez-la hors de votre téléphone. Après plusieurs essais erronés, un délai d'attente croissant s'applique avant le prochain essai.

## 5. Données collectées et partagées

- **Données personnelles** : aucune. L'application ne collecte ni votre nom, ni votre adresse e-mail, ni votre numéro de téléphone, ni votre position.
- **Identifiants uniques** : aucun (pas d'identifiant publicitaire, pas d'empreinte d'appareil).
- **Partage avec des tiers** : aucun.
- **Publicité, analyse et suivi** : l'application ne contient aucune publicité, aucun outil d'analyse ni aucun traqueur tiers.

## 6. Autorisations Android

- **Biométrie (USE_BIOMETRIC, USE_FINGERPRINT)** : uniquement pour déverrouiller le coffre localement avec votre empreinte, si vous l'activez. La vérification est faite par le système Android ; SafeVault n'a jamais accès à votre empreinte.
- **Aucune autorisation réseau** : à partir de la version 1.2.3, SafeVault ne déclare ni la permission Internet ni celle de l'état du réseau. L'application ne peut donc pas se connecter à Internet.

## 7. Presse-papiers, sauvegardes et partage faits par vous

- **Presse-papiers** : lorsque vous copiez un mot de passe depuis votre liste ou depuis une fiche, il est effacé du presse-papiers après 30 secondes, tant que l'application reste ouverte. Pendant ce temps, d'autres applications de votre appareil peuvent y avoir accès.
- **Sauvegarde chiffrée** : vous pouvez exporter votre coffre dans un fichier chiffré, protégé par un mot de passe d'export que vous choisissez. Ce fichier n'est envoyé nulle part par l'application ; c'est vous qui le conservez ou le partagez.
- **Rapport de diagnostic** : vous pouvez copier un rapport technique dans le presse-papiers pour le transmettre vous-même. Il n'est jamais envoyé automatiquement.
- **Partage de l'application** : le bouton « Partager SafeVault » utilise le menu de partage d'Android pour envoyer un lien vers la fiche de l'application ; aucune donnée de votre coffre n'est incluse.

## 8. Vos droits

Comme SafeVault ne collecte aucune donnée personnelle, vos données sont entièrement sous votre contrôle. Vous pouvez les consulter dans le coffre déverrouillé, les exporter, supprimer des entrées une à une, réinitialiser le coffre depuis l'application, ou désinstaller SafeVault, ce qui supprime définitivement toutes les données locales et les clés associées.

## 9. Enfants

SafeVault ne s'adresse pas spécifiquement aux enfants et ne collecte aucune donnée à leur sujet.

## 10. Modifications

Cette politique peut être mise à jour. La date de dernière mise à jour figure en haut de cette page.

## 11. Contact

Christian Luvunga Mayedi — chrisluvunga@gmail.com

---

<a id="english-version"></a>

# Privacy Policy — SafeVault

*Last updated: October 22, 2026*

This policy describes how the Android app **SafeVault** (password manager) handles your information. The app is developed by Christian Luvunga Mayedi.

## 1. Summary

SafeVault collects no personal data, connects to no server and shares nothing with third parties. Your data stays encrypted on your device. The developer has no access to it.

## 2. Offline operation

- **No server and no account**: the app has no server infrastructure, no remote storage API and does not ask you to sign up.
- **Nothing is sent over the Internet**: your usernames, passwords, keys and secrets never leave your device. The app is configured to block all network connections and declares no Internet permission.
- **No developer access**: the developer cannot technically view, recover or reset your data, your master password or your recovery phrase.

## 3. Encryption and local storage

- Vault data is encrypted on your device with **AES-256-GCM**.
- The key is derived from your master password with **PBKDF2** (600,000 iterations) and a random salt unique to your vault.
- The vault **locks automatically** after 3 minutes of inactivity and when the app goes to the background. Decrypted data is then removed from the screen and from the app's memory.
- Screenshots of the app are blocked.
- Android automatic backup is disabled for SafeVault.

## 4. Recovery phrase

When you create your vault, SafeVault gives you a 16-word recovery phrase that lets you regain access if you forget your master password. It is never stored in clear text and is never sent anywhere. Anyone who has it, together with your phone, can open your vault: write it on paper and keep it away from your phone. After several wrong attempts, an increasing waiting time applies before the next try.

## 5. Data collected and shared

- **Personal data**: none. The app collects no name, email address, phone number or location.
- **Unique identifiers**: none (no advertising ID, no device fingerprint).
- **Sharing with third parties**: none.
- **Advertising, analytics and tracking**: the app contains no advertising, no analytics and no third-party trackers.

## 6. Android permissions

- **Biometrics (USE_BIOMETRIC, USE_FINGERPRINT)**: only to unlock the vault locally with your fingerprint, if you enable it. Verification is done by the Android system; SafeVault never has access to your fingerprint.
- **No network permissions**: starting with version 1.2.3, SafeVault declares neither the Internet permission nor the network-state permission. The app therefore cannot connect to the Internet.

## 7. Clipboard, backups and sharing done by you

- **Clipboard**: when you copy a password from your list or from an entry, it is cleared from the clipboard after 30 seconds, as long as the app stays open. During that time, other apps on your device may be able to access it.
- **Encrypted backup**: you can export your vault to an encrypted file protected by an export password of your choice. The app does not send this file anywhere; you keep or share it yourself.
- **Diagnostic report**: you can copy a technical report to the clipboard to pass it on yourself. It is never sent automatically.
- **Sharing the app**: the "Share SafeVault" button uses Android's share menu to send a link to the app's store page; no vault data is included.

## 8. Your rights

Because SafeVault collects no personal data, your data is entirely under your control. You can view it in the unlocked vault, export it, delete entries one by one, reset the vault from the app, or uninstall SafeVault, which permanently deletes all local data and associated keys.

## 9. Children

SafeVault is not specifically directed at children and collects no data about them.

## 10. Changes

This policy may be updated. The date of the last update appears at the top of this page.

## 11. Contact

Christian Luvunga Mayedi — chrisluvunga@gmail.com
