# Bug Report: VK.com – Music Playback Stuttering and Fragment Loss on Repeat

- **Severity:** High  
- **Platform:** Desktop  
- **Browser:** Google Chrome Version 136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Tested Site:** https://vk.com  
- **Feature:** Music Playback

---

## Description:

When playing music in **VK.com**, specifically from the **Recently Played** section under **My Music**, the audio playback experiences **stuttering, missing fragments, and repeatable audio defects**.

This issue becomes especially noticeable when the **track is set to repeat** — the same stuttering errors repeat in the same spots, suggesting that the **initial audio chunk was corrupted during loading**.

Refreshing the page **does not fix the issue**. Only a full **site reload** (close + reopen browser tab) seems to reset the audio buffer and load a clean version of the track. However, if corruption occurs again, the song will stutter at **different locations**.

---

## Steps to Reproduce:

1. Open Chrome (v136.0.7103.114) and go to https://vk.com  
2. Navigate to **My Music** → **Recently Played**  
3. Select any track and set it to **repeat mode**  
4. Let the song play through and restart  
5. Observe **audio artifacts**: missing segments, digital stutter, glitches  
6. Try refreshing the page — issue persists  
7. Close VK tab completely and reopen → sometimes the track plays fine  
8. Repeat the process — errors may occur again in new locations

---

## Expected Result:

- Music should play smoothly and consistently, especially on repeat.  
- Audio should be **cached or buffered properly**, without corruptions.  
- If there are network issues, player should detect and reload missing chunks.

---

## Actual Result:

- Track plays with **missing audio fragments** and **glitch-like stuttering**  
- Same audio errors occur on every loop (indicates cached corrupted buffer)  
- Refreshing the page **does not resolve issue**  
- Only full tab closure and reloading may bring clean playback

---

## Environment:

- Browser: Google Chrome 136.0.7103.114  
- OS: Windows 10 / 11  
- VK Language: Russian  
- Internet: Stable Wi-Fi / Ethernet  
- Tested on multiple audio tracks in “Recently Played”

---

## Evidence:


---

## Notes:

This appears to be a **buffer corruption or packet loss issue** where the **audio stream is cached in a broken state** and is **not revalidated** or redownloaded upon repeat.

Possible fixes:
- Implement **checksum validation or auto-reload on stream errors**
- Add **buffer flushing mechanism** on repeat to avoid reusing bad cache
- Optionally allow users to **force refresh individual track audio**

---

## User Impact:

- Degraded user experience while
