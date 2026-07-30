# Firmware v3.0

Release OTA per display JC3248W535C.

## Modifiche

- Uscite motori abilitate per prova fisica.
- Versione firmware portata a 3.0.
- Simulatore aggiornato a v3.0.
- Documentazione aggiornata con comportamento reale del pin ENABLE.

## Motori

Con `MOTOR_OUTPUTS_ENABLED = true` e `ENABLE_ACTIVE_LOW = true`:

- START abilita il driver selezionato portando `EN` a GND.
- STOP disabilita i driver portando `EN` alto.
- RESET azzera i contatori senza cambiare da solo la logica di abilitazione oltre allo stato macchina.

Mappa GPIO:

```text
M1 STEP   GPIO5
M1 DIR    GPIO6
M1 EN     GPIO7
M2 STEP   GPIO15
M2 DIR    GPIO16
M2 EN     GPIO17
```

## File

- `firmware-jc3248w535c-v3.0.bin`: binario OTA.
- `firmware-jc3248w535c-v3.0-merged.bin`: immagine completa flash.
- `SHA256SUMS.txt`: checksum dei binari.
