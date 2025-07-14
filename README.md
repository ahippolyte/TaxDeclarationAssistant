# 🧾 Tax Declaration Assistant (Vaud, Switzerland)

This project aims to build an intelligent tax assistant for **tax professionals in the canton of Vaud**, automating the processing of individual tax declarations using advanced document understanding and AI technologies.

---

## 🚀 Project Goals

- Dramatically reduce the time and manual effort tax professionals spend preparing individual tax declarations.
- Improve accuracy and consistency of reported tax data.
  
---

## 🧠 Key Features

- **Automated data extraction** from standardized tax documents (salary certificates, bank statements, transmission forms, etc.).
- **Commute distance calculation** between home and workplace for transportation deduction purposes (via Google Maps APIs).
- **Automated currency conversion** for foreign bank accounts.
- **.vaudtax file export**, fully compatible with [VaudTax](https://www.vd.ch/etat-droit-finances/impots/impots-pour-les-individus/remplir-ma-declaration-dimpot/vaudtax) for official submission to the cantonal tax administration (subject to approval).
- **Deduction type recommendation**: lump-sum (forfaitary) vs. actual expenses.

# Technologies

<p align="left">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Microsoft_Azure.svg/2048px-Microsoft_Azure.svg.png" alt="Azure" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://www.cdnlogo.com/logos/f/49/fastapi.svg" alt="FastAPI" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://pydantic.dev/favicon/apple-touch-icon.png" alt="Pydantic" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="React" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Google_Maps_icon_%282020%29.svg/1428px-Google_Maps_icon_%282020%29.svg.png" alt="Google Maps" width="25"/>
</p>

- **Azure**
  - **Azure Document Intelligence** – AI-powered OCR to process unstructured tax documents
  - **Azure OpenAI / Foundry** – Secure LLM hosting to extract relevant tax fields from documents
- **FastAPI** – Python backend
- **Pydantic** – Data validation and serialization for structured tax models.
- **React** – Frontend UI
- **Google Maps APIs** – Geocoding & Distance Matrix for commute analysis.

---

## Demo Preview
Live demo available [here](https://app-taxai-frontend-ch.azurewebsites.net)

To try the demo, upload the 6 sample files from docs/john_doe, then click the "Commencer l’analyse" button.

An intermediate data confirmation step will appear for demonstration purposes, simply click "Confirmer les données" to proceed, and the final tax declaration will then be displayed.

Please note: the "Exporter la déclaration" button is not yet implemented and is currently shown for demonstration purposes only.

---

## Business Collaboration

This project is developed in collaboration with the independent tax advisory firm [**elysio.ch**](https://elysio.ch/), ensuring practical alignment with fiduciary needs and fiscal compliance within the canton of Vaud.

---

## Tech Stack

- `Azure Document Intelligence` – AI-powered OCR for structured tax documents
- `Azure Foundry` – secure LLM hosting
- `Google Maps APIs` – Geocoding & Distance Matrix
- `FastAPI` – Python backend (private)
- `React` – Frontend UI (private)

---

## Learn More / Get in Touch

Interested in partnership?

- Email: [hippolyte.angel@outlook.com]  
- LinkedIn: [linkedin.com/in/angel-hippolyte](https://linkedin.com/in/angel-hippolyte)

---

## 🔒 About the Source Code

The full codebase is proprietary and not available in this repository.
This repository just serves as a **functional and business showcase**.

---
