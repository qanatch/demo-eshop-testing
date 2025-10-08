#  Demo E-Shop – Customer Side Test Checklist (EN)

This checklist covers the **frontend (shop) functionality** of the Demo E-Shop:  
main page, product cards, cart, order form, and discount logic.  
It validates both functional and UI behavior from the customer perspective.


## Homepage ##

## 1.Page Load

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-001 | Page load – main page loads successfully | ✅ Passed | Functional |
| ES-002 | Logo is displayed | ✅ Passed | UI |
| ES-003 | Shop name is displayed | ✅ Passed | UI |
| ES-004 | Click on shop name → redirect to homepage | ❌ Failed | Functional |
| ES-005 | Cart icon is displayed | ✅ Passed | UI |
| ES-006 | “Add to Cart” button is available | ✅ Passed | Functional |
| ES-007 | Repeated click on “Add to Cart” adds another item | ❌ Failed | Functional |

---

## 2.Categories / Sidebar

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-008 | Category list is displayed | ✅ Passed | UI |
| ES-009 | Switching to a specific category (e.g. Audio) → products of that category are displayed | ❌ Failed | Functional |
| ES-010 | Switching to another category (e.g. Toys) | ✅ Passed | Functional |
| ES-011 | Switching to “All” displays all products | ✅ Passed | Functional |
| ES-012 | Switching between categories works correctly | ✅ Passed | Functional |

---

## 3.Filter / Dropdown

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-013 | Filter options are displayed | ✅ Passed | UI |
| ES-014 | Opening the “Sort by” dropdown → all sorting options are shown | ✅ Passed | Functional |
| ES-015 | Sorting alphabetically (A–Z) | ❌ Failed | Functional |
| ES-016 | Sorting alphabetically (Z–A) | ❌ Failed | Functional |
| ES-017 | Sorting by price (Low → High) | ✅ Passed | Functional |
| ES-018 | Sorting by price (High → Low) | ✅ Passed | Functional |
| ES-019 | Sorting by availability (Low → High) | ✅ Passed | Functional |
| ES-020 | Sorting by availability (High → Low) | ✅ Passed | Functional |
| ES-021 | Reset filtering | ✅ Passed | Functional |

---

##  Product Card ##

## 1.Product Detail

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-028 | Product name is displayed | ✅ Passed | UI |
| ES-029 | Product image is displayed | ✅ Passed | UI |
| ES-030 | Specifications / characteristics are displayed | ✅ Passed | UI |
| ES-031 | Availability ("In stock") is displayed | ✅ Passed | UI |
| ES-032 | “Back to Shop” button works | ✅ Passed | Functional |
| ES-033 | “Add to Cart” button is available | ✅ Passed | Functional |
| ES-034 | Spelling and grammar check of the text | ❌ Failed | UI |

## 2.Button: Add to Cart

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-035 | Product is added to cart | ✅ Passed | Functional |
| ES-036 | Repeated product addition to cart | ✅ Passed | Functional |

## 3.Quantity Selector

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-037 | Functionality of “+ / –” buttons | ✅ Passed | Functional |
| ES-038 | Selected quantity is added to cart | ✅ Passed | Functional |

## Cart ##
## 1.General

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-039 | Empty cart is displayed | ✅ Passed | UI |
| ES-040 | Closing the cart using the “X” button | ✅ Passed | Functional |
| ES-041 | Added product is displayed | ✅ Passed | UI |
| ES-042 | Removing an item from the cart | ✅ Passed | Functional |
| ES-043 | Adding multiple products | ✅ Passed | Functional |
| ES-044 | Adding a product with stock = 0 | ✅ Passed | Functional |
| ES-045 | Correct currency display for products | ❌ Failed | UI |
| ES-046 | Correct calculation of the total amount (Total) | ✅ Passed | Functional |
| ES-047 | Clearing the entire cart using the “Clear” button | ✅ Passed | Functional |

## 2.Quantity Selector

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-048 | Increasing quantity using the “+” button | ✅ Passed | Functional |
| ES-049 | Decreasing quantity using the “–” button | ✅ Passed | Functional |
| ES-050 | Quantity limit according to “Stock” value | ✅ Passed | Functional |

