## How to set ```sublime text 3``` as your default pop-up editor to ```bash``` terminal
```Sublime Text``` includes a command line tool, ```subl```, to work with files on the command line. 
This can be used to open files and projects in ```Sublime Text```, as well working as an EDITOR for unix tools, such as git and subversion.
### Set UP
 The first task is to make a symlink to subl. 
 Assuming you've placed Sublime Text in the Applications folder, and that you have a ~/bin directory in your path, you can run:
 ```
 ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" ~/bin/subl
 ```
### Editor  
  To use Sublime Text as the editor for many commands that prompt for input, set your EDITOR environment variable:
  ```
  export EDITOR='subl -w'
  ```
  Specifying ```-w``` will cause the ```subl``` command to not exit until the file is closed.  


