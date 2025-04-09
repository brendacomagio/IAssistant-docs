# Politique de Confidentialité – Extension "IAssistant"

**Date de dernière mise à jour :** 09 Avril 2025

## 1. Introduction

Cette Politique de Confidentialité décrit comment Jérémy Lenard ("l'Éditeur", "nous") collecte, utilise et protège les informations dans le cadre de l'utilisation de l'extension de navigateur "IAssistant" ("l'Extension").

L'Extension a pour but d'assister l'utilisateur en générant des résumés de pages web, en aidant à la rédaction d'emails et en gérant une bibliothèque de prompts personnels, en se connectant à des services d'Intelligence Artificielle (IA) choisis et configurés par l'utilisateur.

Nous nous engageons à protéger votre vie privée. Cette politique explique quelles données sont traitées, pourquoi, et comment nous les gérons.

## 2. Responsable du Traitement

L'éditeur de l'Extension, responsable du traitement des données potentiellement collectées dans le cadre strict de la configuration et du fonctionnement minimal de l'extension (comme les paramètres stockés localement), est :

* **Nom :** Jérémy Lenard
* **Contact :** [brendacomagio@gmail.com](mailto:brendacomagio@gmail.com)

**Important :** L'Éditeur n'est **pas** le responsable du traitement des données envoyées aux services IA tiers (Google Gemini, Groq, LM Studio). Lorsque vous utilisez ces services via l'Extension avec vos propres clés API ou instance locale, vous interagissez directement avec ces tiers selon leurs propres politiques de confidentialité et conditions d'utilisation.

## 3. Données Collectées et Traitées par l'Extension

L'Extension est conçue pour minimiser la collecte de données personnelles par l'Éditeur. Cependant, pour fonctionner, elle interagit avec certaines informations :

* **Contenu de l'Onglet Actif :** Lorsque vous activez les fonctions "Résumer" ou "Email Rapide", l'Extension lit le contenu textuel principal (`body.innerText`) de la page web ou de l'email affiché dans votre onglet actif. Ce contenu peut potentiellement contenir des données personnelles. **Ce contenu n'est PAS stocké par l'Extension après traitement.**
* **Clés API et URL de Services IA Tiers :** Vous pouvez fournir vos propres clés API pour Google Gemini et Groq, ainsi que l'URL de votre instance LM Studio locale. Ces informations sont **stockées localement** dans votre navigateur via l'API `chrome.storage.local` et ne sont utilisées que pour envoyer des requêtes aux services correspondants *à votre demande*. Elles ne sont jamais transmises à l'Éditeur.
* **Bibliothèque de Prompts Personnels :** Les noms et textes des prompts que vous créez et sauvegardez dans l'Extension sont **stockés localement** via `chrome.storage.local`. Les fonctions d'import/export génèrent/lisent des fichiers locaux sur votre machine, sans transfert vers l'Éditeur.
* **Instructions pour Email :** Le texte que vous saisissez dans le champ "Instructions spécifiques" pour la fonction Email Rapide est utilisé temporairement pour construire la requête envoyée au service IA choisi. Il n'est pas stocké durablement par l'Extension.
* **Paramètres de Configuration :** Vos choix de service IA et de modèle préféré sont **stockés localement** via `chrome.storage.local` pour améliorer votre expérience utilisateur.
* **Métadonnées de l'Onglet Actif :** L'Extension accède temporairement à l'URL et au titre de l'onglet actif pour les afficher dans son interface et s'assurer qu'elle peut interagir avec la page. Ces métadonnées ne sont pas stockées.

L'Éditeur ne collecte **aucune** autre donnée personnelle (nom, adresse email, localisation, historique de navigation global, etc.) via l'Extension.

## 4. Finalités du Traitement

Les informations traitées par l'Extension le sont exclusivement pour les finalités suivantes :

* Permettre la génération de résumés du contenu de l'onglet actif via le service IA choisi.
* Permettre la génération de suggestions de réponses email basées sur le contexte de l'email actif et les instructions fournies, via le service IA choisi.
* Permettre la connexion aux services IA tiers (Gemini, Groq, LM Studio) en utilisant les clés API ou URL fournies par l'utilisateur.
* Permettre la sauvegarde, la gestion et la réutilisation des prompts personnels de l'utilisateur.
* Stocker localement les préférences de configuration de l'utilisateur.

## 5. Base Légale du Traitement (RGPD)

Le traitement des données par l'Extension repose sur :

