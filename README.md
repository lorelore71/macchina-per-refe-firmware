# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware. Il codice sorgente resta nel repository privato
`macchina-per-refe`.

## Ultima versione

- Versione firmware: `v3.68`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.68/firmware-jc3248w535c-v3.68.bin`
- Immagine USB completa: `releases/v3.68/firmware-jc3248w535c-v3.68-merged.bin`
- Database rigging: `rev70`
- Immagini vascelli OTA: `rev69`
- Manuali PDF: IT/EN/ES aggiornati automaticamente in `/manuale/` durante l'OTA firmware se piu' recenti o mancanti.
- Simulatore Web: aprire nel browser `http://` seguito dall'IP della macchina, sulla stessa rete locale. Non serve scaricare file.
- [ZIP opzionale per PC v3.68](releases/v3.68/Smart-Ropewalk-Web-Display-v3.68.zip), con istruzioni IT/EN/ES. Estrarre tutto e aprire `index.html`.
- [Manuale italiano](releases/v3.68/Smart-Ropewalk-Manual-Italian.pdf), [English manual](releases/v3.68/Smart-Ropewalk-Manual-English.pdf), [Manual en espanol](releases/v3.68/Smart-Ropewalk-Manual-Spanish.pdf).
- Note firmware: [v3.68](releases/v3.68/README.md). Preset con diametro e RH/LH, cancellazione con conferma, elenco senza RPM, Applica alla pagina principale e attesa Web migliorata. Motori, formule, attivazione e database invariati.

Verificato con Edge su Windows e WebKit con profili iPad. iPadOS 15 o successivo
e' il requisito obiettivo: non e' stata effettuata una prova su iPad fisico.
Chiudere il browser o perdere la connessione non ferma i motori.

## Aggiornamento immagini rev69

- il pacchetto immagini e' indipendente da firmware e database;
- il display confronta gli SHA-256 e scarica solo gli sfondi mancanti o
  modificati sulla microSD;
- avviare la funzione **AGG. DATI** dalla pagina Aggiornamento del display.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```
