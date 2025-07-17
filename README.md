# Assistant de Déclaration Fiscale pour le Canton de Vaud

> [English version here / Version en anglais](README.en.md)

Ce projet vise à créer un assistant fiscal intelligent pour le canton de Vaud, en automatisant le remplissage des formulaires de déclaration fiscale des personnes physiques grâce à des technologies avancées de traitement documentaire et d’intelligence artificielle.

---

## Démonstration en ligne

👉 [**Accéder à la démo en ligne**](https://app-taxai-frontend-ch.azurewebsites.net)

### Comment essayer la démo ?

Rendez-vous sur l'adresse indiquée ci-dessus et suivez les instructions.

### Cas d’usage : Déclaration fiscale réaliste

La démo reproduit un **scénario réel** pour un contribuable du canton de Vaud, basé sur **six documents anonymisés mais authentiques dans leur structure** : tout ce qu’il faut pour justifier une situation fiscale typique en Suisse.

### Documents utilisés dans la démo

| Type de document                  | Informations extraites                                            |
|-------------------------------------|-------------------------------------------------------------------|
| **Formulaire de transmission**   | Métadonnées administratives pour la remise à l’administration     |
| **Certificat de salaire**        | Revenu brut/net, numéro AVS, déductions sociales, bonus           |
| **Attestation fiscale de relevé bancaire – Compte Personnel**  | Solde du compte, intérêts (revenu et fortune)                     |
| **Attestation fiscale de relevé bancaire – Compte Épargne**    | Solde d’épargne, intérêts                                         |
| **Certificat fiscal des cotisations LAMal et LCA** | Primes LAMal/LCA (partiellement déductibles)                      |
| **Certificat de cotisations au pilier 3a**        | Cotisations pilier 3a (déductibles)                               |

> Tous les documents sont entièrement anonymisés tout en conservant leur structure réelle.

---

## Objectifs du projet

- Réduire drastiquement le temps et les efforts manuels nécessaires à la préparation des déclarations fiscales individuelles.
- Améliorer la précision et la cohérence des données fiscales transmises.

---

## Fonctionnalités clés

- **Extraction automatique de données** depuis les documents fiscaux non normalisés.
- **Calcul automatisé de la distance domicile-travail** pour le calcul des frais de transport (via l’API Google Maps).
- **Conversion automatique des devises** pour les comptes bancaires étrangers.
- **Suggestion du type de déduction** : frais effectifs vs. forfaitaires.
- **Export au format `.vaudtax`**, pour une intégration fluide avec le logiciel cantonal [VaudTax](https://www.vd.ch/etat-droit-finances/impots/impots-pour-les-individus/remplir-ma-declaration-dimpot/vaudtax) (fonctionnalité soumise à la certification par le canton de Vaud).

---

## Technologies

<p style="display: flex; align-items: center; justify-content: center; gap: 20px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Microsoft_Azure.svg/2048px-Microsoft_Azure.svg.png" alt="Azure" width="40"/>&nbsp;&nbsp;&nbsp;
   <img src="https://pydantic.dev/favicon/apple-touch-icon.png" alt="Pydantic" width="40"/>&nbsp;&nbsp;&nbsp;
   <img src="https://registry.npmmirror.com/@lobehub/icons-static-png/latest/files/dark/langgraph-color.png" alt="LangGraph" width="50"/>&nbsp;&nbsp;&nbsp;
   <img src="https://www.cdnlogo.com/logos/f/49/fastapi.svg" alt="FastAPI" width="40"/>&nbsp;&nbsp;&nbsp;
   <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="React" width="40"/>&nbsp;&nbsp;&nbsp;
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Google_Maps_icon_%282020%29.svg/1428px-Google_Maps_icon_%282020%29.svg.png" alt="Google Maps" width="25"/>
</p>

- `Azure Document Intelligence` – OCR avancé et extraction de champs structurés
- `Azure OpenAI / Foundry` – Extraction et interprétation intelligente des données fiscales
- `Pydantic` – Validation et modélisation des données
- `LangGraph` – Orchestration pour le traitement structuré des étapes d’analyse fiscale
- `FastAPI` – Backend Python performant
- `React` – Interface web utilisateur
- `API Google Maps` – Géolocalisation et calcul d’itinéraires domicile-travail

---

## Collaboration professionnelle

Ce projet est développé en partenariat avec [**elysio.ch**](https://elysio.ch/), cabinet indépendant de conseil fiscal en Suisse romande.  
Cela garantit un alignement fort avec les besoins et usages métiers.

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
