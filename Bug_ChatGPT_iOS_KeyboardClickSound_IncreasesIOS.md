# Bug Report: ChatGPT iOS App – Keyboard Click Sound Increases After Initial Input

- **Severity:** Medium (Privacy/UX Impact)  
- **Platform:** iOS 18.3.2  
- **App Version:** ChatGPT 1.2025.147  
- **Device:** iPhone SE / iPhone 12 / iPhone 14 (iOS-compatible)  
- **Language:** Russian / English (irrelevant)  
- **Module:** Keyboard input

---

## Description:

In the **ChatGPT mobile app** for iOS, when entering a prompt using the **default Apple keyboard**, the **clicking sound (keyboard feedback)** significantly increases in volume after the **second prompt input**.

- First prompt → Normal click sound  
- Second prompt and beyond → Click sound becomes **noticeably louder**, almost as if **speakerphone mode** is enabled  
- The issue **does not resolve consistently** until switching apps or muting the phone

This behavior is unexpected and **intrusive in quiet environments**, causing discomfort, especially for **introverted or privacy-conscious users**.

---

## Steps to Reproduce:

1. Open ChatGPT iOS app (v1.2025.147)  
2. Enter a prompt using the default iOS keyboard  
3. Notice normal clicking sound on first prompt  
4. Submit and wait for response  
5. Enter a **second prompt**  
6. Notice that **keyboard click sounds increase in volume noticeably**  
7. Switch apps and return → Sometimes issue disappears  
8. In many cases, **only silent mode resolves the issue**

---

## Expected Result:

- Keyboard click sounds should remain **consistent and system-controlled**  
- No unexpected increase in volume  
- App should **not override iOS keyboard audio behavior**

---

## Actual Result:

- Click sounds **amplify unexpectedly** after first message  
- Sounds are **louder than in any other app**  
- **Surrounding people can hear** the user typing  
- Breaks **user's sense of private interaction**

---

## Environment:

- Device: iPhone SE / iPhone 14  
- iOS: 18.3.2  
- App Version: 1.2025.147  
- Keyboard: Default iOS Keyboard  
- Reproducibility: Frequent  
- Network: Irrelevant (offline/online both affected)

---

## Notes:

- May be related to **audio focus handling or audio session configuration** inside the app  
- Possibly caused by improper interaction with iOS `AVAudioSession` settings, which can redirect audio routing unexpectedly  
- Could be an unintended **side-effect of audio hooks** used to play generated speech, affecting keyboard sound routing

---

## Suggested Fix:

- Audit app’s **audio session management** to ensure it does **not override keyboard feedback volume**  
- Test keyboard behavior after multiple inputs in various app states  
- Ensure fallback to **system-level volume and routing** for all input feedback

---

## User Impact:

- Discomfort and anxiety for **introverted or privacy-conscious users**  
- Decreased trust in app’s privacy handling  
- Perception of the app **eavesdropping or exposing user actions**  
- Potential drop in daily usage due to fear of being overheard

---

## Evidence:

- video 

https://github.com/user-attachments/assets/b20ab877-8c7d-45e2-b446-3be12ac340b3


