# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware. Il codice sorgente resta nel repository privato
`macchina-per-refe`.

## Ultima versione

- Versione firmware: `v3.60`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.60/firmware-jc3248w535c-v3.60.bin`
- Immagine USB completa: `releases/v3.60/firmware-jc3248w535c-v3.60-merged.bin`
- Database rigging: `rev70`
- Immagini vascelli OTA: `rev68` (`210` JPEG)

## Aggiornamento immagini rev68

- il pacchetto immagini è indipendente da firmware e database;
- il display confronta gli SHA-256 e scarica solo gli sfondi mancanti o
  modificati sulla microSD;
- avviare la funzione **AGG. DATI** dalla pagina Aggiornamento del display.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```
