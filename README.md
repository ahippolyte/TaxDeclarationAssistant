# 🧾 Assistant de Déclaration Fiscale pour le Canton de Vaud

> 🇬🇧 [English version here / Version anglaise](README.en.md)

Ce projet vise à créer un assistant fiscal intelligent pour les **professionnels de la fiscalité du canton de Vaud**, en automatisant le traitement des déclarations fiscales des personnes physiques, grâce à des technologies avancées de traitement documentaire et d’IA.

---

## Sommaire

- [Objectifs du projet](#objectifs-du-projet)
- [Fonctionnalités clés](#fonctionnalités-clés)
- [Démonstration en ligne](#démonstration-en-ligne)
- [Technologies](#technologies)
- [Collaboration professionnelle](#collaboration-professionnelle)
- [Contact](#contact)
- [A propos du code source](#a-propos-du-code-source)

---

## Objectifs du projet

- Réduire drastiquement le temps et les efforts manuels nécessaires à la préparation des déclarations fiscales individuelles.
- Améliorer la précision et la cohérence des données fiscales transmises.

---

## Fonctionnalités clés

- **Extraction automatique de données** depuis les documents fiscaux non normalisés.
- **Calcul automatisé de la distance domicile-travail** pour le calcul des frais de transport (via l’API Google Maps).
- **Conversion automatique des devises** pour les comptes bancaires étrangers.
- **Export au format `.vaudtax`**, compatible avec [VaudTax](https://www.vd.ch/etat-droit-finances/impots/impots-pour-les-individus/remplir-ma-declaration-dimpot/vaudtax) pour une transmission officielle à l’administration fiscale (fonctionnalité soumise à la certification par le canton de Vaud).
- **Suggestion du type de déduction** : frais effectifs vs. forfaitaires.

---

## Démonstration en ligne

👉 [**Accéder à la démo en ligne**](https://app-taxai-frontend-ch.azurewebsites.net)

### Comment essayer la démo ?

1. **Téléversez les 6 fichiers d’exemple**  
   → Dossier du dépôt : `docs/john_doe`

2. **Cliquez sur “Commencer l’analyse”**  
   → L’analyse fiscale automatisée démarre.

3. **Confirmez l’adresse du lieu de travail et le mode de transport**  
   - L’**adresse du lieu de travail** par défaut est extraite du certificat de salaire, mais peut être ajustée.  
   - **Sélectionnez le mode de transport** (transports publics, voiture, etc.).  
   - Ces informations servent au calcul de la **distance domicile-travail** et des **frais de transport déductibles**.

4. **Consultez la déclaration fiscale générée**  
   → Présentée dans un format structuré similaire à la plateforme officielle **VaudTax**, pour une prise en main immédiate par les professionnels.

> ⚠️ Le bouton **“Exporter la déclaration”** est affiché à titre de démonstration uniquement et n’est pas encore fonctionnel.

---

### Cas d’usage : Déclaration fiscale réaliste

La démo reproduit un **scénario réel** pour un contribuable du canton de Vaud, basé sur **six documents anonymisés mais authentiques dans leur structure** : tout ce qu’il faut pour justifier une situation fiscale typique en Suisse.

### Documents utilisés dans la démo

| Type de document                  | Informations extraites                                            |
|-------------------------------------|-------------------------------------------------------------------|
| **Formulaire de transmission**   | Métadonnées administratives pour la remise à l’administration     |
| **Certificat de salaire**        | Revenu brut/net, numéro AVS, déductions sociales, bonus           |
| **Attestation 3e pilier**        | Cotisations pilier 3a (déductibles)                               |
| **Relevé bancaire – Personnel**  | Solde du compte, intérêts (revenu et fortune)                     |
| **Relevé bancaire – Épargne**    | Solde d’épargne, intérêts                                         |
| **Attestation assurance maladie** | Primes LAMal/LCA (partiellement déductibles)                      |


> Tous les documents sont entièrement anonymisés tout en conservant leur structure réelle.

---

## Technologies

<p align="left">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Microsoft_Azure.svg/2048px-Microsoft_Azure.svg.png" alt="Azure" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://pydantic.dev/favicon/apple-touch-icon.png" alt="Pydantic" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://www.cdnlogo.com/logos/f/49/fastapi.svg" alt="FastAPI" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="React" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Google_Maps_icon_%282020%29.svg/1428px-Google_Maps_icon_%282020%29.svg.png" alt="Google Maps" width="25"/>
</p>

- `Azure Document Intelligence` – OCR avancé et extraction de champs structurés  
- `Azure OpenAI / Foundry` – Extraction et interprétation intelligente des données fiscales  
- `Pydantic` – Validation et modélisation des données  
- `FastAPI` – Backend Python performant  
- `React` – Interface web utilisateur  
- `API Google Maps` – Géolocalisation et calcul d’itinéraires domicile-travail

---

## Collaboration professionnelle

Ce projet est développé en partenariat avec [**elysio.ch**](https://elysio.ch/), cabinet indépendant de conseil fiscal en Suisse romande.  
Cela garantit un alignement fort avec les **besoins des fiduciaires**, la **réglementation fiscale** et les **usages métiers réels**.

---

## Contact

Vous souhaitez collaborer ou en savoir plus ?

- Email : hippolyte.angel@outlook.com
- LinkedIn : [linkedin.com/in/angel-hippolyte](https://linkedin.com/in/angel-hippolyte)

---

## 🔒 A propos du code source

Ce dépôt sert uniquement de **vitrine fonctionnelle et métier**.  
L’intégralité du code reste propriétaire et n’est pas publiée.

---
