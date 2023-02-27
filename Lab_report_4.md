## Lab Report 4

  ### Logging into ieng6
  After completing the lab task once, I had to remove the respository
  from my directory.

  This required the command: 
  ```
  rm -r lab7
  ```

  1) After confirming the removal I restarted my lab task
  by logging into the ieng6 account:

  ![Login](Login.png)

  Keys pressed: <up><enter>
  After exiting the server, the ssh command was the first command
  to appear.

  ### Cloning 

  I cloned the repository using this command:
  ![Cloned](Cloned)
  ```
  git clone git@github.com:ramistry/lab7.git
  ```
  
  1) During the repetition of the lab task, I had to use the same
  command.
  
  Keys pressed: <up><up><up><up><up><up><up><up><up><enter>
  The cloning command was the second command to be executed after logging
  in, thus it required so many <up> commands
  
  2) Change directory to lab7.
  
  This required the command:
  ```
  cd lab7
  ```
  Keys pressed: <up><up><up><up><up><up><up><up><up><up><enter>
  
  ### Running the JUnit Tests
  
  This command was used twice during the first try, so I did not 
  have to press <up> till I reached the first command to run the test.
  Instead, I pressed it until I reached the step where I had to re-test
  the corrected code using the same JUnit commands.
  ![JUnit](JUnit.png)
  
  ```
  javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
  ```
  
  Keys pressed: <up><up><up><up><up><up><up><up><enter>
  This compiled the JUnit tests.
  I had to run the tests as well. 
  ```
  java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests
  ```
  
  Keys pressed: <up><up><up><up><up><up><up><up><enter>
  
  The output showed two tests running, out of which one failed.
  
  ![OutputJ](OutputJ.png)
  
  ### Changing the code
  
  The command I used to change the code was:
  ```
  nano ListExamples.java
  ```


