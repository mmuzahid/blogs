# Java CommandLine Debugging:
--------------------------------
[Java DOC Ref](https://docs.oracle.com/javase/7/docs/technotes/tools/windows/jdb.html)

### Create a HelloWorld.java


    public class HelloWorld {
        public static void main(String[] args) {
            System.out.println("Hellow World");// line: 3
		    int i = 99;
		    System.out.println("i: " + i);
        }
    }

### Open a CMD window, Compile and Run HelloWorld in Debug Mode. Application will be suspended and wait for a debugger attachement at port `8888`.
    
    javac -g HelloWorld.java
    
    java -Xdebug -Xrunjdwp:transport=dt_shmem,address=8888,server=y,suspend=y HelloWorld



### Open another CMD window and Attach a debugger(JDB) to a Java VM that is already running at CMD window 1

- Attach Debugger at port `8888`

      jdb -attach 8888

### Start Debugging at CMD Window 2

- Set a Breakpoint at `Line 3`

      stop at HelloWorld:3

- Run Application that is suspend at CMD window 1.

      run
    
- Go to next Step

      step
    
- Show Code list

      list

- Show local variables

      locals
      
 - Print a variable e.g. *i*
      
       print i
 
