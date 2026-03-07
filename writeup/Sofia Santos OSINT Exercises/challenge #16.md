# TryHackMe OSINT Challenge Write-up  
## Disclosing the “Undisclosed Location” of a Military Aircraft

https://gralhix.com/list-of-osint-exercises/osint-exercise-016/

Date: Feb.25,2026

### Task Briefing

On **November 25, 2020**, a Twitter user posted a photograph showing a **military aircraft flying over an undisclosed location**.  
The objective of the challenge was to determine the **exact location where the photograph was taken** using open-source intelligence techniques.

Difficulty level: **Hard** for both beginners and experts.

---

## Step 1 – Reverse Image Search

The first step was to perform a **reverse image search** using **RevEye**.

This search led to the following article:

https://www.centcom.mil/MEDIA/NEWS-ARTICLES/News-Article-View/Article/1280994/oir-official-outlines-gains-pays-tribute-to-fallen-soldiers/

From the article, it became clear that the image was related to **Operation Inherent Resolve**, a U.S.-led military operation against ISIS in Iraq and Syria.

The article also referenced the aircraft and context of the operation, which helped narrow the timeframe and operational region.

---

## Step 2 – Research Operation Inherent Resolve

After identifying the operation, I searched for **Operation Inherent Resolve strike reports** to determine possible operational locations.

This led to the following strike report:

https://www.inherentresolve.mil/Portals/14/Documents/Strike%20Releases/2017/05May/20170531%20Strike%20Release%20-%20Final.pdf

The report listed several locations where coalition airstrikes were conducted on **May 31, 2017**.

Locations mentioned included:

**Syria**
- Near Abu Kamal  
- Near Dayr Az Zawr  
- Near Raqqah  
- Near Tabqah  

**Iraq**
- Near Bayji  
- Near Mosul  
- Near Tal Afar  

These locations became potential reference points for where the aircraft could have been operating.

---

## Step 3 – Plotting Strike Locations

All of the listed strike locations were **pinned on a map** to visualize their geographic distribution.

However, the original caption provided an important clue:

> “An Air Force A-10 Thunderbolt II departs after receiving fuel from a KC-10 Extender during a flight in support of Operation Inherent Resolve May 31, 2017.”  
> *(Staff Sgt. Michael Battles / U.S. Air Force)*

Since the aircraft was **mid-air refueling**, it was likely **not directly over the strike locations**, but instead operating in nearby airspace.

Therefore, the search area needed to expand beyond the specific strike targets.

---

## Step 4 – Finding Related Images

To gather additional clues, I searched for other images taken by the **same photographer on the same date**.

This led to a stock image archive:

https://www.alamy.com/stock-photo-us-air-force-a-10-thunderbolt-ii-ground-support-fighter-aircraft-during-143589519.html

photo:
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/531be5eb17414e204cdfc76fdb8981ceaf4c8e1b/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2316%20Stock%20Photos.png)

By browsing related photos from the same photoshoot, additional environmental details became visible.

Important clues included:

- A **large river or body of water**
- **Rocky mountainous terrain**
- **Sparse urban neighborhoods**
- Similar lighting and geographic features

photo:![](https://github.com/Wackquine/cybersecurity-scorecard/blob/531be5eb17414e204cdfc76fdb8981ceaf4c8e1b/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2316%20Large%20body%20of%20water.png)

These details helped narrow down the possible location.

---

## Step 5 – Geographic Analysis

Using **Google Earth**, I examined the regions surrounding the strike locations identified earlier.

One key observation from the additional images was the presence of a **large river**. Among the potential locations, the **Euphrates River region** matched the geographic characteristics seen in the photos.

By following the river and examining nearby terrain, a location was found that matched the visual clues:

- Similar **river curvature**
- Nearby **rocky mountains**
- Small **settlements close to the water**
- Terrain consistent with the background of the aircraft photo

---

## Step 6 – Confirmation

The suspected area was compared directly with the original photograph.

photo: ![](https://github.com/Wackquine/cybersecurity-scorecard/blob/531be5eb17414e204cdfc76fdb8981ceaf4c8e1b/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2316%20Angle%20of%20the%20Photo.png)
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/0ba5844727b62f7b85ad78e29af62ba071784cc9/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2316.png)
Matching features included:

- The **shape of the river**
- The **position of the surrounding mountains**
- The **layout of nearby neighborhoods**
- Terrain textures and elevation patterns

All these elements aligned with the imagery seen in the original aircraft photograph.

This confirmed that the image was taken over the **Euphrates River region near the strike locations associated with Operation Inherent Resolve**.

---

## Conclusion

The location of the “undisclosed” photograph was identified through a multi-step OSINT investigation:

1. Reverse image searching the aircraft photo
2. Identifying the associated military operation
3. Analyzing official strike reports
4. Mapping strike locations
5. Finding additional photos from the same shoot
6. Using geographic clues to match terrain in Google Earth

By combining **reverse image search, document analysis, and satellite imagery**, it was possible to determine the location where the aircraft photograph was taken.

This challenge demonstrates how publicly available information can reveal details about seemingly undisclosed locations when analyzed carefully using OSINT techniques.
