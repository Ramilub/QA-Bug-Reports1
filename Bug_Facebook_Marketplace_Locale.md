# Bug Report: Facebook Marketplace – Language Localization Issue in Search Filter

- **Severity:** Low  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (iOS-compatible)

---

## Description:
In the **Russian-language version** of the Facebook app, when performing a search in the **Marketplace** section, a list of filters appears automatically under the search bar.

All filters are displayed in **Russian**, except for the **first filter**, which is labeled **“Distance”** (in English). However, when you open this filter, all internal content is properly translated to Russian.

This inconsistency suggests a **localization defect** — a missing translation string for this particular filter label.

---

## Steps to Reproduce:

1. Open the Facebook app (version 513.0.0) on iOS 18.3.2  
2. Set the app language to **Russian**  
3. Go to the **Marketplace** section  
4. Tap on the **search bar** and enter any keyword (e.g., "highlander hybrid", "телефон")  
5. Observe the filters that appear below the search field ![51667](https://github.com/user-attachments/assets/0d00d3e0-1df6-46f2-88aa-90a876887f4f)
 
6. The **first filter says “Distance”** (in English), while all other filters are in Russian  
7. Tap on the “Distance” filter — all content inside is in Russian

---

## Expected Result:
All filters, including the first one, should be displayed in **Russian**.  
The word “Distance” should be shown as **“Расстояние”**.

---

## Actual Result:
The first filter appears as “Distance” (in English) in a Russian-language interface, which breaks UI consistency.

---

## Environment:
- iOS Version: 18.3.2  
- Facebook App Version: 513.0.0  
- App Language: Russian

---

## Evidence:
*Screenshot recommended: `![99485](https://github.com/user-attachments/assets/6d70856d-abea-4463-bb92-847f4ed80f97)`*

---

## Notes:
This is a **minor but visible localization bug** that may affect user trust and UX quality for non-English users.
