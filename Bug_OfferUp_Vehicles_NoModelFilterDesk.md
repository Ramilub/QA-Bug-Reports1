# UX Bug Report: OfferUp Vehicles – Missing Model Filter in Vehicle Search

- **Severity:** Medium  
- **Platform:** Desktop Web  
- **Browser:** Google Chrome v136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Tested Site:** https://offerup.com  
- **Module:** Vehicles → Filters

---

## Description:

On the **OfferUp** website, when searching within the **Vehicles** category, the filter section provides options to select:

- **Make (brand)**  
- **Year**  
- **Price**  
- **Mileage**  
- **Fuel type**  
- **Transmission**, etc.

However, there is **no option to filter by specific model** after selecting a car brand.  
This makes it **very difficult to search for a specific car model** within a brand, or to explore the full model range (e.g., all Toyota SUVs or sedans).

---

## Steps to Reproduce:

1. Open https://offerup.com in Chrome (desktop)  
2. Click on the **“Vehicles”** category  
3. Click the **Filters** button  
4. Select any brand (e.g., **Toyota**)  
5. Observe that **no model filter appears**  
6. Try to view all models of the brand → not possible without guessing names in the search bar

---

## Expected Result:

After selecting a car **brand**, the UI should dynamically provide a second filter: **Model**, with options such as:
- Toyota → Camry, Corolla, RAV4, Highlander, etc.
- Ford → F-150, Explorer, Mustang, etc.

This is **standard practice** in most vehicle marketplaces (e.g., Autotrader, CarGurus, Craigslist).

---

## Actual Result:

- There is **no way to filter by model** unless the user types a specific model name manually into the search bar
- There is **no overview of available models** per brand
- Makes **exploratory browsing and comparison** nearly impossible for undecided buyers

---

## Environment:

- Browser: Google Chrome 136.0.7103.114  
- OS: Windows 10 / 11  
- Site: https://offerup.com  
- Tested on both signed-in and guest mode

---

## Notes:

This may not be a technical bug, but it’s a **significant UX oversight** for a marketplace dealing with cars.  
Most users expect to browse by brand → then filter by **model**, **price**, **year**, etc.

Without this feature:
- Users are forced to either **guess and search by name**  
- Or **leave the site** to browse model lists on other platforms

---

## Suggested Solution:

- Add a **dynamic model filter** that appears after a brand is selected  
- Populate it based on VIN/model lists or actual listings  
- Optional: provide a "View all Toyota models" dropdown

---

## User Impact:

- Slower decision-making  
- Frustrating search experience for non-expert buyers  
- Leads to **user churn** toward competitor platforms with better filtering
