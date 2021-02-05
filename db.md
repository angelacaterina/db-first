<!-- Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato. -->
# database name: Video Game Store
# nome tabelle: Video Games
- id INT PRIMARYKEY NOTNULL AUTO_INCREMENT UNIQUE
- codice_articolo           number      INT                 UNIQUE
- titolo                    string      VARCHAR(50)         NOTNULL
- descrizione               string      TEXT                NULL
- sviluppatore              string      VARCHAR(30)         NULL
- genere                    string      VARCHAR(20)         NOTNULL
- pegi_età                  number      SMALL               NULL
- data_rilascio             data        DATE                NOTNULL
- contenuti_aggiuntivi_DLC  string      TEXT                NULL
- piattaforma               string      VARCHAR(20)         NOTNULL
- disponibilità             number      TINYIT              NULL DEFAULT(0) 
- immagine-copertina        string      VARCHAR(250)        NULL
- lingua                    string      VARCHAR(30)         NOTNULL
- sottotitoli               string      VARCHAR(30)         NULL
- prezzo                    number      LOAT(6,2) 9999,99   NULL


<!-- ATTRIBUTI: 
    NOTNULL : campo obbligatorio 
    NULL : campo non obbligatorio
    DEFAULT : permette settare un valore di default alla colonna qualora non fosse presente alcun valore al momento del salvataggio

    AUTO_INCREMENT : incrementa ad ogni nuovo record.
    UNIQUE: indica che i valori di quella colonna devono essere unici
-->









