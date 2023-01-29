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
 2) This is the result of adding messages: !(Image)[outcome.png] !(Image)[outcome2.png]
