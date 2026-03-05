# TryHackMe OSINT Challenge Write-up

https://gralhix.com/list-of-osint-exercises/osint-exercise-009/

Date: Feb 23, 2026

## Step 1: Analyze the Tweet and Video

The challenge provided a video shared by the **Visit Tirana** Twitter account on **February 16, 2023**.  
From the tweet, several useful clues were visible:

- Location mentioned: **Tirana, Albania**
- Person who recorded the video: **Eriseld Myrto**
- Tweet timestamp (this depends on the viewer's timezone)

Since my system timezone is **Philippines (PHT)**, the tweet appeared as **9:07 AM on February 17, 2023**. Because Albania is several hours behind the Philippines, this means the post was originally made on **February 16, 2023** in Albanian local time.

Photo: 
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/010e212ee4fab5438a8be588391b0b22467afdac/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%239%20Sunset%20Time.png)
---

## Step 2: Estimate the Recording Time

The video clearly shows a **sunset scene**, which suggests the footage was recorded close to sunset.

To verify this, I searched for the **sunset time in Tirana, Albania for February 2023**. The results showed sunset occurring around **17:10 – 17:20 local time** during that period.

Next, I inspected the tweet page source and looked for the exact timestamp associated with the post. In the HTML code, I found the creation time of the post:

**16:48:43 on February 16, 2023 (local time in Albania)**

This time occurs **shortly before sunset**, which matches the lighting and sky color seen in the video. Since the task asks for the best estimate, this timestamp provides the most reliable approximation.

Q1. To the best of your knowledge, at what time was the video recorded?  
Answer: **16:48:43 (February 16, 2023, Tirana local time)**

---

## Step 3: Extract Visual Clues From the Video

Next, I needed to determine the **exact location where the person was walking**.

To do this, I captured a clear frame from the video and performed a **reverse image search using RevEye**. One of the results pointed to a building called **Garden Building Luxury Apartment**.

The structure and colors of the building matched what was visible on the right side of the video.

Additional visual clues helped confirm the location:

- Distinct **street lamps**
- **Pedestrian crossing sign**
- Trees and street layout

Photo: 
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/a6c26f18ff430aca8d71c41eb76601d8b92bca94/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%239%20Maps.png)

---

## Step 4: Confirm the Location Using Maps

After identifying the apartment building, I searched for **Garden Building Luxury Apartment** on Google Maps.

Using **Google Street View**, I compared the environment with the video. Although the Street View images were older, several elements still matched:

- Street layout

These matching details confirmed the filming location.

---

## Step 5: Determine the Coordinates

After locating the exact street on **Google Maps / Google Earth**, I switched to **satellite view** and identified the approximate spot where the person was walking in the video.

The coordinates for this location are approximately:

**41.326, 19.806**

Q2. Find the coordinates of where the person was walking at the time of the recording.  
Answer: **41.326, 19.806**

---

## Final Answers

a) **16:48:43 on February 16, 2023 (Tirana local time)**  
b) **41.326, 19.806**

---

## Summary

This challenge required combining multiple OSINT techniques:

- Understanding **timezone differences**
- Checking **sunset times** for environmental clues
- Inspecting **tweet page source code**
- Using **reverse image search (RevEye)**
- Confirming locations with **Google Maps and Street View**

By correlating visual clues with map data and timestamps, it was possible to estimate both the **time of recording** and the **exact location** of the video.
