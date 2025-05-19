# Bug Report: Facebook Mobile App – "People You May Know" Suggestion Repeated Too Frequently in Feed

- **Severity:** Low to Medium (UX/redundancy)  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (iOS-compatible)  
- **Module:** News Feed

---

## Description:

While scrolling the **Facebook News Feed** in the iOS app, the "People You May Know" suggestion card may appear **twice in very close proximity** — sometimes separated by only **one regular post**.  

This behavior appears inconsistent with normal content distribution and may indicate a **duplication error** during feed assembly or loading.

Typically, such suggestions should appear **infrequently and spaced out**, possibly every 50+ items, to avoid user fatigue or visual clutter.

---

## Steps to Reproduce:

1. Open Facebook app (v513.0.0) on iOS 18.3.2  
2. Scroll through the **News Feed**  
3. Observe when the **“People You May Know”** suggestion appears  
4. In some cases, it appears again **after just one or two regular posts**  
5. Both cards have similar or identical structure and layout

---

## Expected Result:

- "People You May Know" block should be shown **only once per feed chunk**  
- Frequency should be **regulated by a logic gate** (e.g., every X posts or scroll depth)  
- Content generation system should **avoid duplicate modules in close proximity**

---

## Actual Result:

- Suggestion appears **twice within 3 consecutive posts**  
- Creates a **repetitive experience** and undermines feed diversity  
- May be caused by **duplicate entries during feed loading or caching**

---

## Environment:

- Device: iPhone SE / iPhone 12 / iPhone 14  
- iOS: 18.3.2  
- Facebook App Version: 513.0.0  
- Language: Russian  
- Internet: Stable Wi-Fi and LTE  
- Reproducibility: Intermittent (occurs randomly during feed refresh)

---

## Evidence:

- Video 

https://github.com/user-attachments/assets/87b98663-3c0a-4356-966e-9c2a118100ef



---

## Notes:

This could be caused by:
- A **lack of deduplication logic** in the feed rendering process  
- Improper synchronization during **partial data loads or cache merges**  
- Frontend not validating that “suggestion” modules are spaced correctly

Suggested Fix:
- Implement **post-load validation** for suggestion-type modules  
- Enforce a **minimum distance rule** between duplicate UI blocks of the same type

---

## User Impact:

- Reduces trust in content curation  
- Creates impression of **buggy or low-effort personalization**  
- Contributes to content fatigue and may reduce engagement
