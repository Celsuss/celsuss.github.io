+++
title = "My thoughts on switching to vim bindings"
author = ["Jens"]
date = 2024-01-24T23:27:00+01:00
draft = false
+++

Even though I have been using spacemacs as my daily driver for coding and
writing blog posts like this one I have been using the traditional emacs
keybindings.
Going from "normal" keybindings to emacs felt like a great productivity boost,
this made me wonder if maybe there is an even better option.
Enter vim keybindings, in this post I will explain my experience switching to
vim keybindings and what my
thoughts are about it. I will not tech you how to use vim here,
there are some great resources for that and I will mention some of them that I
used to learn vim.


## Why did I decide to switch to vim keybindings {#why-did-i-decide-to-switch-to-vim-keybindings}

As a software developer the keyboard is one of my most important tools.
It allows me to transfer my thoughts from my brain to the computer.
So it's important for me to use the keyboard in the best possible way.
I'm sure most developers don't give much thought into the keyboard layout, I
know didn't spent a lot of time thinking about it. It was when I switched to
emacs and started using it's keybindings that I really started to think about
it. The keybindings in emacs felt much more effective then what I used before.
So I decided that before I get too used to emacs keybindings I would try
something else.
This is when I decided to switch to vim keybindings.


## Learning vim: my initial steps {#learning-vim-my-initial-steps}

I knew that using vim keybindings would be a big change, if you have ever
accidentally opened vi and can't figure out how to exit
then you understand what I mean.
So I decided to find some tutorials to get me started.
The first thing I tried was the evil-tutor in emacs, this is a great way to get
a feel of the basics of vim.

I also found an online "game" called vim-adventures, this I found as a great way
to practice the muscle memory of using vim. You can find the game at
<https://vim-adventures.com/>. But in the end the only way to get good at using
vim is to start using it in your daily life.

My last learning resource that I want to present is the [practical Vim](https://pragprog.com/titles/dnvim2/practical-vim-second-edition/)
book. This is a great resource to learn plenty of neat tricks and tips
for using vim keybindings.


## What I like with vim {#what-i-like-with-vim}

Some people maybe think that vim keybindings is just a keyboard layout.
But besides just different keys for things like copy and paste it also
gives you a lot of new functionality.
The biggest change is probably that vim uses different modes.
When in normal mode you can't write any text, instead you can move the cursor
and manipulate existing text. Visual mode lets you select text that you
can then use normal mode to manipulate.
If you want to type text then you enter insert
mode by using either 'a' or 'i'. These two keys both enter the insert mode but
'a' enter insert mode after the cursor and 'i' enters insert mode before the
cursor.
These are not even all the ways to enter insert mode but the most basic.


### My favorite commands {#my-favorite-commands}

There was one command that I quickly came to love and use a lot, that is the
**.** key in normal mode. When in normal mode you can press **.** to repeat the
last change that you did.
This may at first not seem as that much until you realize how much one change
can contain.
An example is from normal mode press `cw` to delete a word and enter into
**insert mode**, then type the word 'hello' and press `<ESC>` to go back to normal mode.
Now we can move the cursor to any word, press `.` to replace the word with
the word 'hello', now you got can replace any word with the word 'hello'
just by pressing one button.


### Combining commands {#combining-commands}

One of the strengths with the vim keybindings is that they can easily
combined with each other.
Lets look at another example for this, if we press the keys `dw` in
**normal mode** we can delete the word under the cursor, you can read the
keys as a shortcut for the words "delete word". But if we add
a number to this combination, `d2w`, then the current and next word will be
delete, just like saying "delete 2 words".


### Be kind to your pinkie finger {#be-kind-to-your-pinkie-finger}

Using emacs keybindings make you stretch your little fingers a lot to press keys
like `<ctrl>` and `<alt>`.
Most people seem to have accepted this as a fact of life, just like I used to
do. But once you start using vim you start to notice how much less you need
to move your hands around the keyboard.


## The biggest challenge {#the-biggest-challenge}

It took some time to get used to navigating using the keys `h`, `j`, `k` and
`l`. I had the most problem with remembering `j` (down) and `k` (up) but
I finally came up with the trick of thinking of 'j' as an arrow pointing down.
But ultimately this is just muscle memory.

What really took a change in my mindset was two related things. The first
was that while in **insert mode** I can move back and forth on the current line
but I can't move vertically. For a while I was considering to add custom
keybindings to allow this but I decided not to do that. I thought there
probably was a reason for this and I should learn the reason before I decide
to change it or not.

This leads me to the second change of mindset, when do I press `<ESC>` to
leave **insert mode** and enter **normal mode**? The first answer you will
probably thing is "when I'm done inserting". While it is true that you should
quit **insert mode** when you finish inserting but there are a lot more to take
in to consideration.

Earlier I talked about how using the `.` key repeats the last change, just like
the key `u` undoes the last change. This is important because the process of
entering **insert mode**, writing some text and then exiting **insert mode** counts
as one change. In this way you can think of exiting **insert mode** and entering
**normal mode** creates a checkpoint. Now you can repeat, undo or redo the undoes.

When writing this text I will leave **insert mode** whenever I'm finished
with a paragraph or I need to stop and think, this way I can think of my
inserts as chunks of text on a stack.


## My conclusion {#my-conclusion}

Now after using vim keybindings I don't think I can ever go back.
Not only does it let me write code and manipulate text faster but the decreased
hand movements and stretching of the hand can have medical benefits.
So would I recommend vim keybindings? Absolutely yes!
