<div align="center">

## Session catcher


</div>

### Description

This simple script yet effective little script prints all active session variables to your browser window. I use it as a troubleshooting tool when debugging my code, and I thought I'd share it with the community.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Lewis Mandrake](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/lewis-mandrake.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |ASP \(Active Server Pages\)
**Category**       |[System Services/ Functions](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/system-services-functions__4-23.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/lewis-mandrake-session-catcher__4-7056/archive/master.zip)





### Source Code

```
<%@ Language=VBScript %>
<%
on error resume next
for x = 0 to session.Contents.Count
Response.Write "<nobr><pre><b>"
Response.write session.Contents.key(x) & " - </b>"
Response.write session.Contents.item(x) & "</nobr><p><br>"
next
%>
```

