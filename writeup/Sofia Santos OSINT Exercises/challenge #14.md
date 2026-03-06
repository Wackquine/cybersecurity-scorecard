# TryHackMe OSINT Challenge Write-up

https://gralhix.com/list-of-osint-exercises/osint-exercise-014/

Date: Feb 24,2026

## Step 1: Identify the Earthquake

The challenge provided a CCTV video recorded during an earthquake. The first task was to determine the **magnitude of the earthquake**.

I examined the timestamp visible in the CCTV footage and used it as a starting point for my investigation. Using that date, I searched online for earthquakes that occurred around that time.

This search led me to an earthquake record from the Italian National Institute of Geophysics and Volcanology:

https://terremoti.ingv.it/en/event/8206381#:~:text=Earthquake%20with%20magnitude%20of%20Mw,20%20(Italy)%20in%20region%20Romania&text=and%20geographic%20coordinates%20(lat%2C%20lon,Mediterranean%20Seismological%20Centre%20(EMSC).
Mw 5.6 earthquake occured in region: Romania, on

According to the data, an **Mw 5.6 earthquake occurred in Romania on September 23, 2016**.

Details from the earthquake record:
- Date: 23-09-2016  
- Time: 23:11:20 (UTC)  
- Magnitude: Mw 5.6  

Q1. What was the magnitude of this earthquake?  
Answer: **Mw 5.6**

---

## Step 2: Identify the Location in the Video

Next, I needed to determine where the CCTV camera was located.

I performed a **reverse image search using RevEye** and found a YouTube video that matched the footage:

https://www.youtube.com/watch?v=lvGpouFqmJ0

The title of the video contained the phrase **“Cutremur Chisinau”**. Using Google Translate, this translates to **“Chișinău Earthquake”**, which indicated that the video was recorded in **Chișinău, Moldova**.

---

## Step 3: Locate the Exact Area

To narrow down the exact location, I performed another **Google Image search** using frames from the video. 

This search led me to images of the **Atrium Shopping Center** in Chișinău.

Photo: ![](https://github.com/Wackquine/cybersecurity-scorecard/blob/a02a17f3ec8fabcc53350552ca4e2f0d2f474f28/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2314%20Atrium%20Mall.png)

After identifying the shopping mall, I opened **Google Maps and Google Street View** to explore the surrounding streets. I compared the buildings, road layout, and camera angle from the CCTV footage with the map.

Photo: ![](https://github.com/Wackquine/cybersecurity-scorecard/blob/a02a17f3ec8fabcc53350552ca4e2f0d2f474f28/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2314%20CCTV%20ANGLE.png)

By matching the **building shapes, street orientation, and the visible angle of the Atrium Shopping Center**, I was able to identify the likely location where the CCTV camera was placed.

The coordinates of the location are approximately:

**47.01551849513905, 28.854657388507103**

Q2. What are the coordinates of where the camera was likely located?  
Answer: **47.01551849513905, 28.854657388507103**

---

## Final Answers

a) **Mw 5.6 earthquake**  
b) **47.01551849513905, 28.854657388507103**

---

## Summary

This exercise used several OSINT techniques:

- Using timestamps to search for **historical earthquake records**
- **Reverse image searching** with RevEye
- Translating foreign text to identify locations
- Matching landmarks with **Google Maps and Street View**

By combining earthquake databases, reverse image search, and geographic verification, it was possible to determine both the magnitude of the earthquake and the likely camera location.
