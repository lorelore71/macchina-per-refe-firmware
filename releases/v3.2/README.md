# Firmware v3.2

Release OTA per display JC3248W535C.

## Modifiche

- Firmware display portato a `3.2`.
- Editor preset aggiornato: i campi numerici aprono il tastierino numerico.
- Nome preset modificabile dal titolo con tastierino alfanumerico.
- Rapporto preset preservato al salvataggio, senza sovrascrittura automatica del calcolo.
- UI Display aggiornata con splash nave, bandiere lingua, sfondo pagina e icone correnti.
- Preset salvati anche su microSD in `/recipes`, mantenendo Preferences come fallback.

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

- `firmware-jc3248w535c-v3.2.bin`: binario OTA.
- `firmware-jc3248w535c-v3.2-merged.bin`: immagine completa flash.
- `SHA256SUMS.txt`: checksum dei binari.
