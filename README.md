# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware.

Il codice sorgente resta nel repository privato `macchina-per-refe`.

## Ultima versione

- Versione: `v3.59`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.59/firmware-jc3248w535c-v3.59.bin`
- Immagine USB completa: `releases/v3.59/firmware-jc3248w535c-v3.59-merged.bin`
- Database rigging: `rev69`

## Novita v3.59

- database `rev69` con tutte le 13.172 manovre estratte dalle tavole Steel;
- 9.429 manovre con diametro storico disponibile e 3.743 righe senza dato
  storico mantenute come `n.d.`, senza stime;
- le righe `n.d.` restano consultabili nel display ma non applicabili alla
  ricetta;
- immagini vascelli `rev67` e mapping motori invariati.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```

## OTA

Il file applicativo per OTA e':

```text
releases/v3.59/firmware-jc3248w535c-v3.59.bin
```
