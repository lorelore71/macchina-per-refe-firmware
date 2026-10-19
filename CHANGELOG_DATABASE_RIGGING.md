# Changelog database rigging

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
