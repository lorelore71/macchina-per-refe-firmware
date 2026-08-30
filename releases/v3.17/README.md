# Smart Ropewalk firmware v3.17

Release OTA per display JC3248W535C.

## Novita

- Firmware display portato a 3.17.
- Corretta la lettura della versione reale del database dalla microSD.
- Il firmware non dichiara piu rev57-full se sulla SD e ancora presente un database precedente.
- Database cordame completo rev57 invariato: 214 vascelli e 9450 righe di manovre per classi Steel.
- Buffer manovre allocato in PSRAM.

## File

- firmware-jc3248w535c-v3.17.bin: firmware OTA.
- firmware-jc3248w535c-v3.17-merged.bin: immagine completa per flash via USB.
- rigging_bundle_rev57.csv: pacchetto unico database per aggiornamento su microSD.