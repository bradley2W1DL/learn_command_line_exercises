## Chapter 13 Readme

**Do More**

>Make a few more text files and work with cat.

So, I created three new text files (creatively named one.txt, two.txt, and three.txt) I can then display them together <br/>
with the `cat` command or even rearrange the lines depending upon how I pass arguments to `cat`<br/>
For example...

![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/cat_command1.png "Cat command example")

This shows how cat displays files and combines them together.

>Unix: Try cat ex12.txt ex13.txt and see what it does.

`cat ex12.txt ex13.txt` <br/>
displays: <br/>
`Hi there this is cool.`<br/>
`I am a fun guy.`<br/>
`Don't you know why?`<br/>
`Because I make poems,`<br/>
`that make babies cry.`<br/>
 
 => the cat command when passed two files displays both of the files combined together.<br/>
  In other words, concatenated -- which i guess is where the 'cat' comes from.

**Alternative "english" ways of asking for your working directory:**

>Can you show me the contents of database.yml?

type: `cat database.yml` => will show you the entire contents of 'database.yml' file<br/>
in my case this outputs: `Some Random text`

>What is in your Gemfile?

What indeed? You can find out by typing: `cat Gemfile` into the terminal <br/>
this will output a list of all your gems with their version and their dependencies <br/>
I didn't really know about Gemfiles but, "http://stackoverflow.com/questions/14072880/whats-the-use-of-gemfile-in-rails" helped me out<br/>
So in my case, `cat Gemfile` outputs => <br/>`Some more random text`<br/>
                                        `there should be Gem info in here too`
