<div align="center">

## bDebugmode


</div>

### Description

detect if you are running in debugmode (vbstudio) or in compiledmode (.exe) at runtime !
 
### More Info
 
true or false

none (offcourse :) )


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[skizmo](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/skizmo.md)
**Level**          |Intermediate
**User Rating**    |4.4 (31 globes from 7 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0, VB Script, ASP \(Active Server Pages\) , VBA MS Access, VBA MS Excel
**Category**       |[Debugging and Error Handling](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/debugging-and-error-handling__1-26.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/skizmo-bdebugmode__1-23368/archive/master.zip)





### Source Code

```
Private Function bDebugMode() As Boolean
  On Error GoTo ErrorHandler
'in compiledmode the next line is not
'available, so no error occurs !
  Debug.Print 1 / 0
  Exit Function
ErrorHandler:
  bDebugMode = True
End Function
```

