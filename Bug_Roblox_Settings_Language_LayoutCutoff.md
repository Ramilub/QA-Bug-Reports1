# Bug Report: Roblox Web – "Language" Field in Settings Slightly Cut Off at Bottom

- **Severity:** Low (Visual/UI)  
- **Platform:** Desktop Web  
- **Browser:** Google Chrome v136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Resolution:** 1920x1080  
- **Tested URL:** https://www.roblox.com/my/account#!/info?nl=true
- **Module:** Account Settings → Language selection

---

## Description:

On the **Roblox website**, when accessing the **Account Settings** page, the **"Language" field appears slightly cut off** at the bottom. This includes:

- The **label “Language”**  
- The **language dropdown menu** itself

This occurs **only if the "Account Location" field is not visible** (e.g., not filled or not shown for the user). The layout shifts, resulting in the **bottom portion of the language section being clipped** or cropped.

---

## Steps to Reproduce:

1. Log in to [https://www.roblox.com](https://www.roblox.com)  
2. Go to **Settings** (https://www.roblox.com/my/account#!/info?nl=true)
3. Scroll to the **bottom** of the settings page  
4. If "Account Location" is not shown, observe the **Language** section  
5. Notice the label and dropdown menu are **cut off from below**

---

## Expected Result:

- The **Language** field and dropdown should be **fully visible**  
- Proper padding or spacing should be applied regardless of other fields' presence

---

## Actual Result:

- The **bottom of the Language section is clipped**, causing the UI to look unprofessional  
- Dropdown list appears truncated  
- Field label may look like it's “floating” without margin

---

## Environment:

- Browser: Google Chrome v136.0.7103.114  
- OS: Windows 10 / 11  
- Device: Desktop  
- Resolution: 1920x1080  
- Roblox Account Type: Child/Teen (no location field)

---

## Evidence:

- Screenshot: ![Снимок экрана 2025-05-26 233535](https://github.com/user-attachments/assets/16ea9754-d186-4429-bf10-59f11a69ce50)
![Снимок экрана 2025-05-26 233559](https://github.com/user-attachments/assets/d0cbc3bb-ad42-4668-a683-e74d6d776b28)
 
- Zoom level: 100%  
- No custom styles or browser extensions applied

---

## Notes:

This is a **basic CSS spacing or container height issue**, possibly tied to the conditional rendering of the “Account Location” field.  
Fix likely involves adjusting the **parent container's padding/margin bottom** or forcing a **minimum height** regardless of field presence.

---

## User Impact:

- May cause **confusion and distrust**, especially among **parents of child users**  
- Makes the settings page look **unfinished or low-quality**  
- Could raise concern: "Am I on the real Roblox site?" — affecting **trust during financial transactions or parental monitoring**

---

## Suggested Fix:

- Apply minimum bottom padding to the container even if "Account Location" is hidden  
- Ensure "Language" section has consistent spacing regardless of field visibility  
- Test across various account types (child/teen/adult)

