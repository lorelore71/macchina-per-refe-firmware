# Changelog database rigging

## rev72 - Catalogo kit e sfondi - 2026-11-01

- Pubblicati database rev72 e immagini rev71 per firmware 3.70 invariato.
  Aggiornamento dal comando AGG. DATI; nessuna reinstallazione firmware.

- Dopo la scelta di Lorenzo aggiunti anche 13 vascelli nuovi, inclusa Norske
  Love: totale 359 kit. Cinque modelli esclusi lasciati fuori dal catalogo.
- Preparati 13 sfondi nuovi e corretta l'associazione di HMS Diana:
  originali britannico e spagnolo distinti, nomi SD senza collisioni.
- Manifesto immagini locale rev71: 225 sfondi, 14 file nuovi/modificati.
- CSV distribuiti via OTA; tavole manovre identiche alla rev71. Classi
  Steel non verificate mantenute n.d.; Le Superbe assegnato a 74 guns.

- Prima fase: aggiunti 13 kit di vascelli gia presenti, da 333 a 346 kit.
- Varianti Mantua/Sergal, OcCre, Artesania Latina, Amati, CAF Model e
  Model Shipways; scale e fonti commerciali registrate nel catalogo.
- Dati storici e classi ereditati dalle voci esistenti, senza nuove stime.
  Nessuna modifica alle manovre, formule, immagini o ai kit gia registrati.
- L'Excel separato conserva le decisioni di Lorenzo sui 18 candidati:
  13 inseriti e cinque esclusi. Online rev72, firmware 3.70 invariato.

Questo documento registra le revisioni distribuibili del database storico
Steel. E' distinto dal changelog del firmware: il database puo' essere
aggiornato dalla microSD o via OTA senza cambiare il programma del display.

## Regole dei dati

- Il database conserva il dato storico disponibile nelle tavole di David
  Steel, la classe Steel, la descrizione della manovra e il verso RH/LH.
