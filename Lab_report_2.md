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
    * .contains checks if a particular String contains a particular segment.
    * The argument consists of the thing that is being compared, which is "/add-message". 
    * .getQuery is checking what s=xyz is being set to.
    * .split splits the path into two parts at the point where it finds an "="
    * argument consists of the String "="
    * .equals deep compares the two elements 
    * agument consists of "s"

5) The field that changes is the line field. A new string is concatenated so the value of the line variable changes.
