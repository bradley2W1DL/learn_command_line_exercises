## Chapter 14 readme

**Alternative "english" ways of asking for your working directory:**

>Can you remove blah.txt?

sure can: `rm blah.txt`

>Let's get rid of our development log file.

type: `rm development.log` -- aaaaand it's gone

>Can you remove everything in the slash temp slash foo directory?

As long as you're sure you want all those files gone, type: `rm /tmp/foo/*`

>DANGER: Why is it dangerous to run 'rm -rf /'? DON'T RUN THIS COMMAND.
Why is it a very bad idea?

*See below in the 'Do More' section for complete answer*   Basically, it will delete **everything** with extreme prejudice

### Do More

>Clean up everything in temp from all the exercises so far.

No thanks *(just following instructions)*

>Write in your notebook to be careful when running recursive remove on files.

You have to be careful where you run this command, because the 'recursive' bit implies that the command will run in the
directory that you call it in and then again in any subsequent directories and again in their sub-directories; on an on like
this until it runs out of directories to empty.  And it will perform this command with a finality that will leave you
questioning the very idea that those files existed at all.  This could potentially be a **very** destructive command if
it is run in the wrong directory.  Meaning a directory that contains lots of files and many sub-directory levels. 
The worst possible iteration of this being `rm -rf ~/` which would bring the hellfire of recursive deleting down upon
**all of your files** starting in your root directory. the `f` also has the added effect of force deleting files without
asking for permission.  So yea, be careful with the recursive delete command.
