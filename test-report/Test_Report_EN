#  Test Report – Demo E-Shop

**Author:** Natalia Chernenkaya  
**Project:** Demo E-Shop (Testing Assignment)  
**Testing Period:** 15–18 September 2025  
**Date Created:** 18 September 2025  

---

##  Objective

The purpose of testing was to verify the functionality of the **Demo E-Shop** application, including both **customer (Shop, Checkout)** and **administrative (Admin Panel)** parts, in accordance with the provided requirements.  
Testing focused on validating core business logic — cart, order flow, discounts, data integrity, and synchronization between Shop and Admin Panel.

---

## Scope of Testing

- **Frontend / Shop:** homepage, product catalog, product detail, cart, checkout, confirmation  
- **Checkout:** field validation, discounts, delivery & payment methods, final calculation  
- **Admin Panel:** product management (CRUD), validation of mandatory fields, Excel export, reset  
- **Integration:** synchronization of Stock between Shop and Admin Panel  
- **UI/UX:** layout consistency, visual feedback, responsiveness  

---

## Test Environment

| Component | Details |
|------------|----------|
| Operating System | Windows 11 |
| Browser | Google Chrome v140 |
| Tools | Google Sheets (TMS), Chrome DevTools, MS Excel |

---

##  Execution Summary

| Metric | Value |
|--------|--------|
| Total test scenarios | 262 |
| Executed | 100 % |
| Pass rate | ≈ 88 % |
| Fail rate | ≈ 12 % |

---

##  Defect Summary

| Severity | Count |
|-----------|-------|
| Critical | 6 |
| Major | 12 |
| Minor | 4 |
| **Total** | **30** |

---

##  Critical Defects

### Discounts  
- Coupon **AUDIO20PC** not applied correctly, message “50 %” shown instead.  
- Combinations **Senior + Student** and **Senior + Card** incorrectly summed.  
- Coupon **FLAT20** reduces total by **$200** instead of **$20**.  

### Admin Panel  
- Product can be saved with empty **Name** or **Price**.  
- Editing a product increases **Price + 10** even without modification.  

### Integration  
- After purchase, **Stock** decreases in Shop but remains unchanged in Admin Panel.  

---

##  Duplicate Products Observation

The system allows adding multiple products with **identical values**.  
Although not defined as a defect in the requirements, this can lead to duplicates in the Admin Panel and inconsistent stock data.

**Possible improvements:**  
- Merge identical products and update **Stock** count only.  
- Block duplicates and display a validation message.

---

##  Conclusion

Based on the executed tests, the **Demo E-Shop application is not ready for production release** in its current version.  
Critical issues were identified in discount logic, form validation, data synchronization, and admin product management.  
These defects may result in **financial inaccuracies**, **stock inconsistencies**, and **negative user experience**.

---

##  Recommendations

It is recommended to **fix all Critical and Major defects** before further testing.  
Priority should be given to the **Checkout** process, **discount logic**, and **Admin Panel validation** to ensure data integrity and reliability.

---



