# Smart Ropewalk Display Firmware v3.9

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.9.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.9-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.9-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.9-partitions.bin`: tabella partizioni.
- `rigging_db_rev56.csv`: database compatibile/fallback per aggiornamento dati su microSD.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.9`.
- Scelta vascello separata dalla lista manovre.
- Il vascello selezionato resta salvato e viene mostrato nello splash.
- La lista manovre usa il vascello salvato senza richiedere riconferma a ogni avvio.
- Dettaglio manovra con testo completo e comando `APPLICA A RICETTA`.
- Lettura dati rev56 da microSD: `ships.csv` e `rigging_classes.csv`, con fallback su `rigging_db.csv`.
