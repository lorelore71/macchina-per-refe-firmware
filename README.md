# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware. Il codice sorgente resta nel repository privato
`macchina-per-refe`.

## Ultima versione

- Versione firmware: `v3.66`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.66/firmware-jc3248w535c-v3.66.bin`
- Immagine USB completa: `releases/v3.66/firmware-jc3248w535c-v3.66-merged.bin`
- Database rigging: `rev70`
- Immagini vascelli OTA: `rev69`
- Manuali PDF: IT/EN/ES aggiornati automaticamente in `/manuale/` durante l'OTA firmware se piu' recenti o mancanti.
- Simulatore Web: [pacchetto ZIP v3.66](releases/v3.66/Smart-Ropewalk-Web-Display-v3.66.zip), con istruzioni IT/EN/ES. Estrarre tutto e aprire `index.html`.
- Note firmware: [v3.66](releases/v3.66/README.md). Le ricette salvate vengono preservate anche se manca il marcatore dello schema.

## Aggiornamento immagini rev69

- il pacchetto immagini e' indipendente da firmware e database;
- il display confronta gli SHA-256 e scarica solo gli sfondi mancanti o
  modificati sulla microSD;
- avviare la funzione **AGG. DATI** dalla pagina Aggiornamento del display.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```
