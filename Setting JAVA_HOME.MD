##  How to set JAVA_HOME on MAC OS X
To try a specific version of JDK on a MAC computer, we need to set JAVA_HOME
1. Open terminal

1. Comfirm you have JDK by typing "which Java"
    It should say
    ```
    /usr/bin/java
    ```

1. Check you have the needed version of Java, by typing “java -version”
    ```
    java version "1.8.0_251"
    Java(TM) SE Runtime Environment (build 1.8.0_251-b08)
    Java HotSpot(TM) 64-Bit Server VM (build 25.251-b08, mixed mode)
    ```

1. If you have multiple version of Java, you can try 
    ```
    /usr/libexec/java_home -V
    ```
    It should shows:
    ```
    14.0.1, x86_64:	"Java SE 14.0.1"	/Library/Java/JavaVirtualMachines/jdk-14.0.1.jdk/Contents/Home
    1.8.0_251, x86_64: "Java SE 8"	/Library/Java/JavaVirtualMachines/jdk1.8.0_251.jdk/Contents/Home
    ```   
1.  Open ```/.bash_profile```, after decided which Java to be set as JAVA_HOME, by typing
    In my case, I use sublime txt 3 as my default text editor, which is ```subl```
    ```
    subl ~/.bash_profile
    ```
1.  Add this line to ```/.bash_profile```    
    ```
    Export JAVA_HOME="$(/usr/libexec/java_home -v 1.8)"
    Export PATH="$JAVA_HOME:$PATH"
    ```
    ```- V ```means ```version```, where I select JDK 1.8 as my JAVA_HOME
1.  ```Save``` the file and you are all done!
    
    
