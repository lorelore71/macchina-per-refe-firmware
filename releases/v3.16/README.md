# Smart Ropewalk firmware v3.16

Release OTA per display JC3248W535C.

## Novita

- Firmware display portato a 3.16.
- Database cordame completo rev57 generato da Steel_1794_Cordame_DATABASE_COMPLETO.xlsx.
- Pubblicati 214 vascelli e 9450 righe di manovre per classi Steel.
- Colonna Voce completa ES inclusa nel CSV; dove vuota resta il fallback IT/EN.
- Buffer manovre allocato in PSRAM, per non sottrarre RAM interna a LVGL.

## File

- firmware-jc3248w535c-v3.16.bin: firmware OTA.
- firmware-jc3248w535c-v3.16-merged.bin: immagine completa per flash via USB.
- rigging_bundle_rev57.csv: pacchetto unico database per aggiornamento su microSD.
- ships_rev57.csv: elenco vascelli.
- rigging_classes_rev57.csv: database manovre per classi Steel.