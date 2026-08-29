# Smart Ropewalk Display Firmware v3.13

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.13.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.13-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.13-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.13-partitions.bin`: tabella partizioni.
- `rigging_bundle_rev56.csv`: pacchetto unico database per aggiornamento robusto su microSD.
- `rigging_db_rev56.csv`: database compatibile/fallback.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.13`.
- Diametri normalizzati refe: `0.40`, `0.50`, `0.55`, `0.60`, `0.70`, `0.80`, `0.90`, `1.10`, `1.50 mm`.
- Le ricette sperimentali restano quelle validate: `966/900`, `1000/800`, `960/700`, `876/600`, `840/540`, `820/510`, `760/420`, `670/390`, `500/310`.
- Da `1.10 mm` in su la tensione consigliata e' `250 g`.
- Il database OTA rigging resta basato su pacchetto unico `rev56-full`.
