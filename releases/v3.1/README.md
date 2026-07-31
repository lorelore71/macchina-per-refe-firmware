# Firmware v3.1

Release OTA per display JC3248W535C.

## Modifiche

- Motori gestiti con FastAccelStepper su driver RMT selezionato automaticamente.
- ENABLE DRV8825 gestito manualmente come nel banco prova validato.
- STOP motore reso affidabile con reset immediato dello stato FastAccelStepper.
- AUTO corretto: lo stop avviene al raggiungimento del valore assoluto dei giri target, indipendentemente dal verso.

## Motori

Mappa GPIO congelata sul cablaggio reale:

```text
M1 STEP   GPIO5
M1 DIR    GPIO6
M1 EN     GPIO7
M2 STEP   GPIO15
M2 DIR    GPIO16
M2 EN     GPIO17
```

## File

- `firmware-jc3248w535c-v3.1.bin`: binario OTA.
- `firmware-jc3248w535c-v3.1-merged.bin`: immagine completa flash.
- `SHA256SUMS.txt`: checksum dei binari.
