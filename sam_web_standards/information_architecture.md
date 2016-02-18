---
title: SAM Web Standards | Information Architecture
layout: sam_web_standards
---

# Information Architecture

Information Architecture, in terms of navigation, refers to the layout and depth of pages within a website. There are two primary ways for a front-end user to find information. The first is through links from one page to another. The second is by searching for content and following links within those results. 

When a front-end user is looking for high-level or general information, the front-end user should be able to navigate the site quickly via static menus. The front-end user may not know exactly where to go or what (s)he is looking for; the architecture can help guide the front-end user by starting broad (categories) and becoming more detailed (a specific notice, wage determination, program, and so on).

When a front-end user knows the information (s)he is looking for, search becomes the better option; therefore, front-end users should be allowed to search using text with additional filtering capabilities within a given category.

## Navigation

The *SAM Web Standards* recognize three levels of navigation for page-related content.

1. **Main Navigation:** Contained within the header and footer components and used to navigate between system-wide pages (the Legal page, for example) and between categories within the system (Wages, for example). From a front-end user perspective, this results in a change from transition.SAM.gov to something like transition.SAM.gov/wages.
2. **Category Navigation:** Appended to the header area and provides navigation within a category; thereby, allowing each category to have primary pages (“Due to Be Revised” within Wages, for example). Resulting in something like transition.SAM.gov/wages/to-be-revised.
3. **Sidebar Navigation (up to three levels):** Navigation appearing in a vertical sidebar along the left side of pages (see the [US Web Design Standards](https://playbook.cio.gov/designstandards/sidenav/)). This type of navigation should be avoided, if possible or practical. Further, if possible, only one level of navigation will make it easier to navigate both the site and categories.

## Content

Information Architecture, in terms of content, refers to how content is displayed. This could be the ordering of information within a block of content (chapters within a book, paragraphs within a chapter, sentences within a paragraph, and so on) or how blocks of content are arranged within a page (books in a library).

For the purposes of the *SAM Web Standards* we recognize two primary types of content from a front-end user perspective: content and metadata. Content refers to titles of pages, body copy, attachments, and so on. Metadata refers to details related to *that* content; posting date, related category, and so on.

Grouping content and metadata separately allows a front-end user to quickly discern the *content* of a page and information *about* the content of a page. Further, content and metadata should be ordered, as much as possible, in order of concern; a posted date may be more important than who posted something from a front-end user perspective. For reference, see the Inverted Pyramid from the profession of journalism.

## Content-focused and printable

For content pages (as opposed to those designed as portals or navigation purposes), the text-based content should not be overpowered by the surrounding navigation or branding (chrome). 

If possible, use the default styles applied by the *US Web Standards*; otherwise, some things to consider:

* Normal operating distance from the screen should be considered (handheld device versus laptop or desktop). 
* To allow users the ability to adjust font sizes using their browser, front-end developers and designers should use relative font sizing (ems) and not stipulate font sizes less than one em. 
* Increased leading (the space between lines) makes it easier for readers to discern one line of text from the next. 

On any given page a front-end user should be able to print (or print to file) the content of that page and receive a well-formed (readable) document, without chrome elements. Print stylesheets can be used to facilitate this outcome by hiding the navigation elements, sidebars, footers (except copyright information, if applicable), and so on. Further, the size of the printed page is usually unknown; therefore, it is important to remove (or override) any fixed width information and replace it with a percentage (usually 100%).

NOTE: Printing a page should only include content considered public unless you add proper document handling, marking and labeling in accordance with Federal regulations.

*[SAM]: System for Award Management
*[IAE]: Integrated Award Environment
*[APIs]: Application Program Interfaces
*[HTTPS]: HTTP Secure
*[HTTP]: Hypertext Transfer Protocol
*[URL]: Uniform Resource Locator
*[URLs]: Uniform Resource Locators
*[HTML]: Hypertext Markup Language
*[CSS]: Cascading Style Sheets
*[AJAX]: Asynchronous JavaScript and eXtensible Markup Language