- Il diametro viene ricavato dalla circonferenza Steel solo quando quella
  circonferenza e' presente nella fonte: `diametro mm = circonferenza in x
  25,4 / pi`.
- Un campo `n.d.` significa che nel record sorgente non e' disponibile un
  diametro ne' una circonferenza utilizzabile. Non e' uno zero e non e' una
  stima.
- Le manovre `n.d.` restano ricercabili e consultabili, ma non possono essere
  trasferite al calcolatore della Smart Ropewalk.

## rev71 - 2026-10-31

- 333 kit commerciali e 13.421 manovre complessive: 9.642 con diametro e
  3.779 con diametro `n.d.`. Le 13.172 righe Steel della rev70 sono invariate.
- Aggiunta una tabella dedicata `Vespucci`, con 249 manovre (213 con diametro,
  36 senza). Non e' una classe Steel e non contiene misure verificate della
  nave: i valori sono stime/analogie modellistiche, indicate nei nomi nelle
  tre lingue per renderle riconoscibili anche sul firmware 3.68.
- Completati 83 versi mancanti per analogia con singole manovre `74 guns`:
  68 RH e 15 LH; nelle note sono conservati riferimento e limiti del confronto.
  Totale tabella Vespucci: 232 RH e 17 LH. Diametri non modificati.
- Sette kit Vespucci: OcCre 1:100, Mantua/Panart 1:84, Mantua 1:100,
  Hachette 1:100, Heller 1:150, Mamoli 1:150 e MiniMamoli 1:350.
- Aggiunto Redoutable Artesania Latina 1:84, kit 22907, con classe `74 guns`
  per analogia e nuovo sfondo 480x320. Immagini OTA rev70: 212 file nel
  manifesto, con URL e hash precedenti conservati per tutti gli altri sfondi.
- Compatibile con firmware 3.68 senza ricompilazione o nuovo flash. Aggiornare
  mediante AGG. DATI; ordine indipendente rispetto all'aggiornamento firmware.
- Sorgente rinominato `Database rigging rev71.xlsx`; eliminati i vecchi
  database Excel su richiesta di Lorenzo. Nessuna modifica al normalizzatore
  dei diametri, alle ricette o ai dati sperimentali.

## Immagini vascelli rev68 - 2026-10-19

- Pubblicato un manifesto di sincronizzazione completo con `210` sfondi JPEG
  elaborati per il display.
- La revisione immagini e' indipendente dal database rigging `rev70` e dal
  firmware `3.60`.
- Durante l'aggiornamento OTA il display confronta lo SHA-256 di ogni file e
  scarica soltanto gli sfondi assenti o differenti sulla microSD.

## rev70 - 2026-10-19

- Normalizzate tutte le scale commerciali espresse in pollici/piede nel
  formato standard `1:N`.
- Completate le scale disponibili per i kit senza classe Steel, mantenendo
  la classe `n.d.` quando non esiste un collegamento verificabile alle tavole.
- Ogni scala verificata riporta la propria fonte nel commento della cella del
  workbook sorgente.

## rev69 - 2026-10-17

- Include tutte le `13.172` righe di manovre estratte dalle tavole Steel.
- `9.429` righe riportano un diametro storico disponibile.
- `3.743` righe senza circonferenza o diametro restano nel database con
  valore `n.d.`.
- Nessuna lacuna e' stata colmata per interpolazione, media o stima da classi
  vicine.
- Corregge il comportamento delle revisioni precedenti, che omettevano tali
  righe nel CSV distribuito.

## rev68 - 2026-10-17

- Database distribuito con `9.429` manovre dotate di diametro Steel.
- Aggiunti cinque diametri ricavati dalle rispettive circonferenze presenti
  nella fonte, quando la cella del diametro Excel non aveva un valore salvato.
- Le righe senza dato utile venivano ancora omesse dal pacchetto distribuito.

## rev67 - 2026-10-17

- Contenuto testuale equivalente a `rev66`.
- Introdotto il pacchetto immagini OTA associato ai vascelli: Belem, Gjoa,
  HMS Terror e Hermione La Fayette.

## rev66 - 2026-10-14

- Aggiunti e verificati kit OcCre e Artesania Latina, inclusi Gjoa, HMS
  Terror, Hermione La Fayette e Belem.
- Aggiornati anche HMAV Bounty, San Giovanni Battista e Soleil Royal nel
  catalogo dei kit.

## rev65 - 2026-10-14

- Rigenerato il pacchetto classi Steel dal workbook aggiornato.
- Aggiunti cinque vascelli al catalogo dei kit.
- Il log storico non conserva un dettaglio affidabile riga per riga: questa
  nota riporta solo quanto verificabile dal commit della revisione.

## rev64 - 2026-10-11

- Revisione di allineamento del pacchetto rigging predisposto per la
  microSD, associata alla release firmware 3.55.
- Non e' disponibile una nota storica sufficientemente dettagliata per
  attribuire ulteriori variazioni al solo database.

## rev63 - 2026-09-26

- Revisione tecnica del numero di versione del database su microSD e OTA,
  per evitare che il display proponesse ripetutamente un pacchetto gia'
  installato.

## rev61 - 2026-09-22

- Aggiunte scala commerciale e classe Steel ai kit selezionabili.
- La scala commerciale viene proposta come valore iniziale quando si sceglie
  il vascello.

## rev60-full - 2026-09

- Aggiunto il verso storico di chiusura per ogni manovra: corda RH o cavo LH.

## rev59-full - 2026-09

- Database completo rigenerato dal workbook storico aggiornato.

## rev58-full - 2026-09

- Popolate le descrizioni spagnole delle manovre e distribuito il database
  completo usato dalle prime pagine di ricerca rigging.

## rev57-full - 2026-09

- Primo pacchetto Steel completo per la selezione vascello/manovre, con
  catalogo kit e circa 9.450 manovre allora dotate di diametro utilizzabile.

## rev56 - 2026-09

- Prima base dati OTA usata dal firmware per collegare vascello, classe Steel,
  manovra e diametro in scala.
