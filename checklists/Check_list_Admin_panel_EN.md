#  Demo E-Shop – Admin Panel Test Checklist (EN)

This document contains a complete checklist of manual test cases for the **Admin Panel** of the Demo E-Shop web application.  
It includes validation of all core functionalities: product management, data consistency, and UI behavior.

## Add Product Form ##
## 1. General Checks

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-001 | Opening the “Add Product” form (click the button) | ✅ Passed | Functional |
| AP-002 | Closing the form using the “X” icon | ❌ Failed | Functional |
| AP-003 | Functionality of the “Cancel” button (after filling in required fields) | ✅ Passed | Functional |
| AP-004 | Adding a product with all required fields filled in | ✅ Passed | Functional |
| AP-005 | Adding a product with both required and optional fields (Color, Brand, Description) filled in | ✅ Passed | Functional |
| AP-006 | Highlighting of required fields on focus (Name, Category, Price, Stock, Image) | ✅ Passed | UI/UX |

## 2️ Field: Name

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-007 | Enter a valid product name (e.g. “Smartphone X100”) → product is saved | ✅ Passed | Functional |
| AP-008 | Focus on the Name field → field border highlights in green | ✅ Passed | UI/UX |
| AP-009 | Placeholder text in the Name field = “Enter product name” | ✅ Passed | UI/UX |
| AP-010 | Very short name (1 character) → product is saved | ✅ Passed | Functional |
| AP-011 | Leave the Name field empty → validation error message is displayed | ✅ Passed | Functional |
| AP-012 | Very long name (>255 characters) → error or text truncated (not defined in requirements) | ⚪ Skipped | Functional |
| AP-013 | Duplicate Name (same as existing product) → product is saved | ✅ Passed | Functional |
| AP-014 | Special characters / emojis in Name → error or validation (not defined in requirements) | ✅ Passed | Functional |
| AP-015 | Only spaces entered → validation error displayed | ❌ Failed | Functional |
| AP-016 | Incorrect or empty required field → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |

## 3️ Dropdown: Category

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-017 | Open the Category dropdown → list of available categories is displayed | ✅ Passed | Functional |
| AP-018 | Focus on the Category field → field border highlights in green | ✅ Passed | UI/UX |
| AP-019 | Placeholder text in the Category field = “Select a category” | ✅ Passed | UI/UX |
| AP-020 | Select a category from the dropdown → selected category is displayed in the field | ✅ Passed | Functional |
| AP-021 | Leave the Category field empty → validation modal “Please fill in all required fields correctly” appears | ✅ Passed | Functional |

## 4️ Field: Price

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-022 | Enter a valid price → value accepted | ✅ Passed | Functional |
| AP-023 | Focus on the Price field → field border highlights in green | ✅ Passed | UI/UX |
| AP-024 | Placeholder text in the Price field = “Enter price” | ✅ Passed | UI/UX |
| AP-025 | Leave the Price field empty → validation modal “Please fill in all required fields correctly” appears | ✅ Passed | Functional |
| AP-026 | Very large value (e.g. 1e18) → check for overflow or error (not defined in requirements) | ❌ Failed | Functional |
| AP-027 | Negative value (–1) → validation modal “Please fill in all required fields correctly” appears | ✅ Passed | Functional |
| AP-028 | Decimal number (0.99) → value accepted | ✅ Passed | Functional |
| AP-029 | Non-numeric input (abc) → cannot be entered | ✅ Passed | Functional |
| AP-030 | Adjust value using ↑/↓ arrows → correct change by 0.5 | ✅ Passed | Functional |
| AP-031 | Price with leading zeros (005) → saved as 5 | ✅ Passed | Functional |

