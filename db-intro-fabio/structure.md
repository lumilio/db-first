# Biblioteca

## (Table) books:

- id | BIGINT - PRIMARY KEY, AUTO INCREMENT, UNIQUE, NOTNULL
- isbn | CHAR(13) - NOTNULL, UNIQUE
- titolo | VARCHAR(255) - NOTNULL
- numero_pagine | SMALLINT - NULL
- anno_di_publicazione | YEAR - NULL
- immagine_di_copertina | ('/books/harry_potter_1.jpg') | VARCHAR(255) - NULL
- prezzo | DECIMAL(5,2) -  NULL
- trama | TEXT - NULL
- numero_copie | TINYINT - NOT NULL
- disponibilitá | TINYINT (vero/falso | 1/0) -  DEFAULT(1)
- valutazione | FLOAT(3,1) 99,9 - NULL
- sconto | TINYINT - NULL
- collana | VARCHAR(30) - NULL
- condizione | VARCHAR(20) - NULL
- note | TEXT - NULL

___ DA METTERE ALTROVE ...

- (?) genere (fantasy | coding | giallo) | VARCHAR(20) - NULL
- (?) genere_2 (fantasy | coding | giallo) | VARCHAR(20) - NULL
- (?) autore | VARCHAR(255) - NOT NULL
- (?) editore | VARCHAR(255) - NULL
- (?) reparto | VARCHAR(10) - NULL
- (?) formato | (flessibile, rigido ) VARCHAR(20) - NULL
- (?) fascia_di_eta | (5-10 | 11-20 | 21-99) VARCHAR(5) - NULL
- (?) lingua | VARCHAR(20) - NULL
  