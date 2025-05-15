# Bug Report: Google Developers – "Terms" Page Not Translated While Site Language Is Set

- **Severity:** Medium  
- **Platform:** Desktop  
- **Browser:** Google Chrome Version 136.0.7103.114 (64-bit)  
- **Operating System:** Windows 10 / 11  
- **Tested Site:** https://developers.google.com/youtube?hl=ru  
- **Language Setting:** Russian (applies to German, Spanish, etc.)

---

## Description:

On the Google Developers YouTube API site, when opened with the language setting set to **Russian** (`hl=ru`), the entire interface and navigation (Home, Guides, Samples, etc.) are displayed in Russian — **except for the “Terms” page**.  

Clicking on the “Условия” tab opens a page that loads entirely in **English**, with **no automatic translation** or localized content — even though the rest of the site is localized.

However, if the user navigates within that section (e.g., clicks **Branding Guidelines**), the language **switches back to Russian**. This inconsistent behavior exists in other languages as well (e.g., German, Spanish).

---

## Steps to Reproduce:

1. Open Google Chrome (v136.0.7103.114, 64-bit)  
2. Go to: https://developers.google.com/youtube?hl=ru  
3. Observe that the interface is in Russian  
4. Click on the “Условия” (Terms) tab in the header menu  
5. The Terms page opens in **English**, breaking localization  
6. Now click on **Branding Guidelines** inside the same section  
7. The page returns to **Russian language**

---

## Expected Result:

The “Terms” page should either:
- Be displayed in **Russian** (matching other content),  
- Or display a message: “This page is only available in English” for clarity.

Automatic translation behavior should be **consistent** with the rest of the site.

---

## Actual Result:

- The “Terms” page is shown **in English**, even though the language parameter is set to `hl=ru`.  
- No message explains this behavior.  
- Sub-pages within the same section revert to the correct language.

---

## Environment:

- Browser: Google Chrome 136.0.7103.114 (64-bit)  
- OS: Windows 10 / 11  
- Site: https://developers.google.com/youtube  
- Language: Russian (`hl=ru`), also reproducible in German (`hl=de`), Spanish (`hl=es`), etc.

---

## Evidence:

- Screenshot: ![Снимок экрана 2025-05-15 151558](https://github.com/user-attachments/assets/b0c2599e-401a-4741-8c5a-5d2c35ec851d)
![Снимок экрана 2025-05-15 151635](https://github.com/user-attachments/assets/78d353ab-8b11-41f8-803f-48aec76f43e3)
![Снимок экрана 2025-05-15 152610](https://github.com/user-attachments/assets/9098e49c-9c64-426d-855a-d8d067519872)



---

## Notes:

This is likely a **deliberate exception** — perhaps for legal or compliance reasons — to ensure that **Terms & Conditions are interpreted only in their original English form**, avoiding translation misinterpretation.

If so, this behavior should be **explicitly indicated**, as it currently appears to be a **broken translation or incomplete localization** to the average user.

