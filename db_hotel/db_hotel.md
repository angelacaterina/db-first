# Hotel 
## Ricreare database hotel come da diagramma
Prendere il diagramma e usando phpmyadmin ricreare il database, 
inserire dei dati a piacere per poter effettuare le seguenti ricerche
## Ricerche da effettuare sul database
- selezionare tutti gli ospiti
    SELECT `id_guests`, `name`,`lastname` FROM `guests`

- selezionare tutti gli ospiti che sono stati identificati con la carta di identitá
    SELECT `name`, `type_of_document` FROM `guests` WHERE `type_of_document` = 'carta_identità'

- selezionare tutte le stanze del primo piano
    SELECT `name` FROM `rooms` WHERE `floor` = 1

- selezionare tutti gli ospiti che iniziano per E (vedi uso del Like)
    SELECT `id_guests`, `name`,`lastname` FROM `guests` WHERE `name` LIKE 'e%' 

- Selezionare tutti gli ospiti che abbiano almeno 30 anni
    SELECT `name`, `date_of_birth` FROM `guests` WHERE `date_of_birth` < '1991-02-08'

- selezionare tutte le prenotazioni precedenti ad una data a piacere
    SELECT `id_booking`, `id_room`, `check_in` FROM `booking` WHERE `check_in` < '2021-01-01'

## Altre ricerche (opzionali)
- seleziona tutti gli ospiti nati dopo una certa data
    SELECT `name`, `date_of_birth` FROM `guests` WHERE `date_of_birth` > '1990-01-01'

- calcola il totale degli ordini ricevuti
- calcola il prezzo massimo pagato
- calcola quanti posti letto ha l'hotel in totale