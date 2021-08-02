### Install Lombok in your IDE (for development purpose):

- Go to lombok maven dependecy folder e.g. {User_Home}\.m2\repository\org\projectlombok\lombok\1.18.12\
- Run lombok jar from command line: 
		
		java -jar lombok-1.18.12.jar
		 
- Install Lomobok from list of IDE. 
- Search inside `eclipse.ini` file that something like this `-javaagent:C:\Program Files\eclipse\lombok.jar` added
	
- Re-launch Eclipse

### Compile lombok project from commandline:

- javac -cp lombok-1.18.12.jar Main.java
