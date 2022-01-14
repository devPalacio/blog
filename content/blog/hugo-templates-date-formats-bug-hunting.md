---
title: "Hugo, templates, date formats, bug hunting"
description: "Meta-description summary goes here"
date: "2022-01-13 12:10:00 +0500"
utterances_term: "Hugo, templates, date formats, bug hunting"
categories: []
---

I reached the stage of frustration in which you change 10 things at once and then you're not really sure what fixed it. At least that's how I felt.

When I was adding content to this blog via [Bliss](bliss.js.org) I noted my post date was being set as Jan 1, 0001. 

This led me into the rabbit hole of how Hugo (the really fast static site builder that Bliss uses) uses templates, dates, config files, etc. 

I'll eventually get around to customizing this a bit and making it presentable to prospective employers. First...learn more JavaScript.

After trying a couple config changes with no results, I deleted the date field from the frontmatter (just learned that term 15 minutes ag) hoping it would default to a date from somewhere else. Nope, still Jan 1, 0001. 

After that I chopped off the time from the date component and *VOILA*, it worked!
Simple fix, but ate up about 3 hours of my time. That seems to be the theme with software.

I'd like to try and tackle [this issue](https://github.com/dashtesting/trello-github-etl/issues/5) for the ETL project, especially since it's paid work by the DASH community.

It'll be a strech of my abilitys, but that's probably the best way to learn.

### Day 14 of Javascript30
 - Since objects and arrays are just pointers, you have to be mindful when making a copy of them.
 - MANY ways to do it, which is best? ```Array.from(array), array.slice()```, for loop, and the trendy ```[...spread]``` operator
 - If deep copy is needed (are you sure you need a deep copy?) ```JSON.parse(JSON.stringify(nestedArray))``` will do the trick
 - Objects are a bit different ```Object.assign({}, person, { number: 99, age: 12 });```
### [JS Algo & DS Udemy](https://www.udemy.com/course/js-algorithms-and-data-structures-masterclass/?locale=en_US&persist_locale=) 
 - Did some two pointer challenge questions with no external help. feels good man. [I enjoyed the logic employed in this one](https://github.com/devPalacio/data-struct-and-algos/blob/main/isSubstring.js)
 
 Also got the offer for the no-code web scraping job, debating submitting a counter-offer or declining and persuing the Hack Reactor bootcamp.
