# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware.

Il codice sorgente resta nel repository privato `macchina-per-refe`.

## Ultima versione

- Versione: `v3.58`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.58/firmware-jc3248w535c-v3.58.bin`
- Immagine USB completa: `releases/v3.58/firmware-jc3248w535c-v3.58-merged.bin`
- Database rigging: `rev68`

## Novita v3.58

- il comando **AGG. DATI** confronta database e immagini vascelli in modo
  indipendente;
- vengono scaricati solo i CSV o gli sfondi assenti, senza un ordine obbligato
  tra aggiornamento firmware, database e immagini;
- ogni JPEG viene verificato con SHA-256 e la revisione immagini viene salvata
  sulla microSD soltanto dopo un trasferimento completo;
- database `rev68` con 9.429 manovre con diametro Steel disponibile, incluse
  cinque formule circonferenza-diametro prima mancanti;
- mapping motori e licenze invariati rispetto a 3.57.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```

## OTA

Il file applicativo per OTA e':

```text
releases/v3.58/firmware-jc3248w535c-v3.58.bin
```
