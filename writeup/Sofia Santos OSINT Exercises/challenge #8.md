# TryHackMe OSINT Challenge Write-up 

https://gralhix.com/list-of-osint-exercises/osint-exercise-008/

Date: Feb 22,2026

## Step 1: Inspect the Image

The challenge provided a large photo taken from a page of *The Epoch Times*. The goal was to determine what the audience was applauding, the date the photo was taken, and the venue where the event happened.

Looking closely at the image, the audience appeared to be in a theater applauding a performance on stage. However, the newspaper text was written in Chinese, so understanding the context required translating the visible text.

---

## Step 2: Translate and Identify the Event

To understand the content of the page, I used **Google Lens** to scan and translate the Chinese text from the image. During this process, I noticed repeated references to **Shen Yun**.

Searching for *Shen Yun* revealed that it is a well-known **performing arts show that tours internationally**, showcasing Chinese culture and traditional dance. Since the article referenced the performance and the audience was applauding a stage show, it confirmed that the crowd was applauding **Shen Yun Performing Arts**.

Q1. What was the audience applauding?  
Answer: **Shen Yun Performing Arts**

---

## Step 3: Use Reverse Image Search

Next, I performed a **reverse image search** using Google to find other sources containing the same photo. Among the results, I found an article from *The Epoch Times* that contained the exact same image.

Opening the article and scrolling to the photo provided a **caption describing the event**, which included both the **date** and the **location** where the performance took place.

---

## Step 4: Extract the Date

The caption associated with the image indicated the date when the performance occurred. According to the article, the photo was taken during a performance on **January 7, 2023**.

Q2. When was the photo taken?  
Answer: **January 7, 2023**

---

## Step 5: Identify the Venue

The same caption also revealed the name of the theater where the performance occurred. It stated that the performance took place at **Chrysler Hall**, located in **Norfolk, Virginia**.

Q3. What is the name of the venue?  
Answer: **Chrysler Hall**

---

## Final Answers

a) Shen Yun Performing Arts  
b) January 7, 2023  
c) Chrysler Hall  

---

## Summary

This challenge relied on a combination of OSINT techniques:

- Translating foreign-language text using Google Lens  
- Investigating keywords found in the image  
- Performing reverse image searches to locate the original article  
- Extracting information from image captions and sources  

By combining translation tools with reverse image searching, it was possible to identify the event, date, and venue of the photo.
