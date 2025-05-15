# Bug Report: Facebook Marketplace – Unable to Enter Price Range in Filters

- **Severity:** High  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (iOS-compatible)

---

## Description:
In the **Facebook Marketplace** (Russian language interface), when attempting to search for "Highlander Hybrid" and then use the **price filter**, the app **does not allow the user to enter a valid price range**.  

Only one digit is accepted in the price input fields (e.g., “6”), and any attempt to enter more digits results in:
- The field being automatically cleared  
- Or the second digit not being registered at all  

This makes it **impossible to filter listings by price**, which is a critical feature in the Marketplace.

---

## Steps to Reproduce:

1. Open Facebook app (v513.0.0) on iOS 18.3.2  
2. Navigate to **Marketplace**  
3. Tap the **search bar** and enter: `Highlander Hybrid`  
4. Tap the **Filters** button  
5. Try to input a price range in the “Price from” or “Price to” fields  
6. Attempt to type a value like `6000` or `12000`

---

## Expected Result:
User should be able to enter **any numeric value** into the price range fields (e.g., 6000–12000), and the app should filter results accordingly.

---

## Actual Result:
Only the **first digit** is accepted. Further digits are either **cleared automatically** or not registered at all.  
This **prevents price-based filtering completely**.

---

## Environment:
- Device: iPhone  
- iOS Version: 18.3.2  
- Facebook App Version: 513.0.0  
- App Language: Russian  
- Input Locale: Russian or English (tested both)

---

## Evidence:
- **Video proof available:** 

https://github.com/user-attachments/assets/3b61b95a-bbfd-4d2d-87e4-e50e2f0a77b9

  
*(shows inability to enter a full price)*

---

## Notes:
This appears to be a **UI input field bug**, possibly caused by a localization issue or validation script conflict in the Russian version.  
This bug affects core functionality and creates **critical UX failure** in search filtering.

