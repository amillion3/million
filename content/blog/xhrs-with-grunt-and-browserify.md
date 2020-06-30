---
path: nss-8
date: 2018-04-15T05:00:00.000Z
title: XHRs, with Grunt and Browserify
description: Grunt
---
Our task this week was diving further into XHRs. More XHRs you say? Yes, we tackled XHRs in the context of multiple JSON files. We had to figure out how to combine them without simply pushing them into a global variable. It would have been 10x easier to assign them to a global and work on them from there. However, globals are less secure than variables scoped within functions, so it's a natural choice in favor of security.

I wrote my code partially once and then deleted it. I wrote my code again, late into Friday and then thought I was on the right track. However, after a very helpful discussion in class the next day, I realized my approach was not what I wanted. Refactoring for the third time was the ticket! The discussion in class really helped clear up the proper way to handle multiple JSON files in a secure manner. It takes some jumping through hoops and JS trickery, but it's quite doable. I really struggled with this Friday night, so finally understanding it was so satisfying!

After the functionality was in place, it was time to use Bootstrap. It took more effort than I thought it would to get Bootstrap working the way I wanted. A little out of practice, sure. Once I got back into it, I felt a little more comfortable. The docs are great and it's quite common, so questions and answers litter the internet.

We are starting Grunt and Browserify now, hooray! This is totally new to me and it seems pretty neat. Setting up new projects takes a lot more effort than before. I'm sure it will speed up in the future, but for now, I have to go step by step through a PowerPoint. I like the live-reload feature, it's pretty slick. For my personal projects, a CSS Autoprefixer will be amazing, I can't wait to use that! There is a lot to this, so reading the docs and watching some videos will be helpful for me.

Understanding how all the pieces fit together in Grunt/Browserify is a challenge. It's kind of like a tangled web that you have to follow and track the pieces. Once you do it a few times and then start stringing things together, it makes more sense. I was even able to throw in a randomizer function on my pet adoption website.

I like the linter we are using too! Well, like is too strong of a word. I like that all of us are held to the same styling and we aren't supposed to cheat past it. It has certainly helped me identify when I inadvertently did something wrong too, such as using \`let\` instead of \`const\`. Standardizing our code will make it more readable when working with a team or helping to debug a cohort member's code.