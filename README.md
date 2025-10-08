##  About Project

The **Demo E-Shop Testing Project** was created as a part of a QA assessment task.  
It represents a **complete manual testing cycle** for a demo online store consisting of:
- customer-facing e-shop,  
- administration panel,  
- data synchronization between both parts.

The documentation covers all key QA artifacts — from **Test Plan** and **Checklists** to **Bug Reports** and **Test Report** — demonstrating a professional testing workflow.---

## Demo E-Shop Testing Project

Manual QA documentation for the **Demo E-Shop** – a sample online store with product catalog, shopping cart, checkout form, and admin panel.  
The goal of testing was to verify correct implementation of functional and validation rules, discounts, and data synchronization between the shop and admin interface.---

## Project Scope

Testing covered both **frontend (customer side)** and **admin panel** functionality.

###  Customer Side
- Product categories and product cards  
- Cart operations and checkout process  
- Validation of mandatory and optional fields  
- Discounts, coupons, and payment methods  
- Order confirmation page  

###  Admin Panel
- Adding, editing, and removing products  
- Validation of required fields (Name, Category, Price, Stock, Image)  
- Optional fields (Brand, Color, Description)  
- Excel export and data integrity check  
- Integration between Admin and E-Shop  

###  Integration Tests
Integration scenarios verified **data consistency between the E-Shop and Admin Panel**, including:
- visibility of newly added products in the shop,  
- synchronization of product updates,  
- correct removal propagation (deleted products not shown in the shop),  
- stock reduction after successful checkout.  

---

##  Documentation

- **Test Plan (CZ / EN)** – scope, strategy, entry/exit criteria, risks  
- **Checklists (Admin, E-Shop)** – verified test cases and results  
- **Integration Test Cases (EN)** – end-to-end consistency scenarios  
- **Bug Reports (CZ / EN)** – list of defects with steps and expected results  
- **Test Report (CZ / EN)** – summary of testing progress and results  

---

##  Test Environment

| Item | Description |
|------|--------------|
| Browser | Google Chrome v140 |
| OS | Windows 11 |
| Tools | Google Sheets, Chrome DevTools, Excel |
| Test Data | Created manually based on specification |

---

##  Summary

- **Approach:** Manual functional testing  
- **Focus:** Validation logic, discount rules, UI behavior, data synchronization  
- **Defects found:** Functional and UI issues (sorting, validation, discount logic)  
- **Deliverables:** Full QA documentation lifecycle (Plan → Execution → Report)  

---

####  Author

Natalia Chernenkaya
QA Tester | Manual & API Testing | Test Documentation  
[LinkedIn](https://www.linkedin.com/in/natalia-chernenkaya)  

*This repository demonstrates a structured, end-to-end approach to manual software testing — from requirement analysis and documentation to defect reporting.*

---
### ⚠️ Disclaimer

This repository is shared **for portfolio and educational purposes only**.  
All documents, test cases, and reports are original work created by **Natalia Chernenkaya**.  
Unauthorized copying, redistribution, or commercial use of this content is not permitted.  
If you would like to reference this project or request access to additional materials,  
please contact me directly via [LinkedIn](https://www.linkedin.com/in/natalia-chernenkaya).

> 🇨🇿 Tento projekt je sdílen pouze pro účely portfolia a vzdělávání.  
> Kopírování nebo další šíření obsahu bez souhlasu autora není povoleno.
---


## 🇨🇿 Demo E-Shop – Testovací dokumentace

Tento projekt obsahuje kompletní dokumentaci k **manuálnímu testování demo e-shopu** – ukázkové aplikace pro nákup elektroniky s administračním panelem.  
Cílem testování bylo ověřit funkčnost obchodní části i administračního rozhraní, včetně validací formulářů, slev, exportu dat a synchronizace produktů.

---

###  Rozsah testování
- Uživatelská část: hlavní stránka, produktové karty, košík, objednávkový formulář, slevy  
- Admin panel: přidávání, úprava a mazání produktů, validace polí, export do Excelu  
- Integrační scénáře: propojení e-shopu s administrační částí  

---

###  Dokumentace
- **Test Plan (CZ / EN)** – rozsah, strategie, rizika, harmonogram  
- **Checklists (Admin, E-Shop)** – všechny otestované případy  
- **Integration Test Cases (EN)** – ověření konzistence dat  
- **Bug Reports (CZ / EN)** – seznam chyb, kroky, očekávané výsledky  
- **Test Report (CZ / EN)** – shrnutí výsledků testování  

---

####  Testovací prostředí
Chrome v140 • Windows 11 • DevTools • Excel • Google Sheets  

---