* **Votre Consentement :** Lorsque vous activez une fonction (clic sur "Résumer" ou "Générer une réponse"), vous consentez à ce que l'Extension lise le contenu de l'onglet actif et l'envoie (si nécessaire) au service IA que vous avez sélectionné et configuré.
* **La Nécessité Contractuelle / Fonctionnelle :** Le stockage local de vos clés API, URL LM Studio, préférences et prompts est nécessaire pour que l'Extension puisse fournir les fonctionnalités que vous avez configurées et utilisez.

## 6. Stockage des Données

* **Contenu Web/Email :** Traité de manière éphémère pour la génération du résultat IA et **non stocké** par l'Extension.
* **Clés API, URL LM Studio, Préférences, Bibliothèque de Prompts :** Stockés **localement** sur votre appareil via l'API `chrome.storage.local`. Ces données restent sur votre machine et ne sont pas accessibles par l'Éditeur. Elles sont conservées jusqu'à ce que vous les modifiiez, les supprimiez via les options de l'Extension, ou désinstalliez l'Extension.

## 7. Transferts de Données

**Aucune donnée n'est transférée vers l'Éditeur de l'Extension.**

Les transferts de données suivants peuvent avoir lieu, **uniquement à votre initiative et sous votre contrôle** :

* **Vers Google Gemini / Groq Cloud :** Si vous configurez et sélectionnez ces services, le contenu textuel de l'onglet actif (et vos instructions éventuelles) sera envoyé à leurs serveurs via votre clé API personnelle pour traitement. Ces transferts sont régis par les politiques de confidentialité de Google et Groq, respectivement. Ces serveurs peuvent être situés en dehors de l'Union Européenne (notamment aux États-Unis).
* **Vers LM Studio :** Si vous configurez et sélectionnez ce service, le contenu textuel sera envoyé à l'URL locale spécifiée (généralement sur votre propre ordinateur). Aucun transfert externe n'a lieu via l'Extension dans ce cas.

L'Éditeur n'est pas responsable des pratiques de confidentialité de Google, Groq ou de la configuration de votre serveur LM Studio.

## 8. Vos Droits (Conformément au RGPD)

Vous disposez des droits suivants concernant les données gérées par l'Extension :

* **Droit d'accès, de rectification, d'effacement :** Vous pouvez accéder, modifier ou supprimer vos clés API, URL LM Studio, préférences et prompts directement via la page d'options de l'Extension.
* **Droit à la portabilité :** Vous pouvez exporter votre bibliothèque de prompts via la fonction d'export dans les options.
* **Droit à la limitation du traitement / Droit d'opposition :** Vous pouvez cesser d'utiliser certaines fonctionnalités ou désinstaller l'Extension.

Pour les données potentiellement envoyées à Google Gemini ou Groq, vous devez exercer vos droits directement auprès de ces sociétés.

Pour toute question concernant vos droits sur les données potentiellement gérées localement par l'Extension, vous pouvez contacter l'Éditeur à l'adresse email fournie à la section 2.

Vous avez également le droit d'introduire une réclamation auprès de l'autorité de contrôle compétente (la CNIL en France).

## 9. Sécurité

Nous prenons la sécurité au sérieux. Les clés API et autres paramètres sont stockés via `chrome.storage.local`, conçue pour le stockage sécurisé de données d'extension. Les communications avec les API cloud (Gemini, Groq) se font via HTTPS. Cependant, la sécurité de vos clés API et de votre configuration LM Studio locale relève de votre responsabilité. Ne partagez pas vos clés API.

## 10. Cookies

L'Extension "IAssistant" n'utilise **aucun cookie**.

## 11. Vie Privée des Enfants

L'Extension n'est pas destinée aux enfants de moins de 16 ans (ou l'âge minimum requis dans votre juridiction). Nous ne collectons pas sciemment d'informations auprès d'enfants.

## 12. Modifications de cette Politique

Cette Politique de Confidentialité peut être mise à jour occasionnellement. La date de "Dernière mise à jour" en haut du document indiquera la date d'entrée en vigueur des modifications. Nous vous encourageons à consulter régulièrement cette politique (accessible via la page d'options de l'Extension).

## 13. Contact

Pour toute question relative à cette Politique de Confidentialité, veuillez contacter l'Éditeur à : [brendacomagio@gmail.com](mailto:brendacomagio@gmail.com)

---

**RAPPEL TRÈS IMPORTANT :** Ce texte est un **modèle généré par IA** basé sur l'analyse du code fourni. Il **DOIT ÊTRE VÉRIFIÉ, ADAPTÉ ET VALIDÉ** pour s'assurer qu'il est parfaitement exact, complet et conforme aux lois applicables (RGPD, etc.) et aux pratiques réelles de votre extension. Une consultation juridique est recommandée.
