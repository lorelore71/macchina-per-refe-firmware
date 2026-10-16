# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare gli aggiornamenti firmware.

Il codice sorgente resta nel repository privato `macchina-per-refe`.

## Ultima versione

- Versione: `v3.57`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.57/firmware-jc3248w535c-v3.57.bin`
- Immagine USB completa: `releases/v3.57/firmware-jc3248w535c-v3.57-merged.bin`
- Database rigging: `rev67`

## Novita v3.57

- il comando **AGG. DB** aggiorna il database e gli sfondi vascello collegati alla revisione dati;
- gli sfondi vengono scaricati solo se assenti o modificati e verificati con SHA-256;
- il delta iniziale include Belem, Gjoa, HMS Terror e Hermione La Fayette;
- firmware, mapping dei motori e licenze restano invariati rispetto a 3.56.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```

## OTA

Il file applicativo per OTA e':

```text
releases/v3.57/firmware-jc3248w535c-v3.57.bin
```
