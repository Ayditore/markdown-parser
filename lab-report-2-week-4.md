# Welcome to Anthony's Lab Report

In this report, I would like to show you three code change. These changes are made to fix the symptom caused by failure-inducing input  
  
  
## First Code Change: Avoid Reference to Image  

**Screenshot of the first code change difference implemented to fix bug**  
![First code change to fix bug](Code-Change-1.png)  

**Link to the fist test file**  
[First test case link](https://github.com/Ayditore/markdown-parser/blob/main/test-file-2.md) 

**1st Symptom I saw when I ran my code before first code changing**  
![Symptom 1](Symptom-1.png)  

**Description of the relationship between the bug, the symptom, and the failure-inducing input**  
The symptom I saw is that the output of the program includes the reference to the picture.  
From the lab instruction document, I noticed that the output should only include url.  
So I think the symptom is shown because the method cannot differentiate a reference from a url in the input.  
I uses a if statement to differentiate between image and url by checking if the link includes "https" or "www."  
These are two identifier which can identify a url to web page.  

---
## Second Code Change: Situation when the file contains no links  

**Screenshot of the second code change difference implemented to fix bug**  
![Second code change to fix bug](Code-Change-2.png)  

**Link to the second test file**  
[Second test case link](https://github.com/Ayditore/markdown-parser/blob/main/test-file-4.md)  

**2nd Symptom I saw when I ran my code before 2nd code changing**  
![Symptom 2](Symptom-2.png)  

**Description of the relationship between the bug, the symptom, and the failure-inducing input**    
The second symptom I saw is that I met a java outofbound error when running the code.  
I think this symptom is caused by the system cannot find open bracket in the file.  
Then, to fix the bug, I added a if statement to return a empty list if no url bracket is found.  

---
## Third Code Change: Situation when the file uses () but no []  

**Screenshot of the third code change difference implemented to fix bug**  
![Third code change to fix bug](Code-Change-3.png)  

**Link to the third test file**  
[Third test case link](https://github.com/Ayditore/markdown-parser/blob/main/test-file-3.md)  

**3rd Symptom I saw when I ran my code before 2nd code changing**  
![Symptom 3](Symptom-3.png)  

**Description of the relationship between the bug, the symptom, and the failure-inducing input**  
The third sympton I saw is that the program output a empty output when the file only have `()`.  
This symptom reflects that the program does not have the capability to deal with invalid input.  
Thus, I improved the if statement mentioned in the second code change to output a "invalid output" message.  
