## Chapter 7 readme

### Do more bullet points:
*Make 20 more directories and remove them all.<br/>
Make a single path of directories that is 10 deep and remove them one at a time just like I did above.<br/>
If you try to remove a directory with contents you will get an error. I'll show you how to remove these in later exercises.*

For the first bullet point I actually went over to the chapter_4 directory in my learn_command_line_exercises and did <br/>
some directory removal.  I had a lot of empty directories that I had made earlier that needed deleting.  For a number of them I had <br/>
added an empty file so I received the `rmdir: Random: Directory not empty` error frequently.  I got around this by  <br/>
deleting the file specifically.  I would `ls` the directory and then `rm` the file that appeared.<br/>
For example, I named a lot the the files 'empty.md' (fittingly enough), so the command I used to delete them was: `rm empty.md`<br/>
Then once the directories were empty I was able to use the `rmdir` command to delete them.
To check that they were gone I would us `ls` from the chapter_4 directory and make sure they didn't show up.

For the second bullet point I cruised back over to the chapter_7 dir (by using `cd ../chapter_7`), and I created the <br/>
single path directory 10 directories deep.  Something to the effect of:
`mkdir -p random/layer_1/layer_2/layer_3/layer_4/layer_4/layer_5/layer_6/this_layer/and_this/this_1_too`<br/>
I then navigated into the second-to-last layer and began `rmdir`-ing my way back out.<br/>
The commands looked something like this:
`cd random/layer_1/layer_2/layer_3/layer_4/layer_4/layer_5/layer_6/this_layer/and_this` <br/>
`ls` which printed `this_1_too`<br/>
`rmdir this_1_too` to delete the directory<br/>
`cd ..` to back out a layer <br/>
`rmdir this_layer`<br/>
`cd ..`<br/>
`rmdir layer_6`<br/>
`cd ..`<br/>
`ls` just to check where I was; the terminal printed: `layer_5`<br/>
`rmdir layer_5`<br/>
`cd ..`<br/>
`rmdir layer_4`<br/>
`cd ..`<br/>
`rmdir layer_3`<br/>
`cd ..`<br/>
`rmdir layer_2`<br/>
`cd ..`<br/>
`rmdir layer_1`<br/>
`cd ..`<br/>
`pwd` to check where I was at: `~/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises/chapter_7/random`<br/>
I then backed out one more layer with `cd ..` and deleted the 'random' directory using `rmdir random`<br/>
<br/>
As mentioned in the third bullet point of the 'Do More' section, I had received the `rmdir: Random: Directory not empty`<br/>
and eagerly await learning how to remove directories that have things in them.<br/>
 <br/>
**Alternative "english" ways of asking you to delete a directory:**

>Can you remove the tmp directory?

I can first check to see if there is anything in the 'tmp' directory using `ls tmp`.<br/>
If the directory is empty then I can easily delete it with the command `rmdir tmp`

>Let's remove the tmp directory.

Ok, so long as the directory is empty we can just run `rmdir tmp`, otherwise we'll require some sort of obscure black <br/>
magic that I am not yet privy too. So we'll have to go in and empty each nested directory and delete them individually outwards.<br/>
If there are no directories in the 'tmp' directory we can delete all the files therein with `rm tmp/*` and then run <br/>
`rmdir tmp` to delete the temp directory.
