## Chapter 11 Readme

*Alternative "english" ways of asking for your working directory:*

>Can you rename foo.txt to blah.txt?

but of course: `mv foo.txt blah.txt` => this will effectively rename the file

>Can you move the production.log file in the log directory to slash temp?

yep, just type: `mv log/production.log /tmp/`<br/>

>Can you zero out that file?

you could do this to zero that file out...<br/>
`cd /tmp`<br/>
`touch empty.log`<br/>
`mv production.log empty.log` => this would zero out the 'production.log' file and rename it 'empty.log'<br/>

*you could also...*<br/>
`rm /tmp/production.log` <br/>
`touch /tmp/production.log` <br/>
=> this would zero out the 'production.log' file by deleting it and then creating an new, empty 'production.log'<br/>

`echo '' > production.log` => would also effectively zero the file out by overwriting its contents.
