# **Lab Report 2 - Servers and Bugs(Week 3)**

## **Part 1**
* Code for StringServer.java(implemented in the week-2 lab wavelet folder):
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler{
    String message = "";
    public String handleRequest(URI url){
        System.out.println(url);
        if(url.getPath().contains("add-message")){
            String[] parameters = url.getQuery().split("=");
            message = message + "\n" + parameters[1];
        }
        return String.format("%s",message);
    }
}

class StringServer{
    public static void main(String[] args) throws IOException{
        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
}
```


* Screenshot 1: `add-message?s=hello`
![Image](screenshot1.png)
    * The main method were first called to create a new url with port number 2391, and the handleRequest method were called to add a string according to         the query provided. 
    * The main method take the argument by looking at the args[0] and create the new url using that argument as port number. The handleRequest method take       the url created in the main method as argument so that we can make changes to the websit using method inside the Handler class. The value of string         message is now "hello"
    * The value of message changed from "" to "hello".


* Screenshot 2" `add-message?s=cse15LSpring2023`
![Image](screenshot2.png)
    * The handleRequest method were called to add a String according the query provided.
    * The query method take the argument of the same url as screenshot 1. The value of string message is now "hello\ncse15LSpring2023"
    * The value of message changed from "hello" to "hello\ncse15LSpring2023".


## **Part 2**
*The bug I choose: averageWithoutLowest*

* A failure-inducing input:
  ```
    @Test
    public void test3(){
        double[] input = {2,2,4};
        assertEquals(3,ArrayExamples.averageWithoutLowest(input),0);
    }
  ```
* An input that does not induce a failure:
  ```
    @Test
    public void test4(){
        double[] input = {1,2,4};
        assertEquals(3,ArrayExamples.averageWithoutLowest(input),0);
    }
  ```
 *
  
  
    





