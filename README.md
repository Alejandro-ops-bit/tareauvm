# tareauvm
Sub Cobertura()

Dim lastcell As String

    ' Esto es para borrar todos los datos de estas columnas
    Columns("D:F").Select
    Selection.ClearContents
'   ' Esta parte es para limpiar los datos de esas celdas
    Range("D1:E2").Select
    Selection.ClearContents
    ' Esta parte es para poner los titulos en la celda
    Range("D1").Select
    ActiveCell.FormulaR1C1 = "Región"
    Range("E1").Select
    ActiveCell.FormulaR1C1 = "Estación"
    Range("D2").Select
    Application.CutCopyMode = False
    Application.CutCopyMode = False
    ActiveCell.FormulaR1C1 = _
        "=VLOOKUP(RC[11],'[Cobertura Conglomerada 99 Min.xlsx]CP'!
