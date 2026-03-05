# TryHackMe OSINT Challenge Write-up

https://gralhix.com/list-of-osint-exercises/osint-exercise-007/

Date: Feb 22,2026

## Step 1: Start With Reverse Image Search

The challenge provided an image and asked for the location where the photo was taken. Since there was no additional information, the first step was to perform a reverse image search.

I used Google Reverse Image Search to find visually similar images and related sources. The results pointed to a location called **Centro Vasco da Gama**, which is a shopping center located in Lisbon, Portugal. One of the matching results appeared on Foursquare and confirmed that the image matched this location.

At this point, the name of the location was identified.

---

## Step 2: Confirm the Exact Location

Although the location name was found, OSINT challenges usually require precise coordinates. To verify this, I opened **Google Maps** and switched to **satellite view**.

By comparing the layout in the challenge image with the satellite map and interior views, I noticed that the photo appeared to be taken from an upper level. The escalator blocking part of the view suggested that the camera was positioned on the **second floor of the mall**.

After examining the map closely, the approximate coordinates of the location were identified.

Q1. What is the location in the image?  
Answer: Centro Vasco da Gama, Lisbon, Portugal  

Coordinates: **38.76, -9.09**

---

## Step 3: Identify the Year the Photo Was Taken

Next, the challenge asked for the year when the image was taken.

Looking closely at the image, there was a large event poster visible in the upper-right section. The poster contained the word **“Tutankamon”**, which appeared to reference an exhibition or event.

I searched Google for **Tutankamon Lisbon event**, but the results were limited in English. To get better results, I switched my search language to **Portuguese** and searched again.

This led to a Facebook post displaying the same poster seen in the image.

The poster showed the event date **April 19, 2019**, which strongly indicated the timeframe of the photo.

Q2. What year was the photo taken?  
Answer: **2019**

---

## Step 4: Identify the Website From the Poster

The final question required identifying the website displayed on the poster.

After examining the bottom part of the poster in the image, a website URL was visible.

The link displayed was:

**www.tutankamon.pt**

Even though the website is no longer active, it matches the URL shown on the poster.

Q3. What website is shown on the poster?  
Answer: **www.tutankamon.pt**

---

## Final Answers

a) Centro Vasco da Gama, Lisbon, Portugal (38.76, -9.09)  
b) 2019  
c) www.tutankamon.pt  

---

## Summary

This challenge demonstrated several key OSINT techniques:

- Reverse image searching to identify locations
- Verifying locations using satellite maps
- Extracting clues from posters and visible text
- Searching in local languages for better results
- Confirming details through public sources

The investigation relied entirely on open-source information and careful observation of small details within the image.
