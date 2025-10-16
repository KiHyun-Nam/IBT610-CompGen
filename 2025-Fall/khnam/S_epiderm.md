# Staphylococcus epidermidis - public gene

# Reference_1 - Staphylococcus epidermidis strain ATCC 14990 (from NCBI Refseq)

genomic.gff (GFF file) download

# Tool
windows powershell
code: 'Select-string', 'where-objec't, 'measure-object', 'select-object'

#Process
PS C:\Users\LG> Select-string -path "C:\Compgen\genomic.gff" -pattern "`tCDS`t" | Measure-Object | Select-Object


Count    : 2377
Average  :
Sum      :
Maximum  :
Minimum  :
Property :



PS C:\Users\LG> Select-String -Path "C:\Compgen\genomic.gff" -Pattern "`tCDS`t" | Where-Object { $_ -notmatch "hypothetical protein" } | Measure-Object | Select-Object -ExpandProperty Count
2031

#Result
Total: 2377
Public genes: 2071
