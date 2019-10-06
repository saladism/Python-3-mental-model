# Python-3-mental-model
A story to help build the mental model of Python 3.

# Introduction
Here is my attempt at building a mental model of Python 3, with the help of a story.\
This story is written for beginner Python programmers, particularly for children and those who do not have computer science background.\
The story is inspired by a talk I have seen online by Python guru Brandon Rhodes.\
https://pyvideo.org/pyohio-2011/pyohio-2011-names-objects-and-plummeting-from.html \
All mistakes are mine alone, however the code examples in the attached files seem to support this mental model.
Corrections are welcome.

## Imagine Python 3 as a magical realm.  There are few things in this realm.  There is a Genie, a big recycle bin and lots of sleeping princesses.

## Genie: 
This is the Python language it self, to whom you need to make requests with special incantations(syntax).\
The genie makes any “object” you want, as long as you use the special incantations.\
If you ask for another object, the genie does not store the object it just created, but just tosses it in the recycle bin (most of the time) and makes a new object for you.\
If your incantation is incorrect the genie complains with error message(syntax error).

## Objects: 
Well, the genie can’t give you any object you want (that was a lie, unfortunately) but some objects which have specific properties.\
We will discuss 4 of these objects here. These are numbers, words, trains and magic spell boxes.\
Python can make other objects called locked_trains(tuples), named_trains(dictionaries), bookmarks(generators) etc.

## Numbers(integers): 
Python genie can build any number you ask for.\
Genie builds that number, **puts a lock around it** so that it can’t be changed any further and gives it to you.\
Python is good with numbers, so it does the calculations too, if you ask for it.

## Words(strings): 
Anything which you put in between “ and “ or ‘ and ‘\
it can even be an empty word like “” or ‘’, or an empty space such as “ “ or ‘ ‘\
Python again **puts lock around that word**, so it can’t be changed after it is built.

## Trains(lists): 
These are trains which have numbered carriages from 0 onwards.\
Each carriage can hold an object such as a number or word or even another train in it. (Yes a train in a carriage, this is magical realm after all).\
You can add or remove carriages and change the stuff you put in each carriage.\
**There are no locks here.**\
Genie can make an empty train with no carriages, but if you can't  have empty carriages.\
There needs to be some object in that carriage, even if it is empty word.

## Magic spell box(function): 
This is a box with a name on it and some instructions of magic in it.\
You can have some sleeping princess in this box as well. \
That magic spell will come to life when you call it, with **()** next to the spell name. \
When you do that, it actually creates a **sub realm**, where all the magic happens(but that is a separate story).\
At the end of the magic spell usually an object is created(number or word or train etc) or modified(if it is train etc). \
It returns the object it created back to the main realm as long as you put the right incantation to **return** it.

## Sleeping princess(variables): 
If you don’t want the genie to recycle the objects, one of the sleeping princess needs to wake up and hold it for you.\
**They won't wake up unless you give them a name.**\
**They won’t stay awake unless you give them an object to hold.**\
You and python recognise something in your code as a princess because their name starts with a letter without “ or ‘ around it (or with an _ ).\
You can send the princess back to sleep with **del** incantation.\
Then the princess forgets the name, leaves the object and goes back to sleep.

I have uploaded some Jupyter notebook files with, code examples to explain this mental model.
You can download this files and play with them.
The bestway to install Jupyter is with anaconda distribution available at https://www.anaconda.com/distribution/

Download 3.7 version (or higher if available), for your operating system.
Once anaconda is installed, use JupyterLab in the anaconda navigator to open these notebook files.\
<kbd>Shift</kbd> + <kbd>Enter</kbd> to go through each line in the file

You can now skip the file titled 01-Introduction(as it has the same content) and go to file named 02-Variables.

-- Satya Saladi
