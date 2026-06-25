# Macchina per refe - firmware OTA

Repository pubblico destinato esclusivamente alle release firmware OTA firmate
della Macchina per refe.

## Stato attuale

La release `v1.9` e' pubblicata solo per verificare il flusso OTA nel simulatore
HTML. Non contiene un firmware installabile sul display JC3248W535C.

Il dispositivo reale deve accettare una release soltanto quando sono presenti:

- `firmware-jc3248w535c.bin`
- `firmware-jc3248w535c.bin.sig`
- `firmware-jc3248w535c.bin.sha256`

Il codice sorgente resta nel repository privato del progetto.
