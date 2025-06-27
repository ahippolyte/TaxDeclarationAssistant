# 🧾 Smart Tax Assistant – Automated Tax Declaration for Fiduciaries (Vaud, Switzerland)

This project aims to build an intelligent tax assistant for **fiduciaries in the canton of Vaud**, automating tax declaration processing for individuals using advanced document understanding and AI technologies.

> ⚠️ This repository does **not contain the source code**. It serves as a **functional and business showcase**. A live demo can be provided upon request.

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

🎥 Demo video: [Insert YouTube or Loom link here]

📸 Screenshots:

| Document Upload | Extracted Results | Deduction Preview |
|------------------|-------------------|--------------------|
| ![](demo/screenshot_1.png) | ![](demo/screenshot_2.png) | ![](demo/screenshot_3.png) |

---

## 🧑‍💼 Business Collaboration

This project is developed in collaboration with the independent tax advisory firm [**elysio.ch**](https://elysio.ch/), ensuring practical alignment with fiduciary needs and fiscal compliance within the canton of Vaud.

---

## 🛠️ Tech Stack

- `Azure Document Intelligence` – AI-powered OCR for structured tax documents
- `Azure Foundry` – secure LLM hosting
- `Google Maps APIs` – Geocoding & Distance Matrix
- `FastAPI` – Python backend (private)
- `Vue.js` – Frontend UI (private)
- `PostgreSQL` – Secure data storage

---

## 💡 Learn More / Get in Touch

📬 Interested in a demo or partnership?

- ✉️ Email: [your.email@domain.ch]  
- 💼 LinkedIn: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)

---

## 🔒 About the Source Code

The full codebase is currently **private**, as the project is in active development and commercial validation.  
Access or technical demonstrations can be provided on a case-by-case basis.

---

Would you like me to generate placeholder screenshots or icons for the `/demo/` folder, or prepare a PDF version of this README?








Demander à ChatGPT