## 5️ Field: Stock

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-032 | Enter a valid stock value → value accepted | ✅ Passed | Functional |
| AP-033 | Focus on the Stock field → field border highlights in green | ✅ Passed | UI/UX |
| AP-034 | Placeholder text in the Stock field = “Enter stock quantity” | ✅ Passed | UI/UX |
| AP-035 | Leave the Stock field empty → validation modal “Please fill in all required fields correctly” appears | ❌ Failed | Functional |
| AP-036 | Stock = 0 → value accepted | ✅ Passed | Functional |
| AP-037 | Very large stock value (e.g. 1,000,000,000) → saved and displayed correctly | ✅ Passed | Functional |
| AP-038 | Decimal value (0.5) → validation error, product not created | ❌ Failed | Functional |
| AP-039 | Negative value (–5) → validation modal “Please fill in all required fields correctly” appears | ✅ Passed | Functional |
| AP-040 | Non-numeric input (###) → cannot be entered | ✅ Passed | Functional |
| AP-041 | Numeric stepper ↑/↓ → values change by 1 | ✅ Passed | Functional |


## 6️ Dropdown: Image

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-042 | Open the Image dropdown → list of available images is displayed | ✅ Passed | Functional |
| AP-043 | Focus on the Image field → field border highlights in green | ✅ Passed | UI/UX |
| AP-044 | Placeholder text in the Image field = “Select an image” | ✅ Passed | UI/UX |
| AP-045 | Select an image from the dropdown → selected image is displayed in the field | ✅ Passed | Functional |
| AP-046 | Selected image saved → product is added and image appears on the product card | ✅ Passed | Functional |
| AP-047 | Leave the Image field empty → validation modal “Please fill in all required fields correctly” appears | ✅ Passed | Functional |

## 7️ Optional Fields (Brand, Color, Description)

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-048 | Enter a value in the Brand field → saved and displayed correctly | ✅ Passed | Functional |
| AP-049 | Placeholder text in the Brand field (optional) = “Enter brand” | ✅ Passed | UI/UX |
| AP-050 | Placeholder text in the Color field (optional) = “Enter color” | ✅ Passed | UI/UX |
| AP-051 | Enter a value in the Color field → saved and displayed correctly | ✅ Passed | Functional |
| AP-052 | Placeholder text in the Description field (optional) = “Enter description” | ✅ Passed | UI/UX |
| AP-053 | Enter a value in the Description field → saved and displayed correctly | ✅ Passed | Functional |

## 8️ Button:Export to Excel 

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-054 | Display of “Export to Excel” button → button is visible and clickable | ✅ Passed | UI/Functional |
| AP-055 | Successful export of Excel file → *.xlsx file downloads and opens without errors | ✅ Passed | Functional |
| AP-056 | Correct file name → file has meaningful name (e.g., products.xlsx) | ✅ Passed | Functional |
| AP-057 | Table structure and mandatory fields are correct | ✅ Passed | Functional |
| AP-058 | Data–header consistency → values correspond to headers (Stock → numbers, Color → text) | ❌ Failed | Functional |
| AP-059 | Data format → numeric fields (Price, Stock) are numbers, text fields (Name, Description) are text | ✅ Passed | Functional |
| AP-060 | Data freshness → newly added product appears in export | ❌ Failed | Functional |
| AP-061 | Export of optional fields → Brand, Color, Description are included in export | ✅ Passed | Functional |
| AP-062 | Long strings → long Name/Description are fully saved in Excel | ✅ Passed | Functional |
| AP-063 | Export with no products → empty Excel file created | ✅ Passed | Functional |
| AP-064 | Export with 100+ products → export successful | ✅ Passed | Performance |
| AP-065 | UI after export → Admin panel remains fully functional | ✅ Passed | Stability |
| AP-066 | File encoding → Czech characters displayed correctly | ✅ Passed | Functional |

## 9️ Button:Back to Shop 

| ID | Summary | Status | Type |
|----|----------|---------|------|
| AP-067 | Display of “Back to Shop” button → button is visible and clickable | ✅ Passed | UI/Functional |
| AP-068 | Functionality of “Back to Shop” → redirects to e-shop, correct URL opens | ✅ Passed | Functional |
| AP-069 | Back navigation → Admin panel reopens without re-login | ✅ Passed | Functional |
| AP-070 | Content validation → Admin panel content remains correct after returning | ✅ Passed | Stability |


##  Edit Product Form

### 1️ Modal Content

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-001 | Open the “Edit” form (click Edit button) | ✅ Passed | Functional |
| ED-002 | Close the form using the “X” icon | ✅ Passed | UI |
| ED-003 | Functionality of “Cancel” button (after filling required fields) | ✅ Passed | Functional |
| ED-004 | Update product with all required fields filled | ✅ Passed | Functional |
| ED-005 | Update product with both required and optional fields (Color, Brand, Description) | ✅ Passed | Functional |
| ED-006 | Highlighting of required fields on focus (Name, Category, Price, Stock, Image) | ✅ Passed | UI |
| ED-007 | Update with no changes → product remains unchanged | ✅ Passed | Functional |


### 2️ Field: Name

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-008 | Change Name value → product saved with new name | ✅ Passed | Functional |
| ED-009 | Focus on Name field → field border highlights in green | ✅ Passed | UI |
| ED-010 | Change to short Name (1 character) → product saved | ✅ Passed | Functional |
| ED-011 | Change to empty Name → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |
| ED-012 | Long Name (>255 characters) → error or truncation (not defined in requirements) | ❌ Failed | Functional |
| ED-013 | Duplicate Name (same as existing product) → product saved | ✅ Passed | Functional |
| ED-014 | Change to special characters / emoji → validation behavior not defined | ⚪ Skipped | Functional |
| ED-015 | Change to spaces only → validation modal “Please fill in all required fields correctly” | ❌ Failed | Functional |
| ED-016 | Incorrect or empty input → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |


### 3️ Dropdown: Category

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-017 | Open dropdown → list of available categories displayed | ✅ Passed | UI |
| ED-018 | Focus on Category field → field border highlights in green | ✅ Passed | UI |
| ED-019 | Change category from dropdown → selected category displayed in the field | ✅ Passed | Functional |
| ED-020 | Empty Category field → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |


### 4️ Field: Price

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-021 | Change to valid price → accepted | ✅ Passed | Functional |
| ED-022 | Focus on Price field → field border highlights in green | ✅ Passed | UI |
| ED-023 | Empty Price field → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |
| ED-024 | Very large value (e.g. 100000000000000000) → no overflow error | ✅ Passed | Functional |
| ED-025 | Negative value (–1) → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |
| ED-026 | Non-numeric characters (abc) → cannot be entered | ✅ Passed | Functional |
| ED-027 | Change Price using numeric stepper ↑↓ → incorrect increment by 0.5 | ❌ Failed | Functional |
| ED-028 | Price with leading zeros (005) → saved as 5 | ❌ Failed | Functional |


### 5️ Field: Stock

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-029 | Change Stock to empty field → validation modal “Please fill in all required fields correctly” | ❌ Failed | Functional |
| ED-030 | Focus on Stock field → field border highlights in green | ✅ Passed | UI |
| ED-031 | Change Stock to 0 → accepted | ✅ Passed | Functional |
| ED-032 | Change Stock to large value (e.g. 1,000,000,000) → saved and displayed correctly | ❌ Failed | Functional |
| ED-033 | Change Stock to decimal value (0.5) → validation error, product not saved | ❌ Failed | Functional |
| ED-034 | Change Stock to negative value (–5) → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |
| ED-035 | Change Stock to non-numeric characters (###) → cannot be entered | ✅ Passed | Functional |
| ED-036 | Change Stock using numeric stepper ↑↓ → values change by 1 | ✅ Passed | Functional |


### 6️ Dropdown: Image

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-037 | Open dropdown → list of available images displayed | ✅ Passed | UI |
| ED-038 | Focus on Image field → field border highlights in green | ✅ Passed | UI |
| ED-039 | Change image from dropdown → selected image displayed | ✅ Passed | Functional |
| ED-040 | Changed image saved → product updated and displayed correctly | ✅ Passed | Functional |
| ED-041 | Change image to empty field → validation modal “Please fill in all required fields correctly” | ✅ Passed | Functional |


### 7️ Optional Fields

| ID | Summary | Status | Type |
|----|----------|---------|------|
| ED-042 | Change Brand → product updated successfully | ✅ Passed | Functional |
| ED-043 | Change Color (add/edit/delete value) → product updated successfully | ✅ Passed | Functional |
| ED-044 | Change Description (delete and add new text) → product updated successfully | ✅ Passed | Functional |


##  Remove Button

| ID | Summary | Status | Type |
|----|----------|---------|------|
| RM-001 | Display of “Remove” button → button is visible and clickable | ✅ Passed | UI/Functional |
| RM-002 | Opening confirmation modal → modal displays text “Are you sure you want to remove this product?” with OK / Cancel buttons | ✅ Passed | UI/Functional |
| RM-003 | Cancel product removal → product remains in the list | ✅ Passed | Functional |
| RM-004 | Confirm product removal (OK) → product removed and no longer displayed in Admin panel | ✅ Passed | Functional |
| RM-005 | UI after removal → product list refreshes correctly | ✅ Passed | UI/Stability |
| RM-006 | Removing the last product in the list → empty list displayed correctly | ✅ Passed | Functional |


##  Integration Cases

| ID | Summary | Status | Type |
|----|----------|---------|------|
| IN-001 | Add new product → product appears in the Shop catalog | ✅ Passed | Integration |
| IN-002 | Edit product → changes visible in the Shop | ✅ Passed | Integration |
| IN-003 | Delete product → removed product no longer visible in the Shop | ✅ Passed | Integration |
| IN-004 | Stock synchronization after purchase → stock values decrease in Admin Panel | ✅ Passed | Integration |






