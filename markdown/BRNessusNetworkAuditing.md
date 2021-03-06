## Nessus Network Auditing

Deraison, R. et al; Beale, J. ed.

**Publisher:**  Syngress

**ISBN:** 1-931836-08-06.

508 pp, $49.94 USA, $69.95 CAN.

Official Blurb from O'Reilly:
"Nessus is the premier Open Source vulnerability assessment tool, and
was recently voted the "most popular" open source  security tool of any
kind. This is the first book available on Nessus and it is written by
the world's premier Nessus  developers led by the creator of Nessus,
Renaud Deraison.".

**Intended audience:** This book would be great for people who've never used nessus, but have some network & sysadmin  experience.  This book was of particular interest to me, because I need to learn nessus quick-like.  A little more than half the book is useful without having the app in front of you.  You will want to have a nessus server & something to test scan to follow along with the chapters on installation, scanning, results interpretation, and writing your own plug-ins.  This book is better as a how-to guide than a reference.

### What I liked:

* The layout is easy to follow & you know what's going to come next, which increases the books readability.
* _Lots_ of good generic security info, especially in the sidebars.  For a security newbie, the book is worth reading for  that info even if you're not interested in using nessus.
* When there's more than one way to do something, the advantages & disadvantages of both are clearly discussed.
* Very clear writing style.
* Each chapter has a "summary"; a "solutions fasttrack", a bulleted list of the material covered in the chapter; and a FAQ.

### What needed some help:

* Typos & grammatical errors.  Yes, I realize some of them are unavoidable, but it seems there is a rush to publish technical material because it's so quickly out-of-date, and quality is sacrificed in that rush.
* Key words could have been bolded or italicized on their first introduction to make it easier to find stuff later.
* I would have liked to see equivalent attention to the cli as to the GUI, but that may have been beyond the scope of the book.
* The index.  One of my pet peeves is crappy indexes.  I decided to test the index by looking up  "database", because about half a chapter was devoted to saving scan results in a database, and that chapter was not listed in the index.  Stee-rike one.

**Bottom line:**
**Worth the price. I bought my own copy today.**

---

### Chapter-by-chapter notes:

**Ch1** Vulnerability assessment

Good overview of what a vulnerability assessment is & tools used to find them.

**Ch2** Introducing Nessus

Useful advice on how to choose a security consultant (required reading for PHBs.)
Not-too-long paragraph on the history of nessus, but I'm not sure what's useful about the graph of the growth of the nessus user community.

**Ch3** Installing Nessus

Asserts that nessus is "one of the easiest packages to install".
Because I will not be installing nessus myself, I independently verified this with a poll.  All responders (n=2) disagreed.
Great advice about choosing a server - they actually have hard numbers for the specs. =:O
The lists of mirrors could probably have been replaced with the URL for the main nessus site (why make the book unneccessarily fatter?)

I quit tracking typos/grammatical errors in this chapter.
Great reasons to install from source & super-detailed install
instructions.

**Ch4** Running your first scan

VERY good advice about getting written permission from Those in
Positions of Authority before running **any** scan. Good ammo to use with PHBs about why you should run vuln testing.

Info about how to use the GUI; don't be tempted to skip this because there is some good security advice buried in this section.

Concise explanation of ip subnetting.  Useful plan outline for routine scans.

**Ch5** Interpreting results

Navigating the GUI, how to figure out what you're looking at, some gotchas.

**Ch6** Vulnerability types

Maybe this would have been better after Ch 1, it kind of interrupts the flow here.  It seems that  "False Positives" (Ch7) would better follow "Interpreting Results" (Ch5).

**CH7** False Positives

Lots of examples.   Offers ways to deal with false positives, as the sheer number of them can be enough to put one off vuln testing entirely.

**Ch8**  Under the hood

Good overview of how nessus works.  Didn't need to have the app in front of me to learn anything from this chapter.

**Ch9** Knowledge Base

Seems like a good overview, would need to follow along at home to really test this one out.

**Ch10** Enterprise Scanning  (this was the most useful chapter in the book)

Good info about where to start if you have no idea:  what to scan first, how to report it, bandwidth considerations, etc.  Good advice about who to warn & how to approach them.

Excellent guidelines for approaching a scan in a scientific manner: trying nessus out in a lab environment first, testing to make sure nessus is picking up vulnerabilities you know exist, etc.  How to set up a distributed scanning environment.
Recommendations about storing scan results in a database (ooh, that is exciting).  AND, a list of common problems you might encounter!  Grand!

**Ch11** NASL

Introduction to the NASL scripting language.  This is hard going without hands-on following along.

**Ch12**  The nessus user community

Where to go to get help.  More detail than was useful to me.
