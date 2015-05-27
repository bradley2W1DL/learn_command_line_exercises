##Chapter 8 Readme

>Explain the `pushd` and `popd` commands in your own words

`pushd` : This command essentially saves your current directory, "pushing" it onto a list, and then goes to <br/>
whatever directory was entered as an argument. <br/>
For example: if I am in the directory `~/workspace/` and pass `pushd davinci_coders_t2_2015/homework` to the terminal, <br/>
the command will save my original location and move me into the `homework` directory.<br/>
<br/>
Then if you pass the `pushd` command without any arguments it will switch you back and forth between your current<br/>
directory and the one that you last "pushed".


`popd` : This command works with the pushd command and it basically removes paths from the list that pushd had added to, <br/>
this also effectively moves you back to the directory you were in before calling the last pushd command.<br/>
<br/>
**In other words**, if I call...<br/>

`pwd` => `~/workspace`<br/>
`pushd davinci_coders_t2_2015/homework` => moves me into `homework` directory<br/>
`pushd learn_command_line_exercises/chapter_8/temp` => moves me into `temp` dir for chapter_8<br/>
Now in the 'pushd' buffer I have two previous paths saved, I can switch between my current directory and the last path <br/>
that I "pushed" by simply passing `pushd` without arguments.  I can also backtrack using `popd`<br/>
`popd` => Moves me back to `~/workspace/davinci_coders_t2_2015/homework`<br/>
`popd` a second time => Moves me back another step to `~/workspace`<br/>
Now I'm back at my original path, and if I try to call `pushd` without any arguments I get the error `bash: pushd: no other directory`<br/>
This is because there are no paths "pushed" onto that 'pushd' directory stack.<br/>

##Do More Section
**Explain what directories you visited**
<br/>
>Use these commands to move around directories all over your computer.

`pwd` => `~/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises/chapter_8/temp`<br/>
`pushd stuff/things/frank` => 'frank' directory <br/>
`pushd joe/alex` => moves to 'alex' directory <br/>
`pushd` => moves me back to 'frank' directory <br/>
`pushd` => moves me back to 'alex' directory <br/>
`popd` => moves me to the 'frank' directory, but removes the 'joe/alex' path from the directory stack<br/>
`pushd` => now moves me back to the 'temp' directory<br/>
`pushd` => moves me back up the 'frank' directory<br/>
`popd` => moves me back to the 'temp' directory<br/>
Now `pushd` passed without any arguments will return: `bash: pushd: no other directory` because the <br/>
directory stack is empty.

>Remove the i/like/icecream directories and make your own, then move around in them.

From the `~/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises/chapter_8/` directory...<br/>
type: `rmdir -p i/like/icecream` -- this removes the entire path <br/>
To create the new path that I was navigating around in above type: `mkdir -p temp/stuff/things/frank/joe/alex/john/`

>Explain to yourself the output that pushd and popd print out to you. Notice how it works like a stack?

So, I made a stack directory four deep, so when I type `pushd` I get...<br/>

`~/Pictures/Backpackin ~/Documents/Anki ~/Downloads ~/workspace/davinci_coders_t2_2015/homework ~/workspace`

This shows **all** the different paths in my directory stack, with the most recent path "pushed" listed first.<br/>
So I can tell that if I pass `pushd` without any arguments I will be directed to `~/Documents/Anki` directory, and <br/>
the directory stack now looks like this:<br/>

`~/Documents/Anki ~/Pictures/Backpackin ~/Downloads ~/workspace/davinci_coders_t2_2015/homework ~/workspace` <br/>

I can then start popping things off the directory stack using `popd` <br/>

1. `popd` => `~/Pictures/Backpackin` and the directory stack is: `~/Pictures/Backpackin ~/Downloads ~/workspace/davinci_coders_t2_2015/homework ~/workspace`<br/>
2. `popd` => `~/Downloads` -- Directory stack = `~/Downloads ~/workspace/davinci_coders_t2_2015/homework ~/workspace`<br/>
3. `popd` => `~/workspace/davinci_coders_t2_2015/homework` -- Directory stack = `~/workspace/davinci_coders_t2_2015/homework ~/workspace`<br/>
4. `popd` => `~/workspace` -- Directory stack now just has `~/workspace` in it.<br/>
