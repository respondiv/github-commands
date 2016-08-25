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

git config --system core.longpaths true






