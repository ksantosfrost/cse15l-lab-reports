### **StringServer**
![stringserver](lab2ss/stringserver1.PNG)
### **Output**
![hello](lab2ss/hello1.PNG)

**Which methods in your code are called?**
The method called are handleRequest(URI URL). An object of the class Hnadler is made in the same main method causing the method handleRequest to be run.

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
URI url is an object that contains the path /add-message and the query s=Hello. runningString is initially an empty  string. The messageCount is 0 initially.

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**
messageCount becomes 1. runningString becomes "1. Hello"

![lab](lab2ss/hello2.PNG)

**Which methods in your code are called?**
The method that is called is handleRequest. An object of the class Handler is made in the main method causing the method handleRequest to be run. 

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
URI url contains /add-messsage?s=How are you. runningString has "1. Hello". messageCount is 1. 

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**
messageCount becomes 2. runningString becomes "1. Hello  2. How are you"

![login](lab2ss/login1.PNG)
![keygen](lab2ss/keygen.PNG)
![scp](lab2ss/scp.PNG)

**In a couple of sentences, describe something you learned from lab in week 2 or 3 that you didn’t know before.**
I learned how to make a secure copy into a server (scp). I also learned how to make a directory using the command line (mkdir). I also learned how to remove a directory using (rm -r).

