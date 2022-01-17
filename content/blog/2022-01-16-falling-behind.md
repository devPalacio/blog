---
title: "More Dash + Live Coding with AJ Oneil"
description: "Check me out on youtube"
date: "2022-01-16"
utterances_term: "Untitled"
categories: []
---
### More Dash + Live Coding with AJ Oneil
> Check me out on YouTube

Getting my ass kicked by a cold right now. Anyways, I missed yesterdays post so this might end up being another long retrospective.
The highlight of yesterday was becoming YouTube famous and having a well seasoned JS developer guide me while I added a feature to
a codebase he created days earlier. The objective is to extract a trello board, transform it into usable data, and load it into to github.

[Watch me here](https://www.youtube.com/watch?v=dwcXfsgZ12A&t=3315s)...warning. It goes for
nearly 4 hours. At the end of it we did manage to implement the feature we were going for, we just hit a few speed bumps along the way

Key takeaways for me:
 - You have to really understand the codebase before you go adding features, at one point we went through line by line to
 confirm my understanding
 - variables are free, use them! I would keep trying put way too much logic into one line, and I could see AJ dying inside.
 it makes code more readable, for yourself and the next guy.
 - be mindful of your private tokens! I opened my .env file with my github token on stream...and immediately had to go revoke it. oops.
 - sanity check your logic and scope. I implemented a couple minor logic errors that got corrected on the spot. We ended up
 needing more data than intended in a function, so we had to add an argument to the 3 parent functions. I'm still a bit lost
 on that one.

Today I continued but without supervision on the ETL project. Yesterday laid a solid foundation which I could build upon.
I managed to implement slightly more complex logic in a little bit less time. It was the first time I added to and utilized a
module. As a bonus, my code was way more readable.
UPDATE: after running the code for a bit...there's a pesky bug somewhere that's resulting in duplicate fields. Almost had it.


 Also did 2 days of JavaScript30 since my last post.
 - Both days required video help :(
 - Day 16 involved having a css text shadow follow your mouse cursor
   - That requires good familiarity with offsetX, offsetY, offsetTop, offsetLeft, and some clever math to keep the shadow on a leash
 - Day 17 involved sorting an array but ignoring words such as the, a and an.
   - The implementation was just use the .replace method with a small regex `(/^(a |the |an )/i, "")` and when running the sort
   method, just call your new 'strip' function when comparing a to b. Array stays whole, only time string gets manipulated is
   during the comparison.

Anyways, that's all I care to write about today. Til tomorrow.

