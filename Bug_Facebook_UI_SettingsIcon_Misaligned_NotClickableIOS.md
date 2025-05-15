# Bug Report: Facebook – Misaligned and Non-functional Settings Icon in Support Inbox Subsections

- **Severity:** Medium  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (any iOS-compatible device)

---

## Description:
In the Facebook app, when accessing the **Support Inbox subsections**, the **settings icon (⚙️ gear icon)** is **misaligned and non-functional**.

While the gear icon appears normally and works in the main “Support Inbox” screen, it becomes **visually broken and unclickable** in the following sections:
- “Your Alerts”
- “Reports About Others”

The icon shifts too far to the right, displaying only **half its size**, and **tapping it has no effect**. This creates both a **UI issue and functional loss**.

---

## Steps to Reproduce:

1. Open the Facebook app (v513.0.0) on iOS 18.3.2  
2. Tap the **menu icon** (three lines at bottom right)  
3. Select **Help & Support**  
4. Tap **Support Inbox**  
5. Observe the gear icon – it is correctly placed and functional  
6. Now tap **Your Alerts** or **Reports About Others**  
7. Observe the gear icon:
   - It is **pushed too far right**
   - Only partially visible (clipped)
   - **Tapping it does nothing**

---

## Expected Result:
- The gear icon should be **fully visible and correctly aligned**
- It should **respond to tap**, either opening a settings menu or be removed entirely if not intended to function here

---

## Actual Result:
- The gear icon is **partially hidden**, misaligned toward the screen edge  
- It is **non-functional** — does not respond to tap  
- This **breaks UI consistency and creates confusion** for users

---

## Environment:
- Device: iPhone SE  
- iOS Version: 18.3.2  
- Facebook Version: 513.0.0  
- Language: Russian (tested), likely reproducible in English as well  
- Internet: Stable Wi-Fi or LTE

---

## Evidence:
- Screenshot: ![IMG_1131](https://github.com/user-attachments/assets/fd493916-bd5c-483c-9ff7-56e2bfb86cac)
![IMG_1132](https://github.com/user-attachments/assets/baf2a3a0-9b7f-46d6-8988-efa59a561a33)
  
- Video file: 

https://github.com/user-attachments/assets/a2e7f880-c7c2-4613-8ad1-cfc369eb8716



---

## Notes:
Even if the icon was not intended to be present in these views, its presence **breaks design consistency**.  
A non-functional UI element confuses users and may cause frustration or unnecessary tapping.  
This should be resolved by either:
- Removing the gear icon from submenus  
- Fixing its position and making it functional if needed

