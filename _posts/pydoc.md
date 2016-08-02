Pydoc is a tool that comes with Python that can be used for viewing and generating Python documentation. 

The main focus on this feature is because it means that everywhere you go, you have easy access to Python's documentation. 

Thus, you don't need to carry heavy books, or download extra documentation, and best of all, its all accessible from the command line, so I can access documentation while programming without even switching applications. 

The pydoc documentation tool can even be accessed from within Python's interactive interpreter. 

What this means is that if I need to use Python for a simple task like parsing files to make repetitive changes to the text, then I can do so by firing up the Python shell and typing out my program and 

if I can't remember how to do something I just import pydoc and look it up in the documentation.

Why don't we start with using pydoc from the command line. 

Let's say that you're programming in Python and you find you've forgotten how to quit a program. 

You remember that there is function in the sys module, but you can't remember the name of the function (I know you can probably guess that its sys.exit(). 

What do you do? 

Well, in this case you're going to call the pydoc program from the command line, like so:

$ pydoc sys

Keep in mind that the dollar sign, '$', is the command prompt and not part of what you'll actually type into the Terminal. 

Once you've typed in the line above and pressed Return, you should see something that looks somewhat like a man page, and as such, it will act like a man page as well. 

So, since we are looking for a function, we can narrow down our search by pressing the forward slash, '/' (just like in Vi, this allows you to do a text search), character and typing in the search term, in this case we will type in 'FUNCTIONS' (yes, case does matter, so make sure it's in all caps), 

then press Return again to start the search. 

Subsequent searches for the same term can be performed by repeatedly pressing forward slash '/' and Return. 

You can also use the arrow keys to navigate the documentation or just hit the space bar to scan through a page at a time, and to quit your pydoc session, just type the letter q at any time.

## but 

what do you do if you're currently in the Python interactive shell and you need to look up something in the documentation? 

Well, you could always suspend your session with a Ctrl-z, follow the instructions above, and then enter back into the shell where you left off by typing in fg and Return. 

Another option would be to import the pydoc module directly into your current Python shell session and use the help command to find the documentation you need. 

Below is an example of how we might check the documentation for the sys module, like we did in the last paragraph, but this time during an interactive Python session.

&gt;&gt;&gt; import pydoc

&gt;&gt;&gt; import sys   # Import this in order to check its documentation

&gt;&gt;&gt; pydoc.help(sys)

If you'll remember earlier, I mentioned that you can generate HTML documentation using pydoc. 

Below is just one example of how you can do this (by the way, the open command just launches whatever application is the default for dealing with the specified file. 

In my case, it would open the hello.html file in Safari):

$ pydoc -w hello &gt; hello.html; open hello.html

The final feature of the pydoc tool that I want to show you is the web server feature. 

Basically, by calling pydoc with the -p option and passing to it an open port number, you will start a web server that will allow you to access all of the Python documentation on your system through a web browser, and by "all", I mean both Python's own documentation and documentation for your own files as well 

(assuming you've used docstrings correctly and you've added your file's location to the PYTHONPATH environment variable). 

Below is the command that will start your pydoc web server on port 9999:

$ pydoc -p 9999
