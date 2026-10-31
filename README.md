# Smart Ropewalk - firmware pubblico

Repository pubblico usato dal display JC3248W535C per verificare e scaricare
gli aggiornamenti firmware. Il codice sorgente resta nel repository privato
`macchina-per-refe`.

## Ultima versione

- Versione firmware: `v3.69`
- Manifest: `releases/latest.json`
- Firmware OTA: `releases/v3.69/firmware-jc3248w535c-v3.69.bin`
- Immagine USB completa: `releases/v3.69/firmware-jc3248w535c-v3.69-merged.bin`
- Database rigging: `rev71`, 333 kit e 13.421 manovre.
- Immagini vascelli OTA: `rev70`, aggiunto Redoutable.
- [Novita' database rev71](releases/rigging-rev71/README.md), [ZIP dati](releases/rigging-rev71/Smart-Ropewalk-Rigging-rev71.zip) e [changelog database](CHANGELOG_DATABASE_RIGGING.md).
- Manuali PDF: IT/EN/ES aggiornati automaticamente in `/manuale/` durante l'OTA firmware se piu' recenti o mancanti.
- Simulatore Web: aprire nel browser `http://` seguito dall'IP della macchina, sulla stessa rete locale. Non serve scaricare file.
- [ZIP opzionale per PC v3.69](releases/v3.69/Smart-Ropewalk-Web-Display-v3.69.zip), con istruzioni IT/EN/ES. Estrarre tutto e aprire `index.html`.
- [Manuale italiano](releases/v3.69/Smart-Ropewalk-Manual-Italian.pdf), [English manual](releases/v3.69/Smart-Ropewalk-Manual-English.pdf), [Manual en espanol](releases/v3.69/Smart-Ropewalk-Manual-Spanish.pdf).
- Note firmware: [v3.69](releases/v3.69/README.md). Marca del kit nell'elenco vascelli, classe e scala a destra; cinque righe manovre piu' alte per descrizioni su due righe. Manuali aggiornati. Motori, formule, attivazione e database invariati.

Verificato con Edge su Windows e WebKit con profili iPad. iPadOS 15 o successivo
e' il requisito obiettivo: non e' stata effettuata una prova su iPad fisico.
Chiudere il browser o perdere la connessione non ferma i motori.

## Aggiornamento database rev71 e immagini rev70

- usare **AGG. DATI** sulla macchina: il firmware 3.68 e' gia' compatibile e non va reinstallato;
- aggiunte 249 manovre dedicate al Vespucci, marcate come stime modellistiche, e sette varianti di kit/scala;
- aggiunto Redoutable Artesania Latina 1:84 e relativo sfondo;
- le manovre Steel precedenti sono invariate; i diametri non disponibili restano n.d.;

- il pacchetto immagini e' indipendente da firmware e database;
- il display confronta gli SHA-256 e scarica solo gli sfondi mancanti o
  modificati sulla microSD;
- avviare la funzione **AGG. DATI** dalla pagina Aggiornamento del display.

## URL usato dal display

```text
https://raw.githubusercontent.com/lorelore71/macchina-per-refe-firmware/main/releases/latest.json
```
