# Smart Ropewalk v3.62

Firmware `3.62` per display JC3248W535C con database rigging invariato (`rev70`).

## Correzione manuali PDF

A ogni aggiornamento OTA del firmware il display scarica sempre i tre manuali
PDF in italiano, inglese e spagnolo e sovrascrive i file nella cartella
`/manuale/` della microSD. Non viene eseguito alcun confronto con una revisione
locale del manuale.

Ogni PDF viene scaricato in un file temporaneo, verificato con SHA-256 e poi
sostituito in modo atomico. Un errore nel download di un manuale non annulla il
flash del firmware: il PDF precedente resta disponibile e il tentativo viene
ripetuto al prossimo OTA.

## File

- `firmware-jc3248w535c-v3.62.bin`: aggiornamento OTA del display.
- `firmware-jc3248w535c-v3.62-merged.bin`: immagine completa per installazione USB.
- `Smart-Ropewalk-Manual-*.pdf`: manuali utente distribuiti automaticamente dall'OTA.
