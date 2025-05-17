# Bug Report: Facebook In-App Browser – App Freezes or Lags After Text Selection Attempt

- **Severity:** High (intermittent, with partial recovery)  
- **Platform:** iOS 18.3.2  
- **App Version:** Facebook 513.0.0  
- **Device:** iPhone SE / iPhone (iOS-compatible)  
- **Module:** In-App Browser (opened from News Feed)

---

## Description:

In the **Facebook mobile app**, when opening external articles via the **in-app browser**, attempting to **select text** often causes the interface to **freeze or severely lag**.

- The app may become **temporarily unresponsive**: no scrolling, no gestures
- In some cases, the app **remains frozen until the user closes the in-app browser**
- However, **occasionally the app unfreezes by itself after a few seconds**, and normal scrolling becomes available again

This creates a **disruptive and unpredictable experience**, especially when users try to copy or highlight information.

---

## Steps to Reproduce:

1. Open the Facebook app (v513.0.0) on iOS 18.3.2  
2. Scroll through the News Feed  
3. Tap a post with a link to an external website (news article)  
4. Allow it to open in the in-app browser  
5. Long-tap on any paragraph to **try selecting text**  
6. Observe the behavior:
   - In many cases, **the screen becomes frozen**
   - Touch gestures stop responding (cannot scroll or cancel selection)
   - Sometimes, after ~3–7 seconds, **the app recovers and becomes responsive again**

---

## Expected Result:

- User should be able to **select and copy text smoothly**
- App should **remain responsive** at all times
- If selection fails, it should be **cancelable without freezing the UI**

---

## Actual Result:

- Text selection causes **partial or full UI freeze**
- Scroll and gestures become **non-functional** temporarily or until closed
- In some cases, the app **recovers on its own after a few seconds**, but in others only force-closing the in-app browser helps

---

## Environment:

- iPhone SE / iPhone 12 / iPhone 14  
- iOS: 18.3.2  
- Facebook Version: 513.0.0  
- App Language: Russian  
- Network: Stable Wi-Fi / 5G

---

## Evidence:

-

https://github.com/user-attachments/assets/2e09aea4-5182-4573-bc36-f13026fc8338


