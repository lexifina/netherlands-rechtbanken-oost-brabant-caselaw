# Reproducing this repository

Input: the decision XML (open-rechtspraak format) of davidwickerhf/rechtspraak-opendata revision ba754e64d7286e12968681c11073e8ddf23fc8dc, exports/2026-04-24/<year>.tar.gz (the Rechtspraak open-data XML, unchanged),
parsed by `tools/parse.py`, and lexifina/netherlands-law `main` for the overlay (`tools/bwb_index.py`).

```
python tools/parse.py <archives> <parsed>
python tools/build.py rechtbanken-oost-brabant <parsed> <empty folder> --buckets rb-obr,rb-she --today 2026-11-06
```

Gives 16,326 decision commits and one documentation commit, hash for hash.
