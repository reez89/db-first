Istruzioni:
Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato.


# database name : GameStop
# nome tabella : Video games Consolle

- id BIGINT PRIMARYKEY NOTNULL AUTO_INCREMENT
- isbn string VARCHAR(10) NOTNULL UNIQUE
- title string TEXT(1500) NOTNULL
- description string TEXT NULL
- author string VARCHAR(30) NOTNULL
- year release date YEAR NOTNULL
- genre string VARCHAR(15) NOTNULL
- price int FLOAT(6,2) 9999,99 NULL
- availability int TINYINT NULL DEFAULT(1)
- cover_img string VARCHAR() NULL
- language string VARCHAR(20) NOTNULL
- edition string VARCHAR(20) NULL
- quantity int SMALLINT NULL DEFAULT(0)
- size string VARCHAR (25) NULL
- editor string VARCHAR(25) NULL
- format type string VARCHAR(25) NULL
- created_at_date date DATETIME NOTNULL
- edited_in date DATETIME NULL


