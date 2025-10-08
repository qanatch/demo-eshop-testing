#  Test Plan – Demo E-Shop

**Author:** Natalia Chernenkaya  
**Project:** Demo E-Shop  
**Date:** 15 September 2025  
**Testing Period:** 15–18 September 2025  

---

##  Objective

This document defines the plan for all testing activities for the online store **“Demo E-Shop.”**  
It specifies the testing scope, strategy, documentation, entry/exit criteria, risks, and schedule.  
The goal is to ensure high product quality and a positive user experience when using the application.

---

##  Product Overview

The purpose of testing is to verify the correct functionality of the **Demo E-Shop**, including:

- Display of categories and products  
- Functionality of product cards, shopping cart, and order process  
- Correct application of discounts and price calculations  
- Operation of the **Admin Panel** and additional functions (export, reset)

---

##  Scope of Testing

### Frontend (User Interface)
- **Home page:** Display of product categories with items.  
- **Product card:** Name, price, stock quantity, image, “Add to Cart” button.  
- **Product detail:** Name, price, stock quantity, image.  
- **Shopping cart:** Display of items, total price, and quantity modification.

### Order Process
- **Order form:**  
  - **Required fields:** First name, last name, street, city, ZIP code, email, phone (with prefix).  
  - **Optional fields:** Date of birth, discount code, “Student” checkbox.  
- **Field validation:** Max. 30 characters; valid email and phone formats.  

### Discount Rules
- Age **65+** → −5 %  
- **FREESHIP8** → free shipping  
- **AUDIO20PC** → −20 % on audio products  
- **FLAT20** → −20 USD on total order  
- **Student** → −15 %  
- **Card payment** → −5 % (combinable)

### Delivery Methods
- Pick-up point (free)  
- Delivery to box ($5)  
- Home delivery ($15)

### Payment Methods
- Card (−5 %)  
- Cash  
- PayPal

### Order Summary and Confirmation
- Order summary clearly displays all data.  
- Order confirmation includes all entered information and confirms purchase.

---

##  Admin Panel

- Product list with options to **add**, **edit**, or **delete** products.  
- **Required fields:** Name, Category, Price, Stock, Image (select from list).  
- **Optional fields:** Brand, Color, Description.  
- **Additional features:** Export product list to Excel.

---

##  Out of Scope

- Real payment gateway integrations (card payments simulated only)  
- Performance and load testing  
- Security, authentication, and user permissions  
- Localization and multilingual testing

---

##  Testing Strategy

### Testing Levels
- Functional  
- System  
- Integration  
- User Acceptance  

### Testing Types
- **Functional testing** — verifying all requirements.  
- **Form validation** — required/optional fields, limits, and formats.  
- **Discount logic** — all combinations and edge cases.  
- **UI/UX testing** — layout, responsiveness, and consistency.  
- **Negative scenarios** — empty cart, invalid email, wrong discount code.

---

##  Environment & Tools

| Component | Details |
|------------|----------|
| Platform | Desktop – Windows 11, Chrome 140 |
| Tools | DevTools, MS Excel (for export verification) |
| TMS | Google Sheets |

---

##  Test Documentation & Reporting

Deliverables include:  
- Test checklists  
- Test cases  
- Bug reports  
- Final test summary report  

---

##  Entry Criteria

- Test environment (Demo E-Shop Frontend + Admin Panel) is available.  
- All required functions implemented.  
- Test data, browsers, and tools prepared.  
- Priorities and deadlines defined.

---

##  Exit Criteria

- All planned test cases and checklists executed (**run rate = 100 %**)  
- Test pass rate ≥ 90 %  
- No open blocker or high-priority (**P1**) defects  
- ≤ 10 % open low-severity issues (**P2, P3**)  
- Core product functionality confirmed  
- Final test report prepared and delivered

---

##  Risks & Mitigation

| Risk | Mitigation |
|------|-------------|
| Lack of documentation | Use initial requirements as the single source of truth |
| Possible inconsistencies in discounts | Test all discount combinations |
| Excel export issues | Validate using multiple MS Office versions |
| Schedule delays | Prioritize smoke and critical functionality |

---

##  Test Schedule

| Date | Activity |
|------|-----------|
| **15 Sep 2025** | Smoke test — basic functionality, application availability |
| **16 Sep 2025** | Functional testing — homepage, product detail, cart, order, admin panel |
| **17 Sep 2025** | Discount logic, validation rules, negative scenarios |
| **18 Sep 2025** | UI/UX verification, final test report preparation |

---