## Checkout ##
## 1.General

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-051 | Checkout form loads | ✅ Passed | Functional |
| ES-052 | Mandatory fields are displayed | ✅ Passed | UI |
| ES-053 | Optional fields are displayed | ✅ Passed | UI |
| ES-054 | Saved data remains filled in | ✅ Passed | Functional |
| ES-055 | Combination of empty fields → error message | ✅ Passed | Functional |
| ES-056 | Order Summary is displayed before confirmation | ✅ Passed | UI |
| ES-057 | Pay button inactive with invalid form | ✅ Passed | Functional |
| ES-058 | Pay button active with valid form | ✅ Passed | Functional |
| ES-059 | “Back to Shop” button works | ✅ Passed | Functional |
| ES-060 | Currency consistency in Checkout | ❌ Failed | UI |
| ES-061 | Green border appears when focusing on a mandatory field | ✅ Passed | UI |
| ES-062 | Empty mandatory field → error message | ✅ Passed | Functional |
| ES-063 | Error message disappears after entering valid values | ✅ Passed | Functional |
| ES-064 | Order Summary displays all entered data, applied discounts, and the final price | ✅ Passed | Functional |

## 2.Field: Name

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-065 | Valid input (≤30 characters) | ✅ Passed | Functional |
| ES-066 | Placeholder for First Name field = “Enter your first name” | ✅ Passed | UI |
| ES-067 | Empty Name field → error message, Pay button inactive | ✅ Passed | Functional |
| ES-068 | Boundary value Name = 30 characters is accepted | ✅ Passed | Functional |
| ES-069 | Enter 31 characters → error message, Pay button inactive | ✅ Passed | Functional |

## 3.Field:Last Name

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-070 | Valid input (≤30 characters) | ✅ Passed | Functional |
| ES-071 | Placeholder for Last Name field = “Enter your last name” | ✅ Passed | UI |
| ES-072 | Empty Last Name field → error message, Pay button inactive | ✅ Passed | Functional |
| ES-073 | Boundary value Last Name = 30 characters is accepted | ✅ Passed | Functional |
| ES-074 | Enter 31 characters → error message, Pay button inactive | ❌ Failed | Functional |

### 4.Field:Street

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-075 | Valid input (<30 characters) | ✅ Passed | Functional |
| ES-076 | Placeholder for Street field = “Enter your street” | ✅ Passed | UI |
| ES-077 | Empty Street field → Pay button inactive | ✅ Passed | Functional |
| ES-078 | Enter 31 characters → error message, Pay button inactive | ✅ Passed | Functional |

## 5.Field:ZIP Code

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-079 | Valid ZIP Code (<30 characters) accepted | ✅ Passed | Functional |
| ES-080 | Placeholder for ZIP Code field = “Enter ZIP code” | ✅ Passed | UI |
| ES-081 | Invalid ZIP Code → error message, Pay button inactive | ✅ Passed | Functional |
| ES-082 | Empty ZIP Code field → error message, Pay button inactive | ✅ Passed | Functional |
| ES-083 | Invalid input (letters, symbols) → error message, Pay button inactive | ❌ Failed | Functional |

## 6.Field: Date of Birth

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-084 | Placeholder for Date of Birth field = “dd.mm.yyyy” | ✅ Passed | UI |
| ES-085 | Field supports mask format dd.mm.yyyy (no other characters allowed) | ✅ Passed | Functional |
| ES-086 | Calendar opens when clicking on the icon | ✅ Passed | Functional |
| ES-087 | Selecting a date from the calendar → field is filled in correct format | ✅ Passed | Functional |
| ES-088 | Manual entry (invalid format, e.g. 99.99.9999) → validation error | ✅ Passed | Functional |
| ES-089 | Manual entry (valid format) → accepted | ✅ Passed | Functional |

## 7.Field: Email

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-090 | Valid email (test@test.com) | ✅ Passed | Functional |
| ES-091 | Placeholder for Email field = “Enter your email” | ✅ Passed | UI |
| ES-092 | Invalid – wrong domain (e.g. test@mail) → error message, Pay button inactive | ✅ Passed | Functional |
| ES-093 | Invalid – missing domain (e.g. test@) → error message, Pay button inactive | ✅ Passed | Functional |
| ES-094 | Invalid – missing @ → error message, Pay button inactive | ✅ Passed | Functional |
| ES-095 | Invalid – multiple @ symbols in address → error message, Pay button inactive | ✅ Passed | Functional |
| ES-096 | Invalid – special characters in invalid places (e.g. test..mail@com) → error message, Pay button inactive | ✅ Passed | Functional |

