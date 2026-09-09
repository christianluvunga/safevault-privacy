# Politique de Confidentialité — Safevault

**Dernière mise à jour :** 9 septembre 2026

La présente politique de confidentialité décrit la manière dont l'application mobile **Safevault** traite vos informations.

Safevault a été conçue selon les principes fondamentaux de la **confidentialité dès la conception (Privacy by Design)**, de la **minimisation des données** et du **Zero-Knowledge** (zéro connaissance). Notre engagement est absolu : vous êtes le seul et unique propriétaire de vos secrets.

---

## 1. Architecture Zero-Knowledge & Fonctionnement Hors-Ligne

Safevault est une application **100 % hors-ligne (air-gapped by design)** :
* **Aucun serveur distant :** L'application ne possède aucune infrastructure serveur, aucune API externe de stockage et aucune base de données cloud.
* **Aucun transit réseau :** Vos identifiants, mots de passe, clés et secrets ne transitent jamais sur Internet et ne quittent à aucun moment votre appareil.
* **Absence d'accès développeur :** En tant que développeur, nous n'avons techniquement aucun moyen d'accéder, de consulter, de récupérer ou de réinitialiser vos données ou votre mot de passe maître.

---

## 2. Cryptographie et Stockage Local Sécurisé

Toutes les informations enregistrées dans Safevault sont protégées localement à l'aide de protocoles cryptographiques conformes aux normes industrielles les plus strictes :
* **Chiffrement au repos :** Chiffrement symétrique authentifié **AES-256-GCM** (Galois/Counter Mode) appliqué localement sur votre appareil.
* **Dérivation de clé :** Utilisation d'un algorithme de dérivation de clé robuste (**PBKDF2**) combiné à un sel cryptographique aléatoire unique généré par l'appareil.
* **Mémoire vive volatile :** Les secrets en clair sont conservés en mémoire uniquement le temps de leur consultation, masqués automatiquement après expiration du compte à rebours, et purgés immédiatement de la mémoire volatile lors de la mise en veille ou de la fermeture de l'application.

---

## 3. Données Collectées et Partagées

* **Données personnelles :** **Aucune.** Nous ne collectons pas votre nom, votre adresse email, votre numéro de téléphone ou vos données de localisation.
* **Identifiants uniques :** **Aucun.** Aucun identifiant publicitaire (AAID), empreinte numérique de terminal (device fingerprinting) ou identifiant matériel unique n'est recueilli.
* **Partage avec des tiers :** Safevault ne vend, n'échange, ne loue et ne transmet aucune donnée à des tiers ou à des courtiers en données.

---

## 4. Outils Tiers, Traqueurs et Publicités

* **Aucune régie publicitaire :** L'application est dépourvue de tout SDK publicitaire.
* **Aucune télémétrie ni outil d'analyse :** Aucun traqueur tiers (Google Analytics, Firebase Crashlytics, Mixpanel, Facebook SDK, etc.) n'est intégré au code de l'application.
* **Journalisation :** Aucune journalisation d'activité (logs) externe n'est réalisée.

---

## 5. Autorisations Android Utilisées

Safevault sollicite uniquement les permissions strictement nécessaires à son exécution locale sécurisée :
* **Authentification biométrique (`android.permission.USE_BIOMETRIC`) :** Utilisée exclusivement pour déverrouiller localement le coffre-fort et pour l'authentification renforcée (Step-up Authentication) avant affichage d'un secret. La vérification est déléguée au processeur sécurisé d'Android (TEE / Secure Enclave). Safevault n'a jamais accès à vos empreintes digitales ou données faciales brutes.
* **Service de saisie automatique (`AutofillService`) :** Utilisé uniquement avec votre consentement explicite pour vous proposer le remplissage sécurisé de vos identifiants dans les applications et navigateurs compatibles. Aucune information lue lors de ce processus n'est conservée en dehors du coffre local chiffré.
* **Presse-papier sécurisé :** Lors de la copie d'un secret, le presse-papier du système est sollicité et programmé pour un nettoyage automatique afin de limiter les risques de fuite inter-applications.

---

## 6. Support et Communications par Email

Si vous choisissez de contacter le support via la fonction intégrée "Signaler un problème" :
* L'application pré-remplit un message via votre client de messagerie natif (`mailto:`).
* Les seules métadonnées techniques éventuellement jointes (modèle d'appareil, version d'Android, version de l'application) sont visibles, modifiables et envoyées **uniquement avec votre action manuelle et délibérée**.
* Ces informations ne sont utilisées que pour diagnostiquer l'anomalie signalée et ne sont jamais réutilisées à d'autres fins.

---

## 7. Vos Droits (RGPD / Réglementations de protection des données)

Puisque Safevault ne collecte, ne conserve ni ne traite aucune donnée personnelle sur des serveurs, l'intégralité du contrôle de vos données repose entre vos mains :
* **Droit d'accès et d'exportation :** Vos données sont accessibles directement dans votre coffre-fort déverrouillé.
* **Droit à l'effacement :** Vous pouvez à tout moment supprimer individuellement vos entrées ou désinstaller l'application. La désinstallation de Safevault ou la suppression de ses données via les paramètres d'Android détruit immédiatement et définitivement toutes les bases chiffrées locales ainsi que les clés associées.

---

## 8. Contact

Pour toute question ou demande d'information concernant cette politique de confidentialité ou l'architecture de sécurité de Safevault, vous pouvez contacter :

* **Responsable :** Safevault Development Team
* **Email de contact :** chrisluvunga@gmail.com
