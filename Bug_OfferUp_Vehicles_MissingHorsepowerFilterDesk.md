# UX Bug Report: OfferUp Vehicles – No Filter for Engine Horsepower

- **Severity:** Medium  
- **Platform:** Desktop Web  
- **Browser:** Google Chrome v136.0.7103.114 (64-bit)  
- **OS:** Windows 10 / 11  
- **Tested Site:** https://offerup.com  
- **Module:** Vehicles → Filters

---

## Description:

On the **OfferUp** platform, when browsing vehicles through the desktop site, users are presented with several filters, including:

- **Make (brand)**  
- **Year**  
- **Mileage**  
- **Transmission**  
- **Fuel type**  
- **Price**

However, there is **no filter for engine power (horsepower)** — a critical metric when selecting a vehicle.

Many cars come in different configurations and trim levels that only differ by **engine power**, especially for sport vs. economy variants. Without this filter, users are **unable to narrow down vehicles** by one of the most fundamental performance criteria.

---

## Steps to Reproduce:

1. Go to [https://offerup.com](https://offerup.com) in Google Chrome  
2. Select the **Vehicles** category  
3. Open the **Filters** menu  
4. Observe that there is **no filter for horsepower or engine output**

---

## Expected Result:

Users should be able to:
- Select a **range of horsepower values** (e.g., 100–200 HP, 200–300 HP, etc.)
- Filter vehicles that match performance expectations:  
  - Commuter cars  
  - Family cars  
  - Sport/performance cars  
- Combine this filter with others (make/model/year) to **refine search**

---

## Actual Result:

- Users **cannot search by engine horsepower**
- No performance-based filtering is available
- Power-related criteria must be **guessed manually** through external research

---

## Environment:

- Browser: Google Chrome 136.0.7103.114  
- OS: Windows 10 / 11  
- Site: https://offerup.com  
- Logged-in and guest modes tested

---

## Notes:

This is a **functional gap** that limits OfferUp as a car search platform.  
Horsepower is one of the **most referenced vehicle specifications**, commonly found in:

- Manufacturer specs  
- Car review sites  
- Competing marketplaces (e.g., Autotrader, Cars.com, CarGurus)

---

## Suggested Improvement:

- Add a **horsepower filter**, ideally with:
  - **Slider** (min–max HP)
  - Or **range presets** (e.g., under 150 HP / 150–250 / 250+)
- Fetch HP data from VIN decoding or listing description metadata

---

## User Impact:

- Loss of ability to filter vehicles by **performance profile**
- Increased effort for users who want to compare different variants of the same model
- Encourages users to **leave OfferUp** and search elsewhere for advanced filtering
