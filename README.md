<div align="center">

## Change Form Shape


</div>

### Description

Can Change The Shape of any form
 
### More Info
 
Look Below

The border can be preatty messed up if you don't know what your doing


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[David Serrano](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/david-serrano.md)
**Level**          |Unknown
**User Rating**    |5.9 (621 globes from 105 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Custom Controls/ Forms/  Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/custom-controls-forms-menus__1-4.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/david-serrano-change-form-shape__1-794/archive/master.zip)

### API Declarations

```
Public Declare Function CreateEllipticRgn Lib "gdi32" _
 (ByVal X1 As Long, ByVal Y1 As Long, ByVal X2 As Long, _
 ByVal Y2 As Long) As Long
Public Declare Function SetWindowRgn Lib "user32" _
 (ByVal hWnd As Long, ByVal hRgn As Long, _
 ByVal bRedraw As Boolean) As Long
```


### Source Code

```
Private Sub Form_Load()
Show 'The form!
SetWindowRgn hWnd, CreateEllipticRgn(0, 0, 300, 200), True
End Sub
'E-mail Me at BTMSoft@aol.com for more info
```

