# Smart Ropewalk Display Firmware v3.14

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.14.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.14-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.14-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.14-partitions.bin`: tabella partizioni.
- `rigging_bundle_rev56.csv`: pacchetto unico database per aggiornamento robusto su microSD.
- `rigging_db_rev56.csv`: database compatibile/fallback.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.14`.
- Aggiunta ricetta normalizzata `1.20 mm`: `3x0.22x6`, 18 trefoli totali, `670/390`, `L180 -> L152`, tensione `250 g`.
- Aggiunta ricetta normalizzata `1.40 mm`: `4x0.22x6`, 24 trefoli totali, `500/310`, `L180 -> L159`, tensione `250 g`.
- Le prove 49 e 50 confermano la regola: per diametri finali superiori a `1.00 mm` usare `250 g`.
- Il calcolatore refe ora propone 11 diametri normalizzati: `0.40`, `0.50`, `0.55`, `0.60`, `0.70`, `0.80`, `0.90`, `1.10`, `1.20`, `1.40`, `1.50 mm`.
- Il database OTA rigging resta basato su pacchetto unico `rev56-full`.
