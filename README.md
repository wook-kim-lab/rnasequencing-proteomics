# rnasequencing-proteomics

This is a data repository for the manuscript "Global analyses identify a putative type VI secretion system that contributes to RsmE-mediated spatial structure formation in *Pseudomonas fluorescens* Pf0-1"
 
Raw fastq paired reads for each sequenced isolate can be retrieved from the NCBI Sequence Read Archives (SRA) here: http://www.ncbi.nlm.nih.gov/bioproject/1561030

## Scaffold file, split into two parts

`WT_vs_delRsmE_Pf0-1_search.sf3` (42.6 MB, Scaffold) is split into two zip parts, because GitHub's web upload accepts at most 25 MB per file:

- `WT_vs_delRsmE_Pf0-1_search.sf3.z01` (20.0 MB)
- `WT_vs_delRsmE_Pf0-1_search.sf3.zip` (19.0 MB)

## Rejoin and extract

Download **both** files into the same folder, then:

**macOS / Linux (Terminal):**

```bash
zip -s 0 WT_vs_delRsmE_Pf0-1_search.sf3.zip --out joined.zip
unzip joined.zip
```

**Windows:** open `WT_vs_delRsmE_Pf0-1_search.sf3.zip` with 7-Zip and extract.

Double-clicking the .zip in macOS Finder does not work for split archives; use the Terminal commands above.

## Check the file

SHA-256 of the extracted `.sf3`:

```
c12f4c6a1c122ef45cbe93eca96d97d2ea9b1cd92a0cd38a322827caf674defd
```

Check on macOS/Linux with `shasum -a 256 WT_vs_delRsmE_Pf0-1_search.sf3`. Open it in Scaffold (the free Scaffold Viewer works).
