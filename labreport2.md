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

* Screeshot 1: `add-message?s=hello`

