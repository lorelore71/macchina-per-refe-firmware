# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware. Il codice sorgente resta nel repository privato
`macchina-per-refe`.

## Ultima versione

- Versione firmware: `v3.70`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.70/firmware-jc3248w535c-v3.70.bin`
- Immagine USB completa: `releases/v3.70/firmware-jc3248w535c-v3.70-merged.bin`
- Database rigging: `rev72`, 359 kit e 13.421 manovre.
- Immagini vascelli OTA: `rev71`, 225 sfondi, Diana britannica e spagnola distinte.
- [Novita' database rev72](releases/rigging-rev72/README.md), [ZIP dati](releases/rigging-rev72/Smart-Ropewalk-Rigging-rev72.zip) e [changelog database](CHANGELOG_DATABASE_RIGGING.md).
- Manuali PDF: IT/EN/ES aggiornati automaticamente in `/manuale/` durante l'OTA firmware se piu' recenti o mancanti.
- Simulatore Web: aprire nel browser `http://` seguito dall'IP della macchina, sulla stessa rete locale. Non serve scaricare file.
- [ZIP opzionale per PC v3.70](releases/v3.70/Smart-Ropewalk-Web-Display-v3.70.zip), con istruzioni IT/EN/ES. Estrarre tutto e aprire `index.html`.
- [Manuale italiano](releases/v3.70/Smart-Ropewalk-Manual-Italian.pdf), [English manual](releases/v3.70/Smart-Ropewalk-Manual-English.pdf), [Manual en espanol](releases/v3.70/Smart-Ropewalk-Manual-Spanish.pdf).
- Note firmware: [v3.70](releases/v3.70/README.md). Nel calcolo refe l'input si chiama Diametro richiesto, distinto dal risultato Ottenibile. Etichetta aggiornata nelle tre lingue; formule, motori e database invariati.

Verificato con Edge su Windows e WebKit con profili iPad. iPadOS 15 o successivo
e' il requisito obiettivo: non e' stata effettuata una prova su iPad fisico.
Chiudere il browser o perdere la connessione non ferma i motori.

## Aggiornamento database rev72 e immagini rev71

- usare **AGG. DATI** sulla macchina: il firmware 3.70 resta invariato e non va reinstallato;
- aggiunti 13 kit per vascelli gia presenti e 13 nuovi vascelli, inclusa Norske Love;
- preparati 13 sfondi nuovi e corretta la foto di HMS Diana, distinta dalla Diana spagnola;
- le manovre Steel precedenti sono invariate; i diametri non disponibili restano n.d.;

- il pacchetto immagini e' indipendente da firmware e database;
- il display confronta gli SHA-256 e scarica solo gli sfondi mancanti o
  modificati sulla microSD;
- avviare la funzione **AGG. DATI** dalla pagina Aggiornamento del display.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```
