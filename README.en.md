# Tax Declaration Assistant for the Canton of Vaud

> [Version en français / French version here](README.md)

This project aims to build an intelligent tax assistant for **tax professionals in the canton of Vaud**, automating the processing of individual tax declarations using advanced document understanding and AI technologies.

## Live Demo

👉 [Access the live demo here](http://84.234.28.222:3002)

### How to try the demo?

Go to the address provided above and follow the instructions.

### Use case: Realistic Tax Declaration

The demo reproduces a **real-life scenario** for a taxpayer in the canton of Vaud, based on **six anonymized documents that remain authentic in structure**: everything needed to justify a typical tax situation in Switzerland. During the first step of the demo, you are invited to download these sample documents.

### Documents used in the demo

| Document type                       | Extracted information                                             |
|-------------------------------------|-------------------------------------------------------------------|
| **Transmission form**                 | Administrative metadata for submission to the tax authorities     |
| **Salary certificate**              | Gross/net income, social deductions, bonus |
| **Bank statement tax certificate – Personal Account** | Account balance, interests (income and wealth)                   |
| **Bank statement tax certificate – Savings Account**  | Savings balance, interests                                        |
| **Health insurance (LAMal and LCA) tax certificate** | LAMal/LCA premiums (partially deductible)                         |
| **Pillar 3a contribution certificate**               | Pillar 3a contributions (deductible)                             |

> All documents are fully anonymized while preserving their real structure.

---

## Project goals

- Drastically reduce the time and manual effort required for preparing individual tax returns.  
- Improve the accuracy and consistency of transmitted tax data.

---

## Key features

- **Automatic data extraction** from non-standardized tax documents.  
- **Automated home-to-work distance calculation** for transport cost deductions (via Google Maps API).  
- **Automatic currency conversion** for foreign bank accounts.  
- **Deduction type suggestion**: actual expenses vs. lump-sum.  
- **Export to `.vaudtax` format**, for seamless integration with the cantonal software [VaudTax](https://www.vd.ch/etat-droit-finances/impots/impots-pour-les-individus/remplir-ma-declaration-dimpot/vaudtax) (feature subject to certification by the canton of Vaud).

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

- `Azure Document Intelligence` – Advanced OCR and structured field extraction  
- `Azure OpenAI / Foundry` – Intelligent extraction and interpretation of tax data  
- `Pydantic` – Data validation and modeling  
- `LangGraph` – Orchestration for structured processing of tax analysis steps  
- `FastAPI` – High-performance Python backend  
- `React` – User web interface  
- `Google Maps API` – Geolocation and home-to-work route calculation  

---

## Professional collaboration

This project is developed in partnership with [**elysio.ch**](https://elysio.ch/), an independent tax advisory firm in French-speaking Switzerland.  
This ensures strong alignment with real-world business needs and practices.

---

## Contact

Want to collaborate or learn more?

- Email: hippolyte.angel@outlook.com  
- LinkedIn: [linkedin.com/in/angel-hippolyte](https://linkedin.com/in/angel-hippolyte)  

---

## 🔒 About the source code

This repository serves only as a **functional and business showcase**.  
The full code remains proprietary and is not published.

---
