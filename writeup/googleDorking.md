TryHackMe OSINT Challenge Write-up
https://tryhackme.com/room/googledorking?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=692d67d949c2314779ad896d
Date: Feb 22,2026

# Web Crawlers, SEO, Robots.txt, Sitemaps & Advanced Searching – Write-Up

---

## 1. What Are Crawlers and How Do They Work?

Web crawlers (also known as spiders or bots) are automated programs used by search engines such as Google and Bing to discover and index content across the internet.

### How Crawlers Discover Content

Crawlers find content in two main ways:

#### 1️⃣ Direct Discovery  
A crawler visits a URL directly:
- Retrieves website content  
- Extracts keywords  
- Collects metadata  
- Identifies file types  
- Extracts links  

#### 2️⃣ Link Traversal (Crawling)  
After indexing a website, the crawler follows all hyperlinks found on that site.  
This process repeats, allowing the crawler to map large portions of the web.

---

## 2. What Is Indexing?

The key term for what a crawler builds is:

**Index**

An index is a structured collection of resources and their locations.

When a crawler visits a website:
- It extracts keywords  
- Stores them in a database (index)  
- Associates those keywords with the domain  

Example:

| Domain | Keywords Indexed |
|---------|------------------|
| mywebsite.com | Apple, Banana, Pear |
| anotherwebsite.com | Tomatoes, Strawberries, Pineapples |

If a user searches for "Pears", the search engine checks its index and returns `mywebsite.com`.

---

## 3. How Search Engines Retrieve Information

**Technique used:** Indexing

Search engines retrieve information from their stored index rather than scanning the entire web live during each search.

This allows:
- Fast search results  
- Keyword matching  
- Ranking calculations  

---

## 4. Example of Content Gathered by Crawlers

Crawlers can gather:

- Keywords  
- Page titles  
- Metadata  
- File types  
- Internal and external links  
- Images  
- PDFs  
- Structured data  

---

## 5. Search Engine Optimisation (SEO)

SEO improves how easily a crawler can:
- Access  
- Understand  
- Index  
- Rank  

### Ranking Factors Include:
- Mobile responsiveness  
- Page load speed  
- Keyword usage  
- Sitemap availability  
- Crawl permissions  
- Internal linking structure  

Search engines use complex algorithms to determine ranking order.

---

## 6. Robots.txt

The `robots.txt` file controls crawler access.

### Location

For the domain:


ablog.com


The robots file would be located at:


ablog.com/robots.txt


---

### Basic Robots.txt Structure


User-agent: *
Allow: /
Sitemap: http://mywebsite.com/sitemap.xml


### Keywords Explained

| Keyword | Purpose |
|----------|----------|
| User-agent | Specifies which crawler |
| Allow | Permits indexing |
| Disallow | Blocks indexing |
| Sitemap | Points to sitemap file |

---

### Allow Only Bingbot


User-agent: Bingbot
Allow: /

User-agent: *
Disallow: /


---

### Prevent Crawling of a Directory

To block:


/dont-index-me/


Use:


Disallow: /dont-index-me/


---

### Unix/Linux Configuration File Extension

A common sensitive configuration file extension:


.conf


Other sensitive file types:
- `.ini`
- `.env`
- `.log`
- `.sql`
- `.bak`

---

## 7. Sitemaps

A sitemap is a structured map of website URLs.

### Typical File Structure


XML


Sitemaps are typically located at:


domain.com/sitemap.xml


---

### Real-Life Comparison

A sitemap can be compared to:

**A geographical map**

It shows structured paths and locations within a website.

---

### Keyword for the Path Taken for Content

**Route**

---

## 8. Advanced Google Searching (Google Dorking)

Search engines allow operators to refine queries.

---

### Query BBC About Flood Defences


site:bbc.co.uk "flood defences"


---

### Search by File Type

Operator:


filetype:


Example:


site:bbc.co.uk filetype:pdf


---

### Search for Login Pages

Operator:


intitle:


Example:


intitle:"login"


---

# Final Answers Summary

## Crawlers Section
- Key term: Index  
- Technique used: Indexing  
- Example content gathered: Keywords, metadata, PDFs  

---

## Robots.txt Section
- Location: ablog.com/robots.txt  
- Sitemap location: domain.com/sitemap.xml  
- Allow only Bingbot:

User-agent: Bingbot
Allow: /

- Prevent indexing directory:

Disallow: /dont-index-me/

- Unix config extension: .conf  

---

## Sitemaps Section
- Typical structure: XML  
- Real-life comparison: Map  
- Keyword for path: Route  

---

## Advanced Searching
- Query format:

site:bbc.co.uk "flood defences"

- Search by file type term: filetype:  
- Search for login pages term: intitle:  

---

## Conclusion

This challenge demonstrates:

- How web crawlers discover and index content  
- How search engines rank results  
- How robots.txt controls crawler access  
- How sitemaps improve optimisation  
- How advanced search operators refine queries  

These concepts are foundational for:
- OSINT investigations  
- Web security analysis  
- SEO optimisation  
- Ethical reconnaissance  
