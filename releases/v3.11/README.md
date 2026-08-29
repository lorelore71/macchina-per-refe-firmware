# Smart Ropewalk Display Firmware v3.11

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.11.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.11-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.11-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.11-partitions.bin`: tabella partizioni.
- `rigging_bundle_rev56.csv`: pacchetto unico database per aggiornamento robusto su microSD.
- `rigging_db_rev56.csv`: database compatibile/fallback.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.11`.
- Il comando `DIAMETRI` in Calcolo refe diventa `MANOVRE`.
- La pagina manovre mantiene righe piu' alte e stack LVGL aumentato a 8192 byte.
- Il database OTA resta basato su pacchetto unico `rev56-full`.
