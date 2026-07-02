# Macchina per refe - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare gli aggiornamenti firmware.

Il codice sorgente resta nel repository privato `macchina-per-refe`.

## Ultima versione

- Versione: `v2.1`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v2.1/firmware-jc3248w535c-v2.1.bin`
- Immagine USB completa: `releases/v2.1/firmware-jc3248w535c-v2.1-merged.bin`

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```

## Installazione USB completa

```powershell
python -m esptool --chip esp32s3 --port COM5 --baud 921600 write_flash 0x0 releases/v2.1/firmware-jc3248w535c-v2.1-merged.bin
```

## OTA

Il file applicativo per OTA e':

```text
releases/v2.1/firmware-jc3248w535c-v2.1.bin
```
