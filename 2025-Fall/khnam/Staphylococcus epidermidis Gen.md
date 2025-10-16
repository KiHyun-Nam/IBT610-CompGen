# 🧬 Staphylococcus epidermidis Gene Annotation Summary

## 📖 1. Reference Genome Information

- **Source:** [NCBI RefSeq](https://www.ncbi.nlm.nih.gov/)
- **Organism:** *Staphylococcus epidermidis* ATCC 12228  
- **Assembly Accession:** GCF_000007645.1  
- **File Type:** `genomic.gff` (RefSeq)  
- **Annotation Summary:**
  | Category | Count |
  |-----------|-------|
  | Total Genes | 2,368 |
  | Coding Genes | 2,232 |
  | CDS (with protein) | 2,232 |
  | RNA Genes | 84 |

---

## ⚙️ 2. How to Count Genes from a GFF or GFF3 File

### 🧩 Option A — PowerShell (Windows)
```powershell
# Count the number of CDS entries in the GFF file
Select-String -Path "C:\path\to\genomic.gff3" -Pattern "`tCDS`t" | Measure-Object
