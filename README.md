# Tax Declaration Assistant (Vaud, Switzerland)

This project aims to build an intelligent tax assistant for **tax professionals in the canton of Vaud**, automating the processing of individual tax declarations using advanced document understanding and AI technologies.

---

## Project Goals

- Dramatically reduce the time and manual effort tax professionals spend preparing individual tax declarations.
- Improve accuracy and consistency of reported tax data.
  
---

## Key Features

- **Automated data extraction** from standardized tax documents (salary certificates, bank statements, transmission forms, etc.).
- **Commute distance calculation** between home and workplace for transportation deduction purposes (via Google Maps APIs).
- **Automated currency conversion** for foreign bank accounts.
- **.vaudtax file export**, fully compatible with [VaudTax](https://www.vd.ch/etat-droit-finances/impots/impots-pour-les-individus/remplir-ma-declaration-dimpot/vaudtax) for official submission to the cantonal tax administration (subject to approval).
- **Deduction type recommendation**: lump-sum (forfaitary) vs. actual expenses.

---

## Demo Preview

[Access the live demo here](https://app-taxai-frontend-ch.azurewebsites.net)

To try the demo:
1. Upload the 6 sample files from `docs/john_doe`.
2. Click **"Commencer l’analyse"**.
3. Review and confirm data in the intermediate step.
4. View the generated tax declaration.

> Note: The **"Exporter la déclaration"** button is shown for demo purposes only and is not yet implemented.

---

### Use Case: Complete Tax Declaration (Demo)

The demo showcases a **realistic tax declaration scenario** for an individual taxpayer residing in the canton of Vaud.  
It is based on **six anonymized real-world documents**, which together provide all the information typically required to justify a taxpayer’s fiscal situation in Switzerland.

### Documents used in the demo:
1. **Salary certificate** – Contains yearly gross/net income, employer details, AVS number, social deductions, and any bonuses or allowances.
2. **3rd Pillar certificate (Swiss Life)** – Certifies contributions to a private pension (pillar 3a), deductible from taxable income.
3. **Bank statement – Personal account** – Shows the closing balance and interest payments, relevant for wealth declaration.
4. **Bank statement – Savings account** – Provides savings balance and accrued interest, also part of income and wealth declaration.
5. **Health insurance certificate (Assura)** – Lists mandatory (LAMal) and supplementary (LCA) premiums, which may be tax-deductible.
6. **Transmission form** – An administrative cover sheet used during submission to the tax office.

All documents are **authentic in structure** but have been **fully anonymized** to respect confidentiality.  
They reflect the kind of paperwork commonly handled by fiduciaries during the annual tax season.

---

## Tech Stack

<p align="left">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Microsoft_Azure.svg/2048px-Microsoft_Azure.svg.png" alt="Azure" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://www.cdnlogo.com/logos/f/49/fastapi.svg" alt="FastAPI" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://pydantic.dev/favicon/apple-touch-icon.png" alt="Pydantic" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="React" width="40"/>&nbsp;&nbsp;&nbsp;
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Google_Maps_icon_%282020%29.svg/1428px-Google_Maps_icon_%282020%29.svg.png" alt="Google Maps" width="25"/>
</p>

- `Azure Document Intelligence` – AI-powered OCR to process unstructured tax documents
- `Azure OpenAI / Foundry` – Secure LLM hosting to extract relevant tax fields from documents
- `Google Maps APIs` – Geocoding & Distance Matrix for commute analysis.
- `Pydantic` - Data validation and serialization for structured tax models.
- `FastAPI` – Python backend (private)
- `React` – Frontend UI (private)

---
## Business Collaboration

This project is developed in collaboration with the independent tax advisory firm [**elysio.ch**](https://elysio.ch/), ensuring practical alignment with fiduciary needs and fiscal compliance within the canton of Vaud.

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
