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

There is large performance boost to be had if I were to name my variables properly. I have always tried to name them something short, though it leargely restricts my choices. I have spent an hour
on advent of code trying to fix something, until I realized I was using the wrong variable. But it was not noticeable as the variable name was descriptive of what I wanted to use.
Variable names matter

Finished advent of code 2015 and learnt a lot about python. Now it is time to move on to another language.
I also started a project to add a Git project to the 42 cursus, hopefully it will be good.
I still need to upgrade the Vault. There are many more things I need to add to SDL including an interface.

I think the most important thing I learned from python is simplicity. But also that simplicity isn't just "something that looks simple", it's making something complex as understandable as possible while maintaining it's complexity. that to me is what simple is.
