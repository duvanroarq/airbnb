
![Logo](https://drive.google.com/file/d/1yvZC3g0BluPyTuX4J-b8s71En-ufWOd5/view?usp=sharing)


# Airbnb: Oportunidades de inversión en Buenos Aires

El objetivo de este proyecto es aplicar un análisis exploratorio de los datos, obtenidos a través de la web de Airbnb para la ciudad de Buenos Aires, y establecer un análisis descriptivo de los datos para informar a inversionistas sobre posibles oportunidades de inversión. 
## Datasets de origen

El proyecto parte de 3 archivos .csv de estructura tabular separados por comas.

- Calendar: Está compuesto por una lista de fechas que establecen la disponibilidad de cada uno de los alojamientos acorde a las actualizaciones realizadas por cada uno de los anfitriones.

- Listings: Es una lista de alojamientos que posee un total de 71 columnas con información de los anfitriones, calificaciones realizadas por huespedes, metadata, precios, tipos de propieda, entre otros más.

- Reviews: Es una lista de las reseñas realizadas por cada uno de los reseñadores, incluye información sobre el reseñador y comentarios del mismo.

## Decisiones de transformación

El mayor tabajo de transformación se realizó en la tabla de listings debido a la cantidad de columnas que existían. A continuación algunas decisiones que se tomaron al respecto:

- Segunda forma normal: Para dar cumplimiento a esto se crearon nuevas tablas para segmentar los datos en función de cada atributo. Se crean las siguientes tablas: 

    - Cities: Compuesta por un idCiudad, el Estado y el IdPais al que pertenecen.
    - Countries: Compuesta por el IdPaís y el nombre del país.
    - Hosts: Compuesta por el IdHost, el nombre del anfitrión, la fecha de registro en la plataforma, el tipo de anfitrión, el número de alojamientos que administra y el id de la ciudad en la que reside.
    - HostsMetadata: Almacena información secundaria del anfitrión.
    - Lodges: Lista de los alojamientos, con su nombre, idHost, Latitude y Longitude y el idNeighborhood.
    - LodgesAbout: Incluye una lista de descripciones realizadas por el anfitrión sobre su alojamiento.
    - LodgesDetails: Incluye detalles sobre el alojamiento, como el tipo, el número de habitaciones, baños y los amenities.
    - LodgesMetadata: Almacena información secundaria del alojamiento.
    - LodgesPolicies&Restrictios: Incluye algunas restricciones sobre el alojamiento y su politica de cancelación.
    - LodgesPrices: Información sobre las tarifas por noche, por huesped extra, depósito de seguridad, recargo por limpieza y número máximo de huespedes.
    - LodgesRatings: Incluye información sobre las calificaciones realizadas al alojamiento.
    - NeighborhoodsBA: Incluye una lista de los barrios que hacen parte de la ciudad de Buenos Aires.
    - Reviewers: Una lista con los nombre de los reseñadores.
    - Reviews: Una lista de cada una de las reseñas por IdLodge.

- Tercera forma normal: Se crean realaciones entre las tablas para facilitar las consultas, se crean id para cada una de las tablas. 
## Preguntas planteadas

¿Cuál es la mejor manera de invertir en Airbnb?

- De acuerdo al análisis las mejores propiedades para invertir en Airbnb son las Casas, Condominios TownHouse, y apartamentos. Ya que presentan mayor rentabilidad en cobro por noche.

- Sin embargo, si se ve desde el costo por alojamiento por noche y no por huesped, la mejor opción sería una villa, seguido de las casas, apartahoteles y condominios.

¿En dónde es mejor invertir?

- De acuerdo al análisis el mejor barrio para invertir es San Cristóbal, ya que en promedio triplica el valor por noche que otros barrios como Puerto Madero y Retiro.

Para mayor información sobre el análisis, consultar el archivo Airbnb.
## Documentación

[Airbnb](https://news.airbnb.com/about-us/)

