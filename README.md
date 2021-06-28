# CS305-Project-2
CS 305 project 2 portfolio submission

**Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?**
 
Artemis Financial is a company that processes financial transactions for customers. Things like checking balances, deposits, and withdrawals were likely some of the use cases that they needed from their software. The primary job they asked of us was to look over their software to make sure that it was as secure as possible. They did not want to have any unnecessary vulnerabilities and wanted to know about any that existed. They needed help establishing certificate checks and a checksum into their software and which algorithms to use.
 

**What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?**

I felt that I did a particularly good job in coming up with ways they could improve their dependencies. There are many that can be fixed by updating the version of the dependencies that are used. There are also a few false positives that show on the report, and I was able to supress those.


**What about the process of working through the vulnerability assessment did you find challenging or helpful?**

I had a challenge with the vulnerability assesment at one point because one of their updates during our class stopped it from working. They frequently update the OWASP version and I noticed they had updated it again a few days later and patched the issue. I also found it helpful because it taught me to look at the dependency tree in eclipse. At first it didn't appear that I was using some of the dependencies that were listed in the report. Once I found the tree I was able to see that they were nested inside of other dependencies.


**How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?**

To ensure the best security possible I looked up the most advanced encryption key that had smallest chance of collision. I was able to find that a SHA-256 key has an astronomically small chance of running into a collision. The checksum that I implemented should always make sure the software that users download is valid.


**How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?
What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?**

I was able to make sure the application was functional because I was able to run it in eclipse. Then, I was able to access the server from my browser, and see both the checksum and certificate that I had implemented. I also ran the OWASP vulnerability check after making my changes and found that no new vulnerabilities were introduced.


**Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?**

This is a good example that shows how I can develop code while keeping the security in mind. While developers aren't necesarily IT, they need to work together to make sure everything is secure. From a developer perspective, it's very valuable for me to be able to check my own code for vulnerability. It also shows that I can implement cryptography and certificates into my code.