## 8.Field: Phone

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-097 | Automatic country code prefix | ✅ Passed | Functional |
| ES-098 | Placeholder for Phone Number field = “Enter your phone number” | ✅ Passed | UI |
| ES-099 | Valid number by country (e.g. Slovakia +421 = 9 digits) | ❌ Failed | Functional |
| ES-100 | Empty field → error message, Pay button inactive | ✅ Passed | Functional |
| ES-101 | Short number (less than required digits) → error message, Pay button inactive | ✅ Passed | Functional |
| ES-102 | Long number (more than required digits) → error message, Pay button inactive | ✅ Passed | Functional |
| ES-103 | Letters / special characters → error message, Pay button inactive | ✅ Passed | Functional |

## 9.Discounts

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-104 | Date of birth > 65 years (5% discount) | ❌ Failed | Functional |
| ES-105 | Date of birth = 65 years (5% discount) | ❌ Failed | Functional |
| ES-106 | Date of birth < 65 years (no discount) | ✅ Passed | Functional |
| ES-107 | Checkbox “Student” discount enabled | ✅ Passed | Functional |
| ES-108 | Checkbox “Student” discount disabled | ✅ Passed | Functional |
| ES-109 | Student discount (15%) applied | ✅ Passed | Functional |
| ES-110 | Credit Card payment (5% discount) | ✅ Passed | Functional |
| ES-111 | Cash payment (no discount) | ✅ Passed | Functional |
| ES-112 | PayPal payment (no discount) | ✅ Passed | Functional |

## 10.Coupons

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-113 | Coupon FREESHIP8 → free delivery | ✅ Passed | Functional |
| ES-114 | Placeholder for Coupon Code field = “Enter your code” | ✅ Passed | UI |
| ES-115 | Coupon AUDIO20PC → 20% discount on audio products | ❌ Failed | Functional |
| ES-116 | Coupon FLAT20 → $20 discount | ❌ Failed | Functional |
| ES-117 | Invalid coupon | ✅ Passed | Functional |

## 11.Discount + Coupon combinations

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-118 | Student + Credit Card (15% + 5%) | ✅ Passed | Functional |
| ES-119 | 65+ + Credit Card (5% + 5%) | ✅ Passed | Functional |
| ES-120 | FLAT20 + Credit Card ($20 + 5%) | ❌ Failed | Functional |
| ES-121 | AUDIO20PC + Credit Card (20% + 5%) | ✅ Passed | Functional |
| ES-122 | FREESHIP8 + Credit Card (Free delivery + 5%) | ✅ Passed | Functional |
| ES-123 | Student + 65+ (only bigger discount is applied) | ❌ Failed | Functional |
| ES-124 | Student + FLAT20 | ✅ Passed | Functional |

## 12.Dropdown: Delivery

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-125 | Opening “Delivery Method” dropdown → all delivery options are shown | ✅ Passed | Functional |
| ES-126 | Selecting “Pick up at the branch (Free)” | ✅ Passed | Functional |
| ES-127 | Selecting “Delivery to box ($5)” | ✅ Passed | Functional |
| ES-128 | Selecting “Delivery to home ($15)” | ✅ Passed | Functional |
| ES-129 | Correct delivery price displayed in Order Summary | ✅ Passed | Functional |
| ES-130 | Changing delivery method → recalculation of price in Order Summary | ✅ Passed | Functional |

## 13.Dropdown: Payment Method

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-131 | Opening “Payment Method” dropdown → all payment options are shown | ✅ Passed | Functional |
| ES-132 | Selecting “Credit Card (5% discount)” | ✅ Passed | Functional |
| ES-133 | Selecting “Cash” | ✅ Passed | Functional |
| ES-134 | Correct display of “Payment Method” in Order Summary | ✅ Passed | UI |
| ES-135 | Discount not applied for Cash payment | ✅ Passed | Functional |

## Confirm Page ##

| ID | Summary | Status | Type |
|----|----------|--------|------|
| ES-136 | Confirmation page is displayed | ✅ Passed | Functional |
| ES-137 | Order details are correctly displayed in confirmation | ✅ Passed | UI |
| ES-138 | Correct calculation of the total amount in confirmation | ✅ Passed | Functional |
| ES-139 | Consistent currency and format in confirmation | ❌ Failed | UI |
| ES-140 | “Back to Shop” button works | ✅ Passed | Functional |


🧪 **Environment:** Windows 11, Chrome 140  
📅 **Test Date:** 15–18 September 2025  
👩‍💻 **Tester:** Natalia Chernenkaya
