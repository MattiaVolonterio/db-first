# Primo DB

## Traccia

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

##

| FIELD           | TYPE        | ATTRIBUTES                                 | INDEXES     |
| --------------- | ----------- | ------------------------------------------ | ----------- |
| id              | INT         | AUTO_INCREMENT (UNIQUE, NOTNULL, UNSIGNED) | PRIMARY KEY |
| car_brand       | VARCHAR(50) | NOTNULL                                    |             |
| car_model       | VARCHAR(50) | NOTNULL                                    |             |
| bodywork        | VARCHAR(30) | NOTNULL, DEFAULT("city car")               |             |
| fuel            | VARCHAR(20) | NOTNULL, DEFAULT("Gasoline")               |             |
| mileage         | MEDIUMINT   | NOTNULL, UNSIGNED                          |             |
| power           | SMALLINT    | NOTNULL, UNSIGNED                          |             |
| gearbox         | VARCHAR(20) | NOTNULL, DEFAULT("Manual")                 |             |
| doors_number    | TINYINT     | NOTNULL, UNSIGNED, DEFAULT(5)              |             |
| seats_number    | TINYINT     | NOTNULL, UNSIGNED, DEFAULT(5)              |             |
| condition       | VARCHAR(50) | NOTNULL, default("Like new")               |             |
| bodywork_colour | VARCHAR(20) | NOTNULL                                    |             |
| previous_owners | TINYINT     | NOTNULL, DEFAULT(1)                        |             |
| license_plate   | CHAR(7)     | NOTNULL, UNIQUE                            |             |
| production_year | YEAR        | NOTNULL                                    |             |
| price           | FLOAT(8,2)  | NOTNULL, UNSIGNED                          |             |
