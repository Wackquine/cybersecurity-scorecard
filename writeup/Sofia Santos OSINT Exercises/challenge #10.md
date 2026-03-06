# TryHackMe OSINT Challenge Write-up

[gralhix.com/list-of-osint-exercises/osint-exercise-010/](https://gralhix.com/list-of-osint-exercises/osint-exercise-010/)

Date: Feb 23,2026

## Step 1: Identify the Event

The challenge provided three photos shared on Twitter and asked what event was being celebrated.  
To begin, I performed a **reverse image search using RevEye** on the images.

One of the search results led to a CNN article:

https://edition.cnn.com/2013/12/05/world/africa/voodoo-dances-mystic-trances

The images in the article matched the style and content of the provided photos. The article describes the **Voodoo Festival celebrated in Benin**, which includes traditional rituals, dances, and cultural ceremonies.

Q1. Which event is being celebrated in the photos?  
Answer: **Voodoo Festival – Benin**

---

## Step 2: Identify Photos Taken by the Same Photographer

Next, I needed to determine which two photos were taken by the same person.

I again used **RevEye reverse image search** and found similar photos on Getty Images:

https://www.gettyimages.com/photos/voodoo-festival-celebrated-in-benin

From the Getty Images page, I discovered that two of the photos were credited to the photographer **Dan Kitwood**.

By comparing the credits and matching images, I confirmed that **two of the provided photos were taken by the same photographer**.

Q2. Which two photos were taken by the same person?  
Answer: **The two images credited to Dan Kitwood**

![](https://github.com/Wackquine/cybersecurity-scorecard/blob/723eec27b7d4dd45083a8d7a41d01b4e4c7b2aad/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2310%20Photographer%20(2).png)
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/723eec27b7d4dd45083a8d7a41d01b4e4c7b2aad/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2310%20Photographer.png)

---

## Step 3: Find the Previous City of the Photographer

The final task was to determine which city the photographer had previously been in before taking those photos.

To investigate further, I searched for the photographer’s name along with relevant keywords. I used the following search query:

Dan Kitwood intext: africa

During this search, I found a post from the photographer’s Twitter account:

https://x.com/dkitwood/status/155572926949765120

From the context of the post and related information, it indicated that the photographer had previously been in **Cotonou**, a major city in Benin.

Q3. The photographer was previously in a different city. What was that city?  
Answer: **Cotonou**

---

## Final Answers

a) **Voodoo Festival – Benin**  
b) **The two photos taken by photographer Dan Kitwood**  
c) **Cotonou**

---

## Summary

This challenge used several OSINT techniques:

- Reverse image searching with **RevEye**
- Identifying **photo credits from media websites**
- Investigating **photographers and their posts**
- Using targeted search queries such as **intext**

By tracing the images and photographer information, it was possible to identify the event, determine which photos were taken by the same person, and track the photographer’s previous location.
