# Bug Report: Facebook Marketplace – Incorrect Display of Quotation Mark Entities in Russian Language Interface

- **Severity:** Medium  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (iOS-compatible)  
- **Language:** Russian  
- **Module:** Messenger → Marketplace → Chat → Item status buttons

---

## Description:

In the **Facebook app** (v513.0.0), when navigating to **Messenger > Marketplace > Chat with buyer**, a user may encounter **malformed system text** related to item status (e.g., “Sold”, “On Hold”).  

Specifically, buttons appear with **HTML-encoded quotation marks** instead of proper formatting.

Examples:
- `"Отметить как &quot;отложено&quot;”`  
- `"Отметить как &quot;продано&quot;"`

These strings clearly expose **raw entity codes** (e.g., `&quot;`) instead of properly rendering them as quotation marks `"`.

---

## Steps to Reproduce:

1. Open the Facebook app (v513.0.0) on iOS 18.3.2  
2. Go to **Messenger** from the main menu  
3. Select **Marketplace** conversations  
4. Open any chat with a buyer of your listed product  
5. If the item is marked as sold or held, observe the status button:  
   - It says: **“Отметить как &quot;отложено&quot;”**  
6. Tap the button → See action list → another option appears:  
   - **“Отметить как &quot;продано&quot;"**

---

## Expected Result:

- Buttons and actions should display **clean, localized text**  
- Quotation marks should appear as **“продано”**, **“отложено”**, not as raw code  
- All strings should be properly **decoded before rendering**

---

## Actual Result:

- HTML entities (`&quot;`) are **visible to users**  
- UI appears **unfinished or poorly localized**  
- Reduces trust in **interface quality and app professionalism**

---

## Environment:

- Device: iPhone SE  
- iOS: 18.3.2  
- Facebook App Version: 513.0.0  
- App Language: Russian  
- Module: Messenger > Marketplace chat  
- Reproducibility: Consistent if Marketplace item is in processed status (sold/held)

---

## Evidence:

- Screenshot: ![IMG_1176](https://github.com/user-attachments/assets/fa5f391b-4e1c-4929-98d5-428d7cc28dc1)
![IMG_1177](https://github.com/user-attachments/assets/71e69e16-4305-4c5f-b7ec-dd608154a7da)

---

## Notes:

This is a classic **HTML entity decoding bug**:
- Text is likely rendered from a database or localization file without passing through an HTML/Unicode decode layer
- Could affect **multiple languages** if reused across interfaces

Suggested fix:
- Pass all dynamic UI strings through an HTML entity decoding function before rendering to UI

---

## User Impact:

- Reduces perceived **professionalism and quality** of the app  
- Creates **distrust** during financial interactions (selling items)  
- Makes the app feel **unpolished or “fake”** to Russian-speaking users  
- May lead to hesitation in continuing transactions

