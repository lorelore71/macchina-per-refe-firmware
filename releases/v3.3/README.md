# Firmware v3.3

Release OTA per display JC3248W535C.

## Modifiche

- Firmware display portato a `3.3`.
- Preset 1 caricato di default all'avvio, con priorita' al file microSD `/recipes/p1.txt`.
- UI Main rifinita: icona Wi-Fi con stato connesso/non connesso e nome preset completo.
- Help aggiornata con layout e icone coerenti con la Main.
- Comandi manuali ripuliti graficamente e aggiornati con dati live di step, giri e RPM.
- Limite massimo RPM rimosso dai comandi utente, mantenendo il limite tecnico `9999`.

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

- `firmware-jc3248w535c-v3.3.bin`: binario OTA.
- `firmware-jc3248w535c-v3.3-merged.bin`: immagine completa flash.
- `SHA256SUMS.txt`: checksum dei binari.
