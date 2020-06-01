# Tips & Tricks
This document contains tips and tricks by application. 
If this document gets too big then create a tips-and-tricks folder and parse out by application.

## When Making Decision on a Project use the Negotiating Scale (Credit to Howard Look)
(with building a house example)
1. I have no opinion and just don’t care. Do whatever you want.
2. I have a very, very mild opinion about this, but defer to you. (e.g., kitchen tile)
3. I have opinions. We should talk. I’d like to learn more. I’ll probably be looking at that every day and wonder about 
it, and it’s hard to reverse (e.g., house color)
4. I feel really strongly about this, but not so strongly that it would outweigh one of your 5's.
 (e.g., ice maker in the refrigerator)
5. This is a dig in my heels, I’ll veto if I don’t get my way.


## Excel
### Macro to Automatically Format Spreadsheet
Ed: I use this one a lot to expand columns and freeze panes. Here is the recipe:
* Select `Tools -> Macro -> Record New Macro...` from Tools Menu
* Give in a name like format_worksheet
* Select `Personal Macro Workbook` so macro is available to all excel files you open.
* Assign a short key of your choice
* `Tools -> Macro -> Stop Recording`
* `Tools -> Macro -> Visual Basic Editor`
* Select the module that the macro was recorded in
* Copy & Paste the code below in the module and save
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

## Terminal
### Ignore files that are greater than 50 MB (add to gitignore)
    find . -size +50M | cat >> .gitignore

### Add a terminal shortcut (e.g., to ignore large files)
    alias ignore-large-files="find . -size +50M | cat >> .gitignore"

