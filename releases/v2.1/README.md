# Firmware v2.1 - JC3248W535C

Release firmware per display `JC3248W535C` / ESP32-S3.

## File

- `firmware-jc3248w535c-v2.1.bin`: firmware applicativo, da usare per upload OTA.
- `firmware-jc3248w535c-v2.1-merged.bin`: immagine completa flash, da usare via USB a indirizzo `0x0`.
- `firmware-jc3248w535c-v2.1-bootloader.bin`: bootloader.
- `firmware-jc3248w535c-v2.1-partitions.bin`: tabella partizioni `huge_app`.
- `SHA256SUMS.txt`: checksum dei binari.

## Installazione USB completa

Usare l'immagine merged:

```powershell
python -m esptool --chip esp32s3 --port COM5 --baud 921600 write_flash 0x0 firmware-jc3248w535c-v2.1-merged.bin
```

## Installazione OTA

La scheda deve essere gia collegata al Wi-Fi e la pagina `Aggiornamento` deve indicare `OTA pronto`.

Hostname OTA:

```text
macchina-refe
```

File da caricare via OTA:

```text
firmware-jc3248w535c-v2.1.bin
```

## Impostazioni build

- FQBN: `esp32:esp32:esp32s3`
- Flash: `8M`
- PSRAM: `opi`
- Flash mode: `qio`
- USB: `hwcdc`
- CDC on boot: `cdc`
- Partition scheme: `huge_app`
