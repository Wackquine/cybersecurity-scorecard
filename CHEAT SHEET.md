OSINT Cheat Sheet (Updated)

1) Start With What You’re Given
If image:
- Check metadata (exiftool)
- Reverse image search (Google, Yandex)
- Look at background details (buildings, signs, landmarks, shadows, skyline)

If name or username:
- Google it directly
- Search fullname + reddit
- Search fullname + twitter
- Try username variations

2) Reverse Image Search (IMINT)
Tools:
- Google Images
- Yandex
- TinEye

Focus on:
- Landmarks
- Unique buildings
- Street layouts
- Vacation spots
- Architecture

Confirm using:
- Google Maps
- Street View
- Photos tab comparison
- Building height checks

3) Social Media Investigation
Check:
- Twitter/X
- Reddit
- Bio
- Profile photo
- Banner image
- Tagged people
- Replies and comments

Look for:
- Birthday clues
- Location hints
- Holiday posts
- Pets
- Relationships
- Travel history

Rule: Stay passive. No interaction.

4) GitHub & Code Review
- Check bio (city, email)
- Inspect repositories
- Read README
- Review commit history (especially deleted commits)
- Look for exposed emails, keys, wallet addresses
- Decode PGP keys if present

5) WiFi / BSSID Investigation
If BSSID found:
- Use Wigle.net
- Advanced search
- Retrieve SSID and possible location

6) Spiderfoot / Automation
- Run scan on username
- Check source modules (ex: sfp_accounts)
- Review discovered linked accounts

7) API & Hidden Data
- Inspect API endpoints (example: shadowban API)
- View page source
- Check JSON responses
- Look for IDs and hidden values

8) Wayback Machine Method
- Use old.reddit.com if needed
- Open Wayback Machine
- Check older captures
- Compare versions
- Look for deleted links and paste IDs

9) Common Data to Extract
- Full name
- Email
- Username variations
- Birthdate
- Location
- Coordinates
- WiFi SSID / BSSID
- Paste ID
- Passwords in screenshots
- Building names
- Height of buildings

OSINT Workflow
Observe
Extract
Search
Verify
Cross-check
Confirm
Document

Core Principle
No hacking.
No interaction.
Only public data.
Connect small clues logically.
Think structured.

# 🌐 Web Crawlers, SEO & Sitemap Cheat Sheet (CTF + Security Focus)

------------------------------------------------------------------------

# 1️⃣ How Web Crawlers Work

## Discovery Methods

1.  Direct discovery
    -   Crawler visits a domain directly\
    -   Indexes content type, keywords, metadata
2.  Link traversal (Recursive crawling)
    -   Follows all URLs found on the site\
    -   Crawls internal + external links\
    -   Expands like a graph/tree

Think of it as: Domain → Extract links → Visit links → Repeat

------------------------------------------------------------------------

# 2️⃣ What Crawlers Store

For each domain, crawlers collect:

-   Keywords
-   Page titles
-   Metadata
-   Links (internal & external)
-   Content structure
-   File paths
-   Sitemap references

Example:

Domain: mywebsite.com\
Keywords: Apple, Banana, Pear

Domain: anotherwebsite.com\
Keywords: Tomatoes, Strawberries, Pineapples

Search engine builds a keyword → domain dictionary.

------------------------------------------------------------------------

# 3️⃣ How Search Engines Answer Queries

When user searches:

Example: "Pears"

Search engine checks index: - Which domain contains "Pears"? - Returns
ranked result

If multiple domains contain same keyword: → Ranking algorithm decides
order.

------------------------------------------------------------------------

# 4️⃣ Ranking & SEO (Search Engine Optimisation)

Search engines score websites based on:

✔ Website responsiveness (desktop + mobile) ✔ Browser compatibility ✔
Page load speed ✔ Clean structure ✔ Crawlability ✔ Presence of sitemap ✔
Keyword relevance ✔ Internal linking structure

Important: Search engines use complex algorithms. Exact scoring methods
are private.

You can pay to boost ranking (ads).

------------------------------------------------------------------------

# 5️⃣ robots.txt Cheat Sheet

Location: example.com/robots.txt

Purpose: Controls crawler access.

Syntax:

User-agent: \* Allow: /public/ Disallow: /admin/ Sitemap:
https://example.com/sitemap.xml

Directives:

User-agent → Which crawler \* → All crawlers Allow → What can be indexed
Disallow → What cannot be indexed Sitemap → Where sitemap is located

⚠ Security Note: robots.txt does NOT protect content. It only requests
crawlers to avoid indexing. Attackers can still manually access
disallowed paths.

Common CTF trick: Check robots.txt for hidden directories.

------------------------------------------------------------------------

# 6️⃣ Sitemaps Cheat Sheet

Location: example.com/sitemap.xml

Format: XML

Purpose: Provide structured map of all URLs.

Benefits: ✔ Easier crawling ✔ Faster indexing ✔ Better SEO ranking

Sitemaps list: - URLs - Last modified date - Priority - Change frequency

Security Note: Sitemaps may reveal: - Hidden pages - Admin portals - Old
endpoints - Staging environments

Always check sitemap during recon.

------------------------------------------------------------------------

# 7️⃣ Website Structure Model

Example hierarchy:

Blue nodes → Directory paths Green nodes → Actual pages

Crawlers traverse this tree fully.

------------------------------------------------------------------------

# 8️⃣ Security & Recon Perspective

When performing recon:

1.  Check robots.txt
2.  Check sitemap.xml
3.  View page source
4.  Enumerate internal links
5.  Follow external links
6.  Identify indexed vs non-indexed pages

Useful commands:

curl https://example.com/robots.txt curl https://example.com/sitemap.xml

------------------------------------------------------------------------

# 9️⃣ Key Takeaways

✔ Crawlers index everything they can find ✔ External links expand
crawler reach ✔ SEO influences ranking order ✔ robots.txt controls
indexing (not access) ✔ Sitemaps improve crawl efficiency ✔ Easier to
crawl = better SEO score

------------------------------------------------------------------------

# 🧠 CTF Mental Model

Crawler = Automated Recon Bot

If you understand: - How it discovers content - How it stores keywords -
How it ranks results - How access can be restricted

You can: - Find hidden directories - Discover forgotten endpoints -
Identify misconfigured robots.txt - Exploit exposed sitemap entries

------------------------------------------------------------------------

| Term      | Action                                                                 |
|-----------|------------------------------------------------------------------------|
| filetype: | Search for a file by its extension (e.g., PDF)                        |
| cache:    | View Google's cached version of a specified URL                       |
| intitle:  | The specified phrase MUST appear in the title of the page             |

