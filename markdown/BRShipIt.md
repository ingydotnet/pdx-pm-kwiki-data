## Ship It!

_review by_ [[EricWilhelm]]

**Authors:** Jared Richardson, William A. Gwaltney

**Publisher:**  Pragmatic Bookshelf

**ISBN:** 0-9745140-4-7

200 pp, $29.95 US, $41.95 CA, �20.95 UK

**Intended audience:**

Everyone from programmers to project managers.  Even if you are not in a position to make decisions, you might only be reading it to confirm
that sinking feeling that you are on a sinking ship.  Technical leads will probably benefit most from this book.  If you are a manager and you
do not have a technical lead, you must read this book!

### What I liked:

* _Lots_ of good, pragmatic advice.
* Links to recommended software, often open-source.
* "How to do it" and "Is it working?" sidebars provide condensed information specifically designed to help you put these ideas into practice.
* Very logical, usable layout.
* The suggested practices are not presented as "the one true way", just "what worked for us."  Lots of room is left for the reader to fill-in their own details, but the authors still present enough details, anecdotes, and scenarios to avoid talking in generalities.

### What needed some help:

* Typos!  Usually these don't bother me so much, but at one point two typos appear on facing pages.  Luckily, the entire book does not contain that density of errors, but when they appear so close together, it stands out as very annoying.
* Misattributed quotes by the recently deceased.  A quote by Douglas Adams gets attributed to Scott Adams and put under the header "Dilbert on Deadlines."  Please check your sources.
* Claiming that sloppy Java is "pseudocode" is not allowed!  If you are going to write pseudocode (which is a bad idea anyway), it should be plain English indented to form blocks.  Maybe valid Java would have been too long?  (Hint: next time, try Perl.)  Luckily, there are only a few instances of pseudoJava.
* Some parts are unnecessarily slanted toward Java development.  The introduction claims that the book is language independent, and it mostly holds to this, but tends to revert to a discussion of Java development on occasion.

**Bottom line:**
Very readable and pragmatic advice.  If you are managing, leading, or working on software, and are not already doing all of these things, you should definitely read this book.

---

### Chapter-by-chapter:

**Ch1** Introduction

An overview of the authors' backgrounds, experiences, and their approach to software development.  This is followed by a quick roadmap of the book and then the ever-present "How to Read (This Book)" section.

**Ch2** Tools and Infrastructure

This goes over the tools you should be using and how to get started using them without bringing your project to a complete halt.  The tools appear again in a more concise form in appendices B,C,D,E, and G, but this chapter gives reasons for using each tool and you may recognize your own situation in some of their scenarios about what happens if you do not have each piece of infrastructure in place.

**Ch3** Pragmatic Project Techniques

"The List", technical leads, strategies for communication and meetings,
code reviews, etc.

**Ch4** Tracer Bullet Development

Presents a methodology for developing a project in which you have "running code" from start to finish.  Unfortunately, no mention is made of Brooks, who laid-out this same methodology under a different name long ago.

**Ch5** Common Problems and How to Fix Them

This chapter enumerates and addresses 18 problems ranging from unhappy customers to "Death March" projects.  Mostly, it points out symptoms which manifest when the principles covered in the book have not been used and recommends a "way out" of each given situation.

**Appendices**  A-H

Lots of information here.  Most notably, the list of tools and URL's (which really should be in clickable form somewhere.)  The book has a lot more links, but since I am doing the typing and most of theirs are fairly Java-specific, I will cherry-pick and add a few of my own here.

* Source Code Management:
  * http://subversion.tigris.org/
* Build Scripting Tools:
  * http://search.cpan.org/search?module=Module::Build
* Continuous Integration Systems:
  * http://damagecontrol.codehaus.org/
* Issue Tracking:
  * http://www.bestpractical.com/rt/
* Testing Frameworks:
  * http://search.cpan.org/search?module=Test::More
