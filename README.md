# 🧾 Smart Tax Assistant – Automated Tax Declaration for Fiduciaries (Vaud, Switzerland)

This project aims to build an intelligent tax assistant for **fiduciaries in the canton of Vaud**, automating tax declaration processing for individuals using advanced document understanding and AI technologies.

> ⚠️ This repository does **not contain the source code**. It serves as a **functional and business showcase**.

---

## 🚀 Project Goals

- Dramatically reduce the time required to process tax files for fiduciaries.
- Automatically extract key data from standardized supporting documents.
- Generate `.tax` files compatible with the official [VaudTax](https://www.vd.ch/themes/etat-droit-finances/impots/vaudtax/) platform.
- Assist with deduction suggestions (transportation, pension, dependents, etc.).

---

## 🧠 Key Features

- 📄 **Intelligent document extraction**  
  Leveraging [Azure Document Intelligence](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/) to process:
  - salary certificates,
  - bank certificates and statements,
  - transmission forms,
  - other tax-relevant documents.

- 🤖 **Semantic analysis with LLMs**  
  Using **LLMs hosted on Azure Foundry** to interpret extracted data, identify relevant tax fields, detect inconsistencies, and assist with deduction eligibility.

- 📍 **Automatic commute distance calculation**  
  Integration with **Google Distance Matrix API** and **Geocoding API** to estimate home–workplace travel distance and calculate deductible commuting expenses.

- 🔒 **Compliance with Swiss data protection law (nFADP)**  
  The platform is designed with security and privacy by design, fully compliant with Switzerland’s revised Federal Act on Data Protection (2023).

---

## 🔗 Demo Preview
Live demo available at: app-taxai-frontend-ch.azurewebsites.net

To try the demo, simply upload the two files located in docs/john_doe, then click on the "Commencer l'analyse" button.

An intermediate data confirmation step will appear for demonstration purposes—simply click "Confirmer les données" to proceed, and the final tax declaration will then be displayed.

Please note: the "Exporter la déclaration" button is not yet implemented and is currently shown for demonstration purposes only.

---

## 🧑‍💼 Business Collaboration

This project is developed in collaboration with the independent tax advisory firm [**elysio.ch**](https://elysio.ch/), ensuring practical alignment with fiduciary needs and fiscal compliance within the canton of Vaud.

---

## 🛠️ Tech Stack

- `Azure Document Intelligence` – AI-powered OCR for structured tax documents
- `Azure Foundry` – secure LLM hosting
- `Google Maps APIs` – Geocoding & Distance Matrix
- `FastAPI` – Python backend (private)
- `React` – Frontend UI (private)

---

## 💡 Learn More / Get in Touch

📬 Interested in a demo or partnership?

- ✉️ Email: [hippolyte.angel@outlook.com]  
- 💼 LinkedIn: [linkedin.com/in/angel-hippolyte](https://linkedin.com/in/angel-hippolyte)

---

## 🔒 About the Source Code

The full codebase is proprietary and not available in this repository.

---
