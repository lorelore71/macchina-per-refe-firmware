# Firmware v2.4 - JC3248W535C

Calcolatore empirico banco prova e pausa/ripresa AUTO senza azzerare i contatori.

## Ricette empiriche naturali

- 3 trefoli, diametro 0.22 mm, L180, 150g: 966 torsioni, 900 avvolgimenti.
- 6 trefoli, diametro 0.22 mm, L180, 150g: 876 torsioni, 600 avvolgimenti.
- Cotone, lino, lana e seta trattati come cotone.
- Scala lineare per lunghezza e fattore diametro 0.22 / diametro.
- 2/4/5 trefoli: interpolazione non standard.

## File

- firmware-jc3248w535c-v2.4.bin: firmware applicativo OTA.
- firmware-jc3248w535c-v2.4-merged.bin: immagine completa USB a indirizzo 0x0.
- SHA256SUMS.txt: checksum dei binari.

## Partizioni

Build compilata con PartitionScheme=default_8MB per supporto OTA app0/app1.
