# Smart Ropewalk v3.61

Firmware `3.61` per display JC3248W535C con database rigging invariato (`rev70`).

## Novita'

Durante ogni aggiornamento OTA del firmware, il display scarica anche i tre
manuali PDF in italiano, inglese e spagnolo sulla microSD. Ogni PDF viene
scaricato in un file temporaneo, verificato con SHA-256 e poi sostituito nella
cartella `/manuale/`.

Un errore nel download di un manuale non annulla il flash del firmware: resta
disponibile il PDF precedente e il tentativo viene ripetuto al prossimo OTA.

## File

- `firmware-jc3248w535c-v3.61.bin`: aggiornamento OTA del display.
- `firmware-jc3248w535c-v3.61-merged.bin`: immagine completa per installazione USB.
- `Smart-Ropewalk-Manual-*.pdf`: manuali utente distribuiti automaticamente dall'OTA.
