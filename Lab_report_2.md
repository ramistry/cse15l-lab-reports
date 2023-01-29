## Part 1: Lab Report 2
_Creating a String Server:_ 

1) This is what the code looks like: 
```   
String line = "";
    public String handleRequest(URI url) {


            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {

                    line += (parameters[1] + "\n");
                    System.out.println("Path: " + url.getQuery());
                    return line;
                }
            }
            return "404 Not Found!";
        }
    }
 ```
 2) This is the result of adding messages: ![Image](outcome.png) 
 3) Outcome after changing: ![Image](outcome2.png)
 4) The methods that are called are: ".contains()", ".getQuery()",".split()", and ".equals()".
    1) .contains checks if a particular String contains a particular segment.
    2) The argument consists of the thing that is being compared, which is "/add-message". 
    
    1) .getQuery is checking what s=xyz is being set to.
   
    1) .split splits the path into two parts at the point where it finds an "="
    2) argument consists of the String "="
    
    1) .equals deep compares the two elements 
    2) agument consists of "s"
