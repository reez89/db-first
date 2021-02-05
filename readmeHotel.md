<!-- Istruzioni:
Provare a strutturare il seguente database che modellizza un hotel: Ci sono varie stanze, ognuna con le proprie caratteristiche. Le diverse stanze vengono prenotate per periodi di tempo, da ospiti. Ad ogni prenotazione devono essere associati tutti gli ospiti della stanza.
Nella repo mettete sia il file del diagramma che il file esportato come immagine.
Buon lavoro e buon weekend! -->


# database name : Hotel Motel Holiday Inn
# nome tabella : Utente

- Nome string TEXT(1500) NOTNULL
- Cognome string TEXT(1500) NOTNULL
- Data di nascita int SMALLINT NOTNULL
- Luogo di nascita string VARCHAR(15) NOTNULL
- Indirizzo string TEXT(1500) NOTNULL
- Cap int SMALLINT NOTNULL 
- Email string TEXT(1500) NOTNULL
- Numero di prenotazione int SMALLINT NOTNULL DEFAULT(0)

# nome tabella : Documento
- Tipo di documento string VARCHAR(15) NOTNULL
- Numero documento  string VARCHAR(15) NOTNULL
- Id Utente int SMALLINT NOTNULL

# nome tabella : Soggiorno
- Id utente int SMALLINT NOTNULL
- Durata del soggiorno int SMALLINT NOTNULL
- Tipo di Camera string VARCHAR(15) NOTNULL
- Id numero Camera int SMALLINT NOTNULL

# nome tabella : Camere
- Id camera singola int SMALLINT NOTNULL
- id camera doppia int SMALLINT NOTNULL
- Id camera doppia letti singoli
- Id camera doppia letti separati
- id camera doppia matrimoniale
- id camera suite int SMALLINT NOTNULL

# nome tabella : Extra
- Parcheggio string VARCHAR(15) NOTNULL
- Extra Letto string VARCHAR(15) NOTNULL
- Cancellazione no preavviso string VARCHAR(2) NOTNULL
- Pensione Completa string VARCHAR(2) NOTNULL

# nome tabella : Fatturazione
- Id Fattura int SMALLINT NOTNULL
- Id Soggiorno int SMALLINT NOTNULL
- Id Camere int SMALLINT NOTNULL
- Id Extra string VARCHAR(15) NOTNULL DEFAULT(0)
- Id tipo di pagamento string VARCHAR(15) NOTNULL
- Id consumazione frigo bar  int SMALLINT NULL DEFAULT(0)