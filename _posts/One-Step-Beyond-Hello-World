# What it's really like learning how to code

Today I started digging into the book *"Automate the Boring Stuff With Python: Practical Programming for Total Beginners"* by Al Sweigart.

One of the initial challenges in just getting started is that I'm already aware of other coding environment tools than the ones suggested in the book (IDLE), which wasn't actually even where the book claimed it would be (no icon in the Python application). I decided to go ahead and use what I know about:
- Terminal for Mac
- Atom (new-to-me editor)
- Jupyter notebook

Moving through some super super basic stuff in the first chapter, I copied out a simple program that asks you your name and age and does some simple operations. That's when I hit my first challenge:

# How Do I Run a Python Program?

I had created and saved my little hello.py script using Atom. Since I don't think you can/don't know how to execute scripts *within* Atom, I decided to execute it in Terminal.

- At this point I had to search the internet to find out how to run a .py script in terminal.
- The answer is `python hello.py`

(By the way, the whole time I've been writing this short blog I've had to also go to another tab to look up Markdown formatting.)

In order to run the command, I have to be in the correct directory, which I had named "Teaching Myself Python." 

Turns out you can't "cd" (change directory) into a directory that's named something with spaces. At least, I don't know how to do that (yet). 

## But first: Re-name the directory
So I re-named the directory in Finder, replacing spaces with underscores.

- Okay, so **then** I execute my script in terminal. 

# Successfully Run Python Program!
Awesome, good job, self. Let's continue learning. 

But wait... I notice a typo in my program. ("lenght" instead of "length")

# Fix a Typo?

I return to my Atom editor, fix the typo, save the file.
I switch back to Terminal, run the script. 

The typo is still there.

## But first: Figure out why the file didn't save properly

I go to Finder and realize there are now TWO folders: "Teaching Myself Python" and "Teaching_Myself_Python."

## Figured out why the file didn't save properly!

Okay that makes sense; the Atom editor never updated (I never told it to update) the folder it was working in, so even though I had changed the name of the folder in Finder, the next time I fixed the typo and hit "save" in Atom, it just re-created the original folder with the spaces and saved it there.

## But first: Change directories

At this point, I decide I should skip ahead to the part of the book where you use Python to copy, rename, and move files and folders because that seems relevant to this whole situation. 

This is done using a model called **shutil**
- I start at the beginning, with 'import shutil, os' 
- The next command is to change directories, 'os.chdir('C:\\')

### But first: Figure out how to specify a filepath on Mac

Okay, but that directory path doesn't register on Mac, so then I have to go to the internet again and try to search to find out how to properly specify a filepath on Mac.

#### But first: Decide why I should bother learning this in Python when I already know some Bash

Then I thought about how I already knew some of these types of commands in bash, so why would I bother to try to do it "blind" in Python when I already know Bash? Well searching "Python vs Bash" led me to a blog post talking about how you can do all the same things you do in Bash in Python but mostly better, and so then I decided okay, I should learn how to do this stuff in Python even if I already know how to do it (faster) in Bash.

#### Decide to stick with Python over Bash!

After more searching, I figured out how to specify a filepath on Mac.

### Figure out how to specify a filepath on Mac!

Back to changing directories, I successfully do so (`os.chdir('Users/me/Coding')`)

## Change directories!

- Then I'm looking at `>>> ` and wondering if I did it correctly. So then I go looking for how to find out what the current directory you're in is.

## But first: Figure out which directory I'm currently in?

Back to the internet. I find [this StackOverflow question](https://stackoverflow.com/questions/5137497/find-current-directory-and-files-directory).

- Okay, now I enter
```
import os
cwd = os.getcwd()
cwd
```
And I see what directory I'm in. 

## Figure out which directory I'm currently in!
**Super, back to work.**

- I go back to Atom, close the old folder with the spaces in it.
- I delete the folder with the spaces, again.
- I open the folder with the underscored in Atom and re-open the python script file.
- I fix the typo and save it in Atom.
- I return to Terminal, to my `shutil` directory situation, and attempt to navigate to the proper directory:
```
os.chdir('/Users/me/Coding/Teaching_Myself_Python')
```

...all seems probably fine...

- I check the current working directory (`cwd`)
```
'/Users/me/Coding'
```

...explitives explode in my brain as I realize I think that I did everything exactly correctly and yet I still do not appear to be able to navigate to the proper directory using Python.

### But first: Figure out why I can't navigate to the proper directory

- I give up on Terminal. 
- I briefly debate just going back to Bash.
- I decide to see if I can get it to work in Jupyter.

I switch to Jupyter and input
```
import shutil, os
cwd = os.getcwd()
cwd
```
And it tells me I'm already in '/Teaching_Myself_Python'

#### But first: Attempt to change directories

Then I try to change into the next higher-level up directory:
```
os.chdir('/Coding')

FileNotFoundError: [Errno 2] No such file or directory: '/Coding'
```

# Give up, call my (software engineer) boyfriend, just go back to Bash in Terminal, run the stupid fixed hello.py script, realize I've spent two hours on this crap, stop "learning to code" for the day.

I don't know if I can do this, y'all.
