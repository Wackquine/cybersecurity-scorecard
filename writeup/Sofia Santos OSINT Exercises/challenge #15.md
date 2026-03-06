# TryHackMe OSINT Challenge Write-up

https://gralhix.com/list-of-osint-exercises/osint-exercise-015/

Date: Feb 24,2026

## Step 1: Extract Text from the Document

The challenge provided a screenshot from a CIA declassified document. The caption described a **telescope being assembled at a factory**, but the exact photo and final location were not provided.

To begin, I extracted the visible text from the screenshot and used it as a search query.

Search query used:
telescope built at the askania factory for the university of bonn

This search helped narrow down historical references related to the telescope mentioned in the document.

---

## Step 2: Locate a Matching Photo

While searching the extracted text, I found a historical archive page containing a photo and caption that closely matched the description.

I also foudn this news paper archive:

![](https://github.com/Wackquine/cybersecurity-scorecard/blob/762dab1c357c7786a8f7cd16afb3b5776cd4e15f/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2315%20News%20paper.png)
![](https://github.com/Wackquine/cybersecurity-scorecard/blob/a154280d14812265ffc2d48b04f083e2bb743b38/writeup/Sofia%20Santos%20OSINT%20Exercises/Assets/Exercise%20%2315%20News%20Article.png)

I also foudn this source which further supported and related to the photo:

Source:
https://www.imago-images.com/st/0061895213

The caption stated:

"Jan. 01, 1953 - Gigantic telescope built in Berlin Factory: For the first time since the war a telescope has been built in the Berlin factory of Askania, for the University of Bonn. The telescope is used to study and take pictures of stars..."

The description matched the CIA document's caption mentioning a **telescope assembled at the Askania factory**. The article also referenced the same **year (1953)**, which further confirmed the connection.

The photo from this archive shows the **large telescope being assembled inside the Berlin factory**, matching the description in the declassified report.

Q1. A photo that matches the description on the caption report.  
Answer: The historical photo of the **gigantic telescope assembled at the Askania factory in Berlin for the University of Bonn (1953)**.

---

## Step 3: Determine the Final Location of the Telescope

The caption stated that the telescope was constructed for the **University of Bonn**. This indicated that after being assembled in Berlin, the telescope would eventually be installed at the university's observatory.

By researching astronomical facilities associated with the University of Bonn, I found that the telescope was placed at the **Hoher List Observatory**, which is operated by the university.

The observatory is located in Germany and served as a research site for astronomical observations.

Approximate coordinates of Hoher List Observatory:
50.1623, 6.8506

---

## Final Answers

a) Photo of the **gigantic telescope assembled at the Askania factory in Berlin (1953)** for the University of Bonn.

b) **Hoher List Observatory, Germany**  
Coordinates: **50.1623, 6.8506**

---

## Summary

This challenge involved analyzing historical information and verifying it through open sources. The process included:

- Extracting text from a declassified document
- Searching historical records related to the telescope
- Finding an archive photo that matched the caption description
- Identifying the final installation location of the telescope

By combining keyword searches, historical archives, and institutional information, it was possible to identify both the photo and the telescope’s final location.
