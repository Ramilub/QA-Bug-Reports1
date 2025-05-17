# Bug Report: OfferUp – Vehicle Categories Sometimes Fail to Load Listings

- **Severity:** High  
- **Platform:** Desktop Web  
- **Browser:** Google Chrome v136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Tested Site:** https://offerup.com  
- **Module:** Vehicles → Category Listings (e.g., Commercial Vehicles)

---

## Description:

On the OfferUp website, when accessing the **Vehicles** category and selecting any subcategory (e.g., **Commercial Vehicles**, **Trucks**, etc.), the page **sometimes fails to load any listings**.

- The site layout loads correctly (navigation bar, filters, page frame)  
- However, the actual **item listings do not appear** — only a spinning loading indicator is shown  
- This loading **continues indefinitely** with no timeout or error message

Internet connection is stable, and no issues are observed on other websites at the same time.

---

## Steps to Reproduce:

1. Open [https://offerup.com](https://offerup.com) in Chrome (desktop)  
2. Navigate to the **Vehicles** category  
3. Select a subcategory such as **Commercial Vehicles**  
4. Observe the page:
   - UI frame appears  
   - **No listings are displayed**  
   - A **spinning loader** remains on screen indefinitely  
5. Refresh the page  
6. Listings may appear after refresh — indicating this is an intermittent failure

---

## Expected Result:

When selecting a vehicle subcategory, listings should load within a reasonable time, or an error message should be shown if something goes wrong.

---

## Actual Result:

- The listing section **fails to load**  
- No feedback is provided to the user (e.g., “No items found”, “Network error”, etc.)  
- Only a **spinning loading indicator** is visible indefinitely  
- **Page refresh fixes the issue** in most cases

---

## Environment:

- Browser: Google Chrome 136.0.7103.114  
- OS: Windows 10 / 11  
- Internet: Stable (Wi-Fi and Ethernet tested)  
- Site: https://offerup.com  
- Reproducibility: Intermittent (occurs randomly on any subcategory)

---

## Evidence:

- Video proof: 

https://github.com/user-attachments/assets/0bae1df6-5f82-4a88-8882-d5e776f233f6



---

## Notes:

This appears to be a **server-side or client-server sync issue**, possibly due to:
- Lost packets during API call  
- Unhandled response delay or failure  
- Broken endpoint or cached request

Suggested fixes:
- Add a **fallback message** after X seconds: “Unable to load listings. Please try again.”  
- Implement **automatic retry mechanism**  
- Improve **network error handling** on the frontend

---

## User Impact:

- Users are **blocked from viewing listings**  
- Loss of trust in the platform's stability  
- Encourages users to **abandon site and try competitors**  
- Bad user experience, especially for first-time visitors
