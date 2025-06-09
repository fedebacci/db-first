> NB: VEDERE IL FILE EXCEL PER DOMANDE E RAGIONAMENTI FATTI





| name                     | type                                                                             | attributes                         | index       |
| ------------------------ | -------------------------------------------------------------------------------- | ---------------------------------- | ----------- |
| id                       | BIGINT                                                                           | NOT NULL, AUTO INCREMENT, UNSIGNED | PRIMARY KEY |
| VIN                      | CHAR(17)                                                                         | NOT NULL, UNIQUE                   | INDEX       |
| brand                    | VARCHAR(50)                                                                      | NOT NULL, DEFAULT ("Sconosciuto")  |             |
| model                    | VARCHAR(25)                                                                      | NOT NULL, DEFAULT ("Sconosciuto")  |             |
| production_year          | YEAR                                                                             | NULL                               |             |
| first_ownership          | YEAR                                                                             | NULL, DEFAULT(production_year)     |             |
| km                       | MEDIUMINT                                                                        | NOT NULL, DEFAULT(0)               |             |
| customer_price           | MEDIUMINT                                                                        | NOT NULL, DEFAULT(0)               |             |
| agency_acquisition_price | MEDIUMINT                                                                        | NOT NULL, DEFAULT(0)               |             |
| agency_mantainance_price | MEDIUMINT                                                                        | NOT NULL, DEFAULT(0)               |             |
| engine_size              | SMALLINT                                                                         | NOT NULL, DEFAULT(0)               |             |
| engine_configuration     | ENUM("inline3", "inline4", "boxer4", "inline6", "v6", "v8", "v10", "v12", "v16") | NOT NULL                           |             |
| years_sitting            | SMALLINT                                                                         | NOT NULL, DEFAULT(0)               |             |
| hasCrashed               | BOOLEAN                                                                          | NOT NULL, DEFAULT(FALSE)           |             |
| buying_date              | DATE                                                                             | NOT NULL                           |             |
| selling_date             | DATE                                                                             | NULL                               |             |