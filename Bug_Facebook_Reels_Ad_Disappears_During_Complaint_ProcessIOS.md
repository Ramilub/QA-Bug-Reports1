# Bug Report: Facebook Reels – Ad Disappears If Complaint Process Is Not Completed

- **Severity:** Medium (UX, user trust, ad reporting integrity)  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 515.0.0  
- **Device:** iPhone SE / iPhone 12 / iPhone 14  
- **Module:** Reels → Ad Reporting

---

## Description:

When watching **Facebook Reels**, and encountering an **ad in video format**, tapping the **three-dot menu (•••)** and selecting **“Report Ad”** opens a reporting submenu.  

However, if the user **does not complete the report** (e.g., closes the submenu or scrolls away without choosing a reason), the ad **disappears from the feed immediately**.  

It becomes **impossible to view or report it again at that moment**, yet the **same ad reappears later** during regular scrolling.

This creates the impression that:
- **Facebook forcibly removes the ad from view** during reporting
- The user’s right to evaluate or reconsider reporting is **interrupted**
- There is a **bias in favor of ad delivery over user experience**

---

## Steps to Reproduce:

1. Open Facebook (v515.0.0) on iOS 18.3.2  
2. Scroll through **Reels** until a **sponsored ad** appears (in video format)  
3. Tap **three dots** on the ad → Select **"Report Ad"**  
4. Do **not** choose a reason or complete the report  
5. Close the submenu or tap outside  
6. The ad immediately **disappears from the feed**  
7. Attempt to go back and find the ad – it’s gone  
8. Scroll further → The same ad may reappear much later

---

## Expected Result:

- The ad should **remain visible** until the report is **fully completed or canceled**  
- The user should have a chance to **reopen the menu**, **review options**, or **change their mind**  
- No ad should disappear unless **intentionally removed by the user or moderation logic**

---

## Actual Result:

- The ad **vanishes prematurely** during the initial stage of reporting  
- User loses the ability to **review or finalize complaint**  
- Feels like the app **prioritizes ad display over user feedback**

---

## Environment:

- Device: iPhone SE / iPhone 12 / iPhone 14  
- OS: iOS 18.3.2  
- Facebook App Version: 515.0.0  
- Reproducibility: Frequent  
- Network: Wi-Fi / LTE – Irrelevant  
- Language: Russian (but UI-independent)

---

## Evidence:

- Video Proof: 

https://github.com/user-attachments/assets/fa6b2224-11d4-459d-b519-4674cac14a93


---

## Notes:

This may be caused by:
- An **auto-dismiss trigger** connected to the reporting flow  
- Premature **ad queue rotation** or **cache invalidation** after entering report mode  
- Lack of state-check for **incomplete reporting actions**

---

## Suggested Fix:

- Keep the ad visible until the user **completes or cancels** the complaint  
- Add a **"Back" or "Cancel"** button in the report submenu  
- Allow user to **re-enter report flow** without losing access to the ad

---

## User Impact:

- Breaks **trust in the integrity of the reporting system**  
- Creates suspicion that **Facebook limits user agency** in favor of advertisers  
- Reduces user willingness to **engage with Reels ads critically**  
- Harms perception of Facebook as a **neutral platform**

