TryHackMe OSINT Challenge Write-up

https://tryhackme.com/room/somesint?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=692d67d949c2314779ad896d

Date: Feb, 13,2026

Task 1 was just an overview of the room. It explained the prerequisites like critical thinking, Google skills, and Python/Spiderfoot setup. The flag format is ks{flag}. No solving needed here.

Task 2 introduced the story. I was hired by ks{H} and the target was ks{Thomas Straussman}.

In Task 3, I followed the instructions and only collected passive information from Twitter and Reddit. I searched Thomas Straussman on Google and found his Twitter. Then I searched variations of his username and found his Reddit account.

From his profiles:

Favorite holiday: ks{Christmas}

Birthdate (from Reddit age info): ks{12-20-1990}

Fiancée’s Twitter: ks{@FHodgelink}

Background picture: ks{Buddha}

Task 4 required Spiderfoot. After installing and scanning the given keyword, I checked the source module and found ks{sfp_accounts}. For the shadowban API question, I used the provided link and found the value ks{1346173539712380929}.

Task 5 focused on reverse image searching. I used reverse image tools to analyze vacation photos and other posts.

Answers:

Vacation location: ks{Koblenz, Germany}

Francesca’s mother’s birthday: ks{December 25th}

Cat’s name: ks{Gotank}

Show Francesca watches: ks{90 Day Fiance}

Task 6 used Reddit and Wayback Machine to check older versions of profiles. By reviewing archived captures, I found additional information.

Answers:

Coworker’s name: ks{Hans Minik}

Coworker’s location: ks{Nuuk, Greenland}

Paste ID: ks{ww4ju}

Password: ks{1qaz2wsx}

Mistress’s name: ks{Emilia Moller}

Thomas’ email: ks{straussmanthom@mail.com
}

Overall, I followed the same OSINT process: search, verify, cross-check, and use archived data when needed.
