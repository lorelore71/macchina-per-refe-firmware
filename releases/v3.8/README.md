# Smart Ropewalk Display Firmware v3.8

Release OTA per display JC3248W535C.

## File

- `firmware-jc3248w535c-v3.8.bin`: firmware applicativo per aggiornamento OTA.
- `firmware-jc3248w535c-v3.8-merged.bin`: immagine completa per flash USB.
- `firmware-jc3248w535c-v3.8-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v3.8-partitions.bin`: tabella partizioni.
- `rigging_db_rev56.csv`: database rigging compatibile per aggiornamento dati su microSD.
- `ships_rev56.csv`: elenco kit/vascelli con tonnellaggio e classe Steel.
- `rigging_classes_rev56.csv`: database completo delle manovre per classe Steel.
- `rigging_deductions_rev56.csv`: tracciamento dei diametri dedotti.
- `diameter_normalization_rev56.csv`: tracciamento delle normalizzazioni numeriche.
- `SHA256SUMS.txt`: checksum SHA256 degli artefatti.

## Note

- Versione firmware impostata a `3.8`.
- Database rigging aggiornabile via Wi-Fi dalla pagina Aggiornamento.
- Il CSV viene salvato sulla microSD in `/rigging/rigging_db.csv`.
- Scelta guidata: prima vascello con ricerca testuale, poi manovra con filtro/sezione/ricerca.
- Correzione: aggiornamento database eseguito dal loop principale, non dal callback touch.
- Database OTA aggiornato a `rev56`; il firmware attuale scarica il solo file compatibile `rigging_db_rev56.csv`.
