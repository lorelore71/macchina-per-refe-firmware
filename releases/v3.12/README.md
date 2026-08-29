# Smart Ropewalk Display Firmware v3.12

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.12.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.12-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.12-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.12-partitions.bin`: tabella partizioni.
- `rigging_bundle_rev56.csv`: pacchetto unico database per aggiornamento robusto su microSD.
- `rigging_db_rev56.csv`: database compatibile/fallback.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.12`.
- Il calcolatore refe usa le 9 ricette sperimentali validate per cotone/naturali con trefolo base `0.22 mm`.
- La prova `33` sostituisce la prova `10` per il diametro `0.42 mm`: `1x0.22x3`, `966/900`, `L180`, `150 g`.
- I diametri normalizzati proposti diventano `0.42`, `0.50`, `0.55`, `0.62`, `0.72`, `0.80`, `0.92`, `1.10`, `1.50 mm`.
- Da `1.10 mm` in su la tensione consigliata passa a `250 g`; gli intermedi tra `1.10` e `1.50 mm` restano da validare.
- Il database OTA rigging resta basato su pacchetto unico `rev56-full`.
