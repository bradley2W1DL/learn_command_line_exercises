##Chapter 22 Readme
___

###Do More

>Take and list out all the environment variables you've found and then go look up what they are online.<br/>

1. rvm_bin_path => shows the path for my ruby version manager bin directory
2. TERM_PROGRAM => displays the terminal program that I'm using (iTerm.app)
3. GEM_HOME => shows the directory path where my Gems are stored
4. SHELL => Stores the full path-name to the shell
5. TERM  
6. IRBRC
7. TMPDIR => gives the exact location of my /tmp directory
8. Apple_PubSub_Socket_Render
9. OLDPWD => show the working directory that i was in just before the one I'm currently in.
10. MY_RUBY_HOME => shows the directory that my enabled version of Ruby is operating out of
11. USER => shows my username
12. \_system_type 
13. rvm_path => show location of my ruby version manager
14. SSH_AUTH_SOCK
15. rvm_prefix => shows prefix directory for ruby version manager.  In this case it's my home directory.
16. PATH => tells the unix shell where to look for program files when trying to run commands
17. PWD => Shows present working directory
18. LANG => shows my currently enabled language.  In my case it's en_US.UTF-8 (American English)
19. ITERM_PROFILE => gives the name of my iTerm visual profile.
20. \_system_arch
21. XPC_FLAGS
22. PS1
23. \_system_version => gives the operating system version (10.10 on my comp)
24. XPC_SERVICE_NAME
25. rvm_version
26. SHLVL
27. COLORFGBG
28. HOME => shows home directory path
29. ITERM_SESSION_ID => shows the session I'd for current running iTerm shell
30. LOGNAME => shows the currently logged-in user (username)
31. GEM_PATH => gives the different directories that the computer should look in for Ruby Gems
32. RUBY_VERSION => shows the currently enabled version of Ruby (2.2.1 on my machine)
33. \_system_name => show the name of my operating system (OSX)

>Read the man page for env again. What else can it do?
____

###Alternative "english" ways of asking for your working directory:
  
>Can you set the debug environment variable to true?

sure thing: `export DEBUG=true` => you can then check this by typing: `echo $DEBUG` in the CLI

>Can you remove the debug environment variable?

also yes: `unset DEBUG` => this will completely remove the $DEBUG environment variable
