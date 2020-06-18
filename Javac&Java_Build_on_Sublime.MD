1.  Open ```Sublime Text 3```
1.  Select ```Tools``` > ```Build_system``` > ```New Build System``` in sublime txt3
The sublime txt3 will automatically pop-up a file for you


1.  Paste following codes in your file

    ```
    "cmd": ["javac $file_name && java $file_base_name"],
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
    "path": "/usr/bin/",
    "selector": "source.java",
    "shell": true
    ```
1.  Save as ```Java&JavaC.sublime-build```, which saved at ```/Users/Which_User/Library/Application Support/Sublime Text 3/Packages```

1.  Quit ```sublime txt 3```, and open one JAVA files with ```sublime txt 3 ```

    ```Tool``` > ```Build_system``` >```Java&JavaC```
    
1.  Run a Java program

    ```
    Command + b 
    ```





