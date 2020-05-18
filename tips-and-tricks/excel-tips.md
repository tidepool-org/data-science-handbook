# Excel Tips

#### Turn on filter for every column (Mac)

* CTRL+SHIFT+l (lowercase L)

#### Macro to Automatically Format Spreadsheet

Ed: I use this one a lot to expand columns and freeze panes. Here is the recipe:

- Select `Tools -> Macro -> Record New Macro...` from Tools Menu
- Give in a name like format_worksheet
- Select `Personal Macro Workbook` so macro is available to all excel files you open.
- Assign a short key of your choice
- `Tools -> Macro -> Stop Recording`
- `Tools -> Macro -> Visual Basic Editor`
- Select the module that the macro was recorded in
- Copy & Paste the code below in the module and save

```
Sub format_worksheet()
'
' format_worksheet Macro
'
' Keyboard Shortcut: Ctrl+g
'
    Cells.Select
    With Selection
        .HorizontalAlignment = xlCenter
        .VerticalAlignment = xlCenter
        .WrapText = False
        .Orientation = 0
        .AddIndent = False
        .IndentLevel = 0
        .ShrinkToFit = False
        .ReadingOrder = xlContext
        .MergeCells = False
    End With
    Cells.EntireColumn.AutoFit
    
    Range("B2").Select
    ActiveWindow.FreezePanes = True
    
End Sub
```

## 