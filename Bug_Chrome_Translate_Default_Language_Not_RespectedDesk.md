# Bug Report: Google Chrome – Default Translate Target Language Not Respected

- **Severity:** Medium (UX inconsistency / accessibility issue)  
- **Platform:** Google Chrome Version 137.0.7151.69 (Official Build) (64-bit)  
- **OS:** Windows 11  
- **Module:** Google Translate built-in integration  
- **Languages:** Source: English / Target: Russian  
- **Reproducibility:** 100%

---

## Description:

When browsing **English-language websites** in **Google Chrome**, using the **built-in Translate feature** does not correctly follow the **user-defined default translation target** (in this case, **Russian**).

Despite Chrome’s settings being configured to **auto-translate English to Russian**, the popup window always **defaults to English → English**, forcing the user to **manually select "Russian" every time** they use Translate.

This behavior repeats **on every new website**, even within the **same browsing session**, breaking the expectation of **persistent language preferences**.

---

## Steps to Reproduce:

1. Open Chrome (v137.0.7151.69) on Windows 11  
2. Set Chrome display language to **Russian** (or any non-English language)  
3. Navigate to an English-language website (e.g., (https://www.cbsnews.com/sacramento/))  
4. Click the **three-dot menu** → **Translate**  
5. Observe that the **Translate popup defaults to English → English**  
6. Manually change the target language to **Russian**  
7. Visit another English website → Repeat steps → Observe that **settings are not saved**

---

## Expected Result:

- Chrome should **remember** that the user wants **English → Russian translation**  
- Once set, this preference should be **applied globally across browsing sessions**  
- The popup should **default to Russian** as the translation target for English content

---

## Actual Result:

- Translate always shows **English → English** in the popup, regardless of user settings  
- User must **manually select Russian** every time  
- Language setting does **not persist** across websites  
- Breaks **workflow**, especially for users relying on translation for accessibility

---

## Environment:

- Browser: Google Chrome v137.0.7151.69 (64-bit)  
- OS: Windows 11  
- Display Language: Russian  
- Chrome Settings:  
  - "Offer to translate pages that aren’t in a language you read" → Enabled  
  - Preferred translation target: Russian  
- Reproducibility: Every time

---

## Notes:

- This may be caused by improper **local storage or profile sync of language preferences**  
- Likely related to the **Translate extension or embedded module**, failing to persist the previous selection  
- The issue severely impacts **non-English-speaking users** and disrupts smooth browsing

---

## Suggested Fix:

- Ensure Translate remembers the **last used language pair** per session or per user  
- Use Chrome profile settings to **respect user-defined target language automatically**  
- Add option to **lock translation pair** (e.g., “Always translate English → Russian”)

---

## User Impact:

- Causes **repetitive manual input** for users reading foreign websites  
- Undermines **accessibility** and ease-of-use  
- Reduces trust in **browser intelligence and customization**  
- Particularly frustrating for users relying on **non-native interfaces** or working internationally

---

## Evidence:

- Screenshot: ![Снимок экрана 2025-06-03 004302](https://github.com/user-attachments/assets/0d33912d-38d4-4f83-ae41-bfab46332f76)
![Снимок экрана 2025-06-03 004315](https://github.com/user-attachments/assets/4fec99d3-0dde-45b5-9df1-bb42fd7f8af9)
![Снимок экрана 2025-06-03 004344](https://github.com/user-attachments/assets/f4e4bef1-9d2c-4718-8252-98e53bb8d44a)
![Снимок экрана 2025-06-03 004418](https://github.com/user-attachments/assets/be734138-715d-4f07-b511-bfdfe15e1801)
![Снимок экрана 2025-06-03 004447](https://github.com/user-attachments/assets/8644e4fe-7c83-488e-a04e-0e38501f030e)
![Снимок экрана 2025-06-03 004838](https://github.com/user-attachments/assets/00d2929b-e33f-44bf-a70c-d11e1168d873)

