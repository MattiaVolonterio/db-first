# Primo DB

## Traccia

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

##

| FIELD                              | TYPE        | ATTRIBUTES                                 | INDEXES     |
| ---------------------------------- | ----------- | ------------------------------------------ | ----------- |
| id                                 | INT         | AUTO_INCREMENT (UNIQUE, NOTNULL, UNSIGNED) | PRIMARY KEY |
| car_brand (Marca)                  | VARCHAR(50) | NOTNULL                                    |             |
| car_model (Modello)                | VARCHAR(50) | NOTNULL                                    |             |
| bodywork (carrozzeria es.berlina)  | VARCHAR(30) | NOTNULL, DEFAULT("city car")               |             |
| fuel (tipo carburante)             | VARCHAR(20) | NOTNULL, DEFAULT("Gasoline")               |             |
| mileage (chilometraggio)           | MEDIUMINT   | NOTNULL                                    |             |
| power (Kw)                         | SMALLINT    | NOTNULL                                    |             |
| gearbox (Tipo di Cambio)           | VARCHAR(20) | NOTNULL, DEFAULT("Manual")                 |             |
| doors_number (Numero di porte)     | TINYINT     | NOTNULL, DEFAULT(5)                        |             |
| seats_number (Numero di posti)     | TINYINT     | NOTNULL, DEFAULT(5)                        |             |
| condition (Condizioni del veicolo) | VARCHAR(50) | NOTNULL, default("Like new")               |             |
| bodywork_colour                    | VARCHAR(20) | NOTNULL                                    |             |
| previous_owners                    | TINYINT     | NOTNULL, DEFAULT(1)                        |             |
| license_plate                      | CHAR(7)     | NOTNULL, UNIQUE                            |             |
| production_year                    | YEAR        | NOTNULL                                    |             |
