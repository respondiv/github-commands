### Contains Popular Commands to run github


#### My personal git Configuration


##### changes the settings in git to make it colourful (instead of black and white). The --global will apply the setting to all of the git projects

`git config --global color.ui auto`


##### set sublime text as default editor: -n -> opens in new window; -w -> git waits for us to close sublime before trying to continue

`git config --global core.editor "'C:/Program Files/Sublime Text 3/sublime_text.exe' -n -w"`


##### It's needed, don't know why .. YET

`git config --global push.default upstream`


##### It's needed, don't know why .. YET

`git config --global merge.conflictstyle diff3`


#### Global settings for line endings:  Configure Git on OS X or Linux  or Windowsto properly handle line endings

`git config --global core.autocrlf input`


#### Caching your github password so that you don't need to type it again and again when doing commit

`git config --global credential.helper wincred`


#### Run this command to increase window's path length limit. This will help when you see an error in cloning the repository

`git config --system core.longpaths true`



**Download the files from git-files directory and run following commands**

```
Note: 

git-completion.bash ->  This enables 'Tab Completion' 
This file can also be downloaded from https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash . All you need to do is save as.

git-prompt.sh -> enable git features in prompt (customize git prompt)
This file can also be downloaded from https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh .All you need to do is Save as.


```


###### Open git bash and run following commands


Go to home directory

`cd ~`

Move the `git-completion.bash` from the download folder to home directory. Note when you doing save as it will rename the file to `git-completion.bash.txt`

`mv Downloads/git-completion.bash.txt git-completion.bash`

Move the `git-prompt.sh` from the download folder to home directory. Note when you doing save as it will rename the file to `git-prompt.sh.txt`

`mv Downloads/git-prompt.sh.txt git-prompt.sh`

Download (save) the `bash_profile` file from `git-files' to the download folder as bash_profile.txt and run following commands

`mv Downloads/bash_profile.txt .bash_profile`


**Open .bash_profile file in text editor. On the last line, if needed, update the location of the text editor (like sublime text)**
