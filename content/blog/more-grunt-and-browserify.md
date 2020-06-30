---
path: nss-9
date: 2018-04-24T05:00:00.000Z
title: More Grunt and Browserify
description: Grunting continues
---
We continued with Browserify and Grunt this week. It was another challenge and very overwhelming at first. Our task was to create a Movie Maker app. In this app, the user could submit a movie budget (say $100,000) and then start adding components to the movie. These components were things like actors/actresses, locations, special effects, etc. Each movie component cost a certain amount of money that was added or removed from the budget depending on if it was part of the movie or not. As well, there was a progress bar to show if the movie completed all the requirements. Finally, text colors had to be changed based on the status (green was under budget, red was over budget, etc). 

At first, this project was quite overwhelming. There were so many moving parts and things to tie together, it kind of made my head hurt! Working with our team was a big help, breaking down the requirements and the functionality needed was important. One piece at a time, not the whole thing!

This week, the whole class had study group at the same time and place. Our instructors knew we would need more help with the added complexity this week. It was super helpful to have them ready to assist. I chatted with Callan twice when I got stuck. Both times, I made very subtle mistakes, but it totally broke the app from moving forward. One of the things she told me or corrected me on was extremely helpful. In a file \`data.js\`, I had code similar to this: 

\`module.exports = { doSomething, doSomethingElse, };\`

When I tried to reference these functions, I kept trying","\`doSomething(foo)\` and \`doSomethingElse(bar)\`

These wouldn't work and I wasn't sure why. I triple checked for spelling errors, I checked my \`require\` statements, everything looked fine! Callan simply said, 'you are exporting an object from data.js, so how do you reference things inside that object?'. I kind of paused and thought for a second. Dot notation! That's it. I made the connection between the export and the call and what I was missing. It should have been \`data.doSomething(foo)\`! Once I understood what was happening, it made a lot more sense how to properly structure my calls. One of those enlightening moments!