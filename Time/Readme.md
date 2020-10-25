# Past light-cone

### Year 2020

**[August](August2020)**

**[September](September2020)**

**[October](October2020)**

## August2020
- With Tiles I hope to be able to make a simple function which tells me what part of the screen has been clicked, and which button this corresponds to.
My main problem is that I am very reluctant to loop trough every object on the screen in order to find which has been hit.
I think the best solution to these kind of problems is to divide the screen in a grid, each square pointing to an array of button pointers in the grid.
I am not sure that this is the optimal solution but maybe a step in the right direction? With this I would still need to iterate through every
button in the grid square, as well as allocate sufficient memory for each and every grid square. Taking all of this into account, would it be
faster /better to only iterate trough all of the object? I think it would be, at least memory wise only up to a certain number of objects...That number is unknown to me...

Maybe I can instead have a sorted array / list and store its median so I can know which half to search? This would still be relatively slow given a large enough amount of numbers.
It is always a tradeoff between speed and memory.

- It will soon be necessary to add a Grid struct so that I am able to clickon things on the screen. The real challenge is to make it so I am able to use it or not use it.. and so it
must not be an integrant part of the tools... I must also restructure my tools so that every file behaves in this way. I think void pointers will be useful for this..
- It might also become necessary to add a lerp functions to Math_Tools... It occured to me when I was thinking about Boids, that they should not snap into an angle but rather get to it over time
For now I do not know how this function works but I intend to find out

- I should write a more extensive Quantum_Vault... The present one only contains a SDL projecttemplate but I do not think I will be satisfied with it much longer... I need command
option so that I can use only what I need... Altough it might be better to have everything in an archive file? I am not sure. I just know the current template is mediocre at best.
This problem is more apparent for Math_Tools. Not all projects require Vectors and misc funxtion but the current Quantum_Vault does not differenciate between them. It might also make
my understanding of code structure better if am able to make most files /functions of my libraries modular and abe to to be used on their own. I am thinking I should add a Master struct to SDL_Tools
as the current Display struct is good for keeping track of things but I do not want to keep everything in the Display struct. Another concern is that the mouse_x, andmouse_y should really be Vector2
although I think I can do some casting magic on that or not use them at all. I am not yet sure that getting the mouse state at every frame is a betetr solution than simply getting it's x and y position.
	Adding a DefineHeader [header name] function script would be nice so I don't have to manually define them all the time

	- Taking a break from coding... Altough before I go, here is a reminder to myself of what to do when I come back : ^ the above about the Vault needs to be done.
In preparation for Obj renderer, make 3d vectors.. I also need to finish restructuring and rewriting SDL_Tools, although I have yet to come up with a decent idea of how to organize everything inside of it.
I think it will soon be time to compile it into an archive file.

---
## September 2020
- As it is customary, not everything goes according to plan. Mine has shifted from C to learning new languages, I shall complete Advent of Code, and learn Python, Java, Go, Rust and Perl.
Then I will come back to my beloved C

There is large performance boost to be had if I were to name my variables properly. I have always tried to name them something short, though it largely restricts my choices. I have spent an hour on advent of code trying to fix something, until I realized I was using the wrong variable. But it was not noticeable as the variable name was descriptive of what I wanted to use.

**Variable names matter**

Finished advent of code 2015 and learnt a lot about python. Now it is time to move on to another language.
I also started a project to add a Git project to the 42 cursus, hopefully it will be good.
I still need to upgrade the Vault. There are many more things I need to add to SDL including an interface.

I think the most important thing I learned from python is simplicity. But also that simplicity isn't just "something that looks simple", it's making something complex as understandable as possible while maintaining it's complexity. that to me is what simple is.

## October 2020

As this month is coming to a close, a lot of things have and are still happenning. 42Silicon Valley is closing. It is time to shift to a more job oriented mindset. C has but a small place in the industry... But I will always love it.
I have finished AoC 2016 and I'm halwayf through AoC 2017. For now I will stop there. I have done both of these in C and learned a lot in the process. I will transfer all of what I have learned to my own C library and improve on it as time passes. I still wish to finish my 3Drenderer, and I had hoped to work on it once my knowledge in C was suffcient. I think I am at a point where I know enough, but unfortunately, due to the current events it will have to be put off a little bit longer. 
I am giving myself until the end of the week to finish up all that can be finished in C , and then I will start learning a language that is more of the industry standard... Most likely Js or C++(I do have some knowledge of C++)

I have looked into Macros and Generic and started woking with them a little more. Although macros aren't especially safe I think they can be really useful for implementing some functions such a python's Map or C#'s foreach. There is also more to learn about optimization as I have just scratched the surface.
I think I also need to to improve in my knowledge of algorithms and data strcutures - it might be beneficial to implement stack, queues, generic trees and dictionaries - These are the ones I am familiar with, but there's a whole part that I don't really know or use (tries, red black trees, etc)  

### The end of an era ... and the start of a new one

While I'm here I want to talk about 42... and how it really changed my life, in a way. Altough I may be sad that my time here is coming to an end so prematurely, I am still grateful for all the valuable lessons I learned.

I can't quite put it into words. First, and obviously, I learned how to program. I don't want to say that it thaught me C, because I learned C on my own. What I learned is much more valuable than any language. From the first day of the piscine to my last day as a cadet and even further in my life. I learned how to learn and I learned how to program and I learned how to succeed. The importance of hard work and perseverance. I remember tackling each project thinking "There is no way I will ever be able to do this, it's far too complicated". Lo and behold, I have achieved level 10.

There was this crazy two month stretch where I had to accomplish 4 levels. I slept 4h a night. I ate once a day. All my energy and willpower was entirely focused on coding. Hours upon hours, it was all that mattered. I would not even go to my desk, I had put my computer on my bed, and I would fall asleep coding. Then I would wake up, and immediatly open my computer and get back to it. More than just the 4 levels I wanted to prove to myself that I could do such an impossible task. In the end, I managed to finish the last project right on the deadline.

Second, the people. The community. Without them, there is no 42. I have met wonderful people here. This entire school is based on the student within its walls. Since there are no teachers, we rely on each other to solve problems and correct our mistakes. When we finish a project we need to get it correct by others in order to get our grade.
Having been to college before, and having absolutely hated it, I can say that 42 is probably the best learning experience for me. Everyone is passionate about coding, everyone will help you if you have trouble.

If there is one thing I regret its corrections. I haven't given the bests ones nor always paid attention, and now that I'm finally ready to learn and embrace the 42 style, it is going away... Hopefully I will bring this to whatever comes next for me.

My group of friends, I am especially thankful for. They are such great people, each smart and talented and I got to watch them and learn from them everyday, without them I would still not know anything.

To all of them : The pumpkin carving, the hikes, the late running DnD campaigns and the 1am In-n-out, the bobba runs, the 12h minecraft sessions, the really early morning breakfasts, thanksgiving, new year, endless xbox playing sessions, the 2am chair races, the chinese drama binging, the early quarantine boredom and the early quarantine board games, the VR sessions, the all nighter game sessions.

**Our time together will be forever engraved in my heart.**

Our roads now part, but someday, I am confident that we will meet again. The world is small
