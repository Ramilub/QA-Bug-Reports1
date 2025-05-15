# Bug Report: Facebook Marketplace – Filtered Item Count Does Not Match Actual Results

- **Severity:** Medium  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone 12 / etc.

---

## Description:
In the Russian-language version of Facebook (v513.0.0), when applying advanced filters in the **Marketplace**, the application **shows a misleading number of available listings**.  

Specifically, the number of listings displayed on the **“See items”** button does **not match** the actual number of search results shown after pressing it.

---

## Steps to Reproduce:

1. Open the Facebook app on iOS (18.3.2), version 513.0.0  
2. Navigate to the **Marketplace**  
3. Tap the **search bar** and enter a keyword (or no keyword)  
4. Apply the following filters:
   - **Sort by**: Recommendations  
   - **Price**: from $6000 to $12000  
   - **Make**: Toyota  
   - **Model**: Highlander Hybrid  
5. At the bottom of the screen, observe the text on the blue button:  
   → **"Смотреть товары (14)"** *(View items (14))*
6. Tap on the button to view the results
7. The actual number of listings shown is **only 4**

---

## Expected Result:
The number shown on the “View items” button should **accurately reflect** the real number of listings matching the active filters.

---

## Actual Result:
The button claims **14 items** are available, but only **4 listings** are actually shown. This creates **confusion** and **loss of trust** in filter accuracy.

---

## Environment:
- Device: iPhone  
- iOS Version: 18.3.2  
- Facebook App Version: 513.0.0  
- Language: Russian  
- Internet: Stable Wi-Fi / LTE  

---

## Evidence:
- - Screenshot filename:
  - ![IMG_1124](https://github.com/user-attachments/assets/70ad88eb-2d4c-48d5-bc7e-2fc840a73c25)
  - ![IMG_1122](https://github.com/user-attachments/assets/5da34b87-cc7f-4af3-b51e-851338fcdc03)


## Notes:
This appears to be a **backend or indexing issue**, where the filter engine counts items incorrectly, or cached values are not refreshed before display.  
It negatively impacts user experience and trust in the Marketplace filtering system.

