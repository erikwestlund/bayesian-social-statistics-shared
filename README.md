# Bayesian Social Statistics: shared files

This repository holds files shared by the R, Python, and Stata projects of
the Bayesian Social Statistics series. Each project includes it as a git
submodule at `shared/`.

- `data_spec/`: one file per data set (`els.csv`, `hsls.csv`): the NCES
  variables kept, with their new names, labels, nonresponse and skip codes,
  recodes, and value labels.
- `data_locations.csv`: every file each project downloads from NCES or
  extracts from a downloaded zip, one row per file: its data set
  (`dataset`), where it goes (`path`), where it comes from (`url`, or `from`
  for the source zip), and its SHA-256, Stata checksum (`crc`), and size in
  bytes.
- `docs/`: how the HSLS:09 data spec treats NCES reserve codes
  (`missing-data.md`) and the HSLS:09 codebook (`codebook.md`).

Clone a project with its shared files:

```
git clone --recurse-submodules <project URL>
```
