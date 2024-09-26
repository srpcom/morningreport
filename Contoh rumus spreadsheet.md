Rumus 1 
membuat nomor urut
```
=SEQUENCE(counta(B2:B))
```
Rumus 2
Membuat tanggal, menghilangkan format jam dan detik, hanya tanggal saja, misal sumber data tanggal ada di kolom D
```
=ARRAYFORMULA(if(($C$2:$C)="";"";INT($D$2:$D)))
```
Rumus 3 mengcopy kolom
```
=ARRAYFORMULA(if(($C$2:$C)="";"";($D$2:$D)))
```
Rumus 4 Importrange
```
=IMPORTRANGE("https://docs.google.com/spreadsheets/d/1rCUL4DQ2xqgoET_iN6kHH8lwhiIh9JysDE92e1s1Qx4/";"Sheet1!S1:X")
```
Rumus 5 Mengambil data unik, utuk data dropdown dinamis
```
=UNIQUE(Sheet1!B2:B)
```
Rumus 6 Query
```
=QUERY(Sheet1!B1:F; "SELECT * WHERE (" & IF(C1=""; "1=1"; "B = DATE '" & TEXT(C1; "yyyy-MM-dd") & "'") & ")"; 1)
```
untuk penjelasan rumus pakai saja chat gpt
