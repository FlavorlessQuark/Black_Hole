# Foreword

I wish to become proficient at C, though I have recently learned that knowing other languages helps you become a better programmer.
For now I don't really understand how programming languages differ from each other but I hope to learn this soon.
I think I will also learn Go or Rust, at least the basics. As well as some Perl, JS and maybe the basics of Java as well. I will also try to get a better understanding of C++ and Python.

Here I will record what I have learned about these languages
---

## -Python-

### Beatiful is better than ugly

I now have a fairly good idea of which subjects I should master, was I to get better at python(not in order of importance):

- Firstly, a mastery of **[regex][0]** would be I think, immensely useful. The amount of time it saves is just incredible.
Everything you can do to parse something in a complex function you can do it with one regex. The documentation is also pretty good.

- Second, being able to work with different libraries and have a wide knowledge of them and what they do. I have mostly used re (regex), itertools (to do combination and permuatations) a tiny bit of numpy (for array nonsense), and some misc libs that are version dependent (for example, __future___ for float division results, as I am not using python3). And though my knowledge of them is fairly limited, I'm sure some amazing things can be done with just these

- Third, **[Comprehensions][1]**. Comprehensions are just regex level of useful. I started by making the for loop(s) and then reducing it to a comprehension, but I think I am at a level where I can spontaneously write them (given that they are not too complex).
I'm not sure if these count as comprehensions but these types of expression : `num = sum(map(int, (e for line in input for e in re.findall(r'-?\d*', line) if len(e) > 0)))` are also something worth looking into. Which brings us to the next point...

- Fourht, built-in functions and **[Lambda][2]**. Sum, map, int, list etc... are all functions worth using. There are so many little quality of life things in these that I can't possible write them all here. But I think the real power is they can all be combined. You can for example, apply a function to each item in a list that you just made out of a string of integers. And you can do that in one expression. Lambda and map just go hand in hand.

[0]:https://docs.python.org/3/tutorial/datastructures.html?highlight=comprehension#list-comprehensions
[1]:https://docs.python.org/3/library/re.html
[2]:https://docs.python.org/3/reference/expressions.html
