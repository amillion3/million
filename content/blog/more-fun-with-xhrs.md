---
path: nss-7
date: 2018-04-08T05:00:00.000Z
title: More fun with XHRs!
description: XHR fun
---
This past week was kind of a roller coaster. Big ups and downs, but thankfully, the downs didn't last too long. Our big assignment this week was to create a solar system single-page app. The page upon loading would have 8 cards, one for each planet. When you put your mouseover the card, an image of the planet would show up. When you click it, the cards would go away and one big card would appear. This would show a large image of the planet, with additional details about the planet. In addition, there is basic search functionality at the top of the page. Fun project!

Two things really threw me off about this project:

1. Trying to make a single XHR call to do all the work.
2. Figuring out how to pass JSON data around as needed.

In regards to the first point, I tried and tried to make a single XHR call that would power the whole page. I knew global variables were a no-no because of security issues and the fact that in the real world, data from a database could change at anytime. My initial thought was to try and capture the JSON data and allow other functions to call and have it returned. I went through a few iterations of this and seemingly endless console.log() statements. I finally gave up on this idea and decided to see what others were doing. As it turns out, multiple XHR calls are needed!! That would have made it so much simpler and saved time.

The second point, passing JSON data where it's needed was my final big hurdle on this project. Now that I had two XHR calls (one for the mini-cards and one for the big-cards), I wanted to pass the data out to other functions after a 'click' event. Simple, right? Well...no, not simple. After Googling, digging through Stack Overflow, I was getting the message. You can't pass data through a named function in an event listener. Why!!

Well, no biggie, actually. You can just call an anonymous function and run it right there. Bingo. Nailing that down was huge and I felt quite proud to have solved this issue. I was able to share my knowledge with my teammates and I was happy to help them. I really enjoy the collaborative approach to learning here at NSS. It's more of a sharing knowledge and teaching one another space, instead of the traditional teacher-student relationship I'm so used to.

After all this, I needed to organize my code better and add some comments. It's the most complicated JavaScript I've written and it's easy to get lost in the code. It was well worth the time and I hope it helps whomever looks at my code more easily follow my logic and flow. I wanted to do some bigger refactoring, but I just didn't have the time.