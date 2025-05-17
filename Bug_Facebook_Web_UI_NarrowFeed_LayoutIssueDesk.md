# UX Bug Report: Facebook Web – Feed Layout Appears Too Narrow on Desktop, Resembling Mobile Adaptation

- **Severity:** Low to Medium (visual/layout impact)  
- **Platform:** Desktop Web  
- **Browser:** Google Chrome v136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Screen Resolution:** 1920×1080 and higher  
- **Tested URL:** https://www.facebook.com  
- **Language:** Russian (though language-independent issue)

---

## Description:

When accessing the **Facebook web version** on a **standard or wide-screen monitor**, the **main news feed column is significantly narrower** than expected. There is an **excessive amount of whitespace** on both sides of the feed, especially between:

- The central feed (posts/images/stories)  
- The left-side panel (navigation) and right-side panel (contacts, ads)

This layout **resembles a mobile-first responsive design**, but on desktop it feels **cramped and visually inefficient**, especially on large or ultra-wide monitors.

Images and videos appear smaller than they could, and the central content feels compressed.

---

## Steps to Reproduce:

1. Open https://www.facebook.com on a desktop computer  
2. Use a standard or widescreen display (1920×1080 or wider)  
3. Observe the **main feed area** and spacing between columns  
4. Try resizing the browser window — feed remains narrow  
5. Note that even on large displays, images do not scale up appropriately

---

## Expected Result:

On desktop devices with large resolutions, the layout should:
- **Use available screen width more efficiently**  
- Expand the main feed to **better fit modern wide monitors**  
- Display media (images, videos) in a **larger and clearer format**

---

## Actual Result:

- The feed remains **narrow**, wasting available space  
- **Large gaps** appear on both sides of the content  
- Images and posts look **smaller than necessary**, reducing user immersion

---

## Environment:

- Browser: Google Chrome v136.0.7103.114  
- OS: Windows 10 / 11  
- Resolution: 1920×1080, 2560×1440 (tested)  
- Facebook Web: latest layout  
- Account language: Russian  

---

## Evidence:

- Screenshot: ![Снимок экрана 2025-05-17 030952](https://github.com/user-attachments/assets/0fb94252-f4e2-4118-a9ae-97c5b289e81c)


---

## Notes:

This may be **intentional responsive design**, but from a UX perspective:
- It looks like an **incomplete adaptation or mobile-first layout ported to desktop**
- It fails to utilize available horizontal space  
- May affect visual clarity, engagement, and long-form reading

---

## Suggested Improvement:

- Adjust layout dynamically based on screen width  
- Allow the feed to **expand proportionally** on larger monitors  
- Provide a user toggle for **“compact vs. expanded feed view”**

---

## User Impact:

- Feels like a **reduced experience** on desktop  
- May discourage **extended usage** due to constrained visual space  
- Creates the impression that the desktop version is **neglected in favor of mobile**

