# Bug Report: Google Chrome – "Show Bookmarks Bar" Toggle Does Not Work Properly

- **Severity:** Medium (UI bug with privacy and UX implications)  
- **Platform:** Google Chrome Version: 137.0.7151.69 (Official Build) (64-bit)  
- **OS:** Windows 11  
- **Reproducibility:** 100%  
- **Language:** Russian (reproducible in all languages)  
- **Module:** Bookmarks Bar UI

---

## Description:

In the latest version of Google Chrome for Windows, the **"Show bookmarks bar"** toggle in the context menu **fails to function correctly**.

When the user:
- **Right-clicks** on a tab or the empty space near the tabs
- Selects or deselects the **"Show bookmarks bar"** option

…the **bookmarks bar remains visible** even when **unchecked**. Enabling the option shows the bar (as expected), but **disabling it has no effect** — the bar stays visible.

This defeats the purpose of the toggle and creates frustration, especially for users concerned with **visual clarity or privacy**.

---

## Steps to Reproduce:

1. Open Google Chrome (v137.0.7151.69) on Windows 11  
2. Make sure you have **saved bookmarks visible** on the bookmarks bar  
3. Right-click anywhere in the **tab area**  
4. Uncheck the **“Show bookmarks bar”** option  
5. Observe that the **bookmarks bar is still visible**  
6. Try toggling it on/off again – no change unless browser is restarted

---

## Expected Result:

- When the user **disables** the “Show bookmarks bar” option, the bar should **immediately disappear**
- The setting should take **instant effect**, matching historical Chrome behavior

---

## Actual Result:

- The toggle has **no effect**  
- The bookmarks bar **remains visible even when disabled**  
- The user is **unable to hide personal or sensitive bookmarks**

---

## Environment:

- Browser: Google Chrome 137.0.7151.69 (64-bit)  
- OS: Windows 11  
- Display: 1920x1080  
- Extensions: None active (same result with all disabled)  
- Bookmarks: Present (personal)

---

## Evidence:

- Screenshot: ![Снимок экрана 2025-06-03 010315](https://github.com/user-attachments/assets/cdfb4b57-83a4-4b64-935c-3901d37c724a)
![Снимок экрана 2025-06-03 010333](https://github.com/user-attachments/assets/71ef4e65-b018-4632-b7bd-1c7584c28833)
![Снимок экрана 2025-06-03 010358](https://github.com/user-attachments/assets/7e48f036-5515-4408-83b4-2e5ade5191e8)


---

## Notes:

- May be caused by regression in UI state handling or rendering layer  
- Possibly connected to recent changes in tab layout or unified side panel logic  
- Also reproducible with **Ctrl+Shift+B** shortcut — bar does not disappear

---

## Suggested Fix:

- Audit toggle behavior for bookmarks bar  
- Ensure UI state updates upon click and reflects real setting in chrome://settings  
- Add fallback detection to force-hide bar when deselected

---

## User Impact:

- **Loss of privacy** when screen sharing or presenting (users may expose bookmarks unintentionally)  
- Feels like the **browser is ignoring user control**  
- May reduce **trust in Chrome's UI quality**  
- Can lead to users **switching browsers** due to perceived bloat or lack of refinement

---

## Business Impact:

- Chrome is known for **clean, minimalist UX** – bugs like this damage brand image  
- Power users may shift to competitors like Firefox or Edge due to **UI control issues**

