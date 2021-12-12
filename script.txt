


1) NOME DELLA COLONNA : Chiaro e immediatamente comprensibile Future-proof

2) RAPPRESENTAZIONE DEL DATO DA INSERIRE : Es. una data di nascita (17-02-1988, 17th Feb 88, ...)

3) TIPO DI DATO : Con cui il database gestirà l’informazione

4) ATTRIBUTI



////////////////   TIPO DI DATI  /////////////////
 
 
--------------- Numeri interi ---------------

    TINYINT
        Utilizza solo un byte per salvare numeri che vanno da -128 a 127.
        Viene utilizzato ad esempio per salvare i valori boolean, proprio
        perché è il tipo di dato più piccolo possibile


    SMALL / MEDIUMINT
        Occupano rispettivamente 2 e 3 bytes

    INT
        Utilizza 4 bytes per rappresentare numeri compresi tra
        -2.147.483.648 e 2.147.483.647

    BIGINT
        Corrisponde ad un INT con il doppio di bytes disponibili
        Numeri interi


Numeri con la virgola

    FLOAT(I, D)
        un numero con la virgola da 4 bytes

    DOUBLE(I, D)
        un numero con la virgola da 8 bytes

    DECIMAL(I, D)
        un double che gestisce gli
        arrotondamenti considerando i numeri
        dal punto di vista finanziario



--------------- Stringhe ---------------

    VARCHAR(numero)
        permette di indicare la lunghezza massima della stringa da
        rappresentare, con il limite di 255 caratteri

    TEXT
        fino a 65535 caratteri - è usato ad esempio per le descrizioni prodotto

    MEDIUMTEXT
        16mb

    LONGTEXT
        4.2gb - usato per salvare porzioni di HTML o lunghi testi



--------------- Date ---------------

    DATETIME
        permette di memorizzare data e ora (YYYY-MM-GG HH:II:SS)

    DATE
        contiene solo la data (YYYY-MM-GG)

    TIME
        contiene solo l’orario (HH:II:SS)

    YEAR
        contiene solo l’anno (YYYY)

    TIMESTAMP
        può avere diversi formati




////////////////   ATTRIBUTI  /////////////////


    NULL / NOTNULL
        indica che la colonna può o non può contenere il valore NULL.
        Se una colonna è NOT NULL e durante il salvataggio non viene passato alcun valore per quella colonna,
        verrà restituito un errore e l'intera riga non verrà inserita.

        Esempio:
        In un database di un'anagrafe, la colonna data_di_nascita sarà NOT NULL per indicare che non è possibile salvare nel
        database di una persona senza indicare anche la data di nascita


    DEFAULT
        permette di settare un valore di default alla colonna qualora non fosse presente alcun valore al
        momento del salvataggio.

        Esempio:
        Se vogliamo contare il numero di volte in cui un prodotto è stato acquistato, può avere senso avere DEFAULT(0)
        Ad ogni colonna, possiamo assegnare degli attributi


    AUTO_INCREMENT
        Il valore della colonna è incrementa ad ogni nuovo record, per questo motivo è utilizzabile solo con le
        colonne di tipo numero.
        Viene utilizzato ad esempio per gli ID: ogni volta che si aggiunge una nuova riga, in automatico l’ID sarà
        +1 rispetto alla riga precedente.


    UNIQUE
        Indica che i valori di quella colonna devono essere unici, ossia non ci può essere alcun valore ripetuto
        all'interno della colonna.