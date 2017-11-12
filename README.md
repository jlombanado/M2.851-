# M2.851 - Tipología y ciclo de vida de los datos aula 1

El Ayuntamiento de Toledo ha decidido realizar análisis de sentimiento en las principales redes sociales de referencia, en relación a las opiniones manifestadas por los turistas con respecto a la ciudad y las principales atracciones que ofrece. Para ello, se han propuesto como objetivo conocidas redes como facebook o twitter, pero también otros sitios web turísticos donde la gente expresa libremente su opinión en relación a determinados sitios de interés (ciudades, hoteles, restaurantes etc.). Uno de estos sitios web que se ha propuesto como objetivo principal para el presente estudio, es www.tripadvisor.com.

Según Wikipedia, TripAdvisor es una empresa estadounidense de sitios web de viajes que ofrece reseñas de viajeros sobre sus experiencias en hoteles, restaurantes, ciudades  y monumentos. Stephen Kaufer y Langley Steinert fundaron TripAdvisor en febrero de 2000 como un sitio que incluye información de guías, periódicos y revistas. InterActiveCorp compró el sitio en 2004, y un año después, se separó de su grupo de viajes de negocios, Expedia. Después de eso, el sitio web recurrió al contenido generado por el usuario. Desde entonces se ha convertido en la comunidad de viajes más grande, llegando a 390 millones de visitantes únicos cada mes y enumerando 465 millones de opiniones y opiniones sobre más de 7 millones de alojamientos, restaurantes y atracciones en 49 mercados en todo el mundo. 

La siguiente figura muestra un pantallazo de la página de tripadvisor vinculada a la ciudad de Toledo y que es objeto de este estudio. 



# Web Scrapping

Para el desarrollo de la aplicación se ha utilizado python, y como entorno de trabajo, Anaconda. Como librerías se ha utilizado beautifulSoup para la lectura y desglose de las variables desde html y urlopen para la lectura de la web. Así mismo, en su segunda parte, la aplicación transforma el resultado del ejercicio de web scrapping realizado a dataframe y genera un fichero csv con la salida resultante, para lo cual se ha utilizado también la librería pandas.

El dataset resultante contiene sólo 4 variables principales (título, opinión, rate y fecha) ya que he considerado que dicha información era suficiente para dar respuesta al objetivo del ejercicio, pero para futuras mejoras y ya orientándolo más al análisis de sentimiento propondría introducir datos demográficos de clientes (edad, sexo, nacionalidad). Una particularidad de tripadvisor es que los clientes que opinan deben haber creado un perfil previamente y este es público, por lo que sería muy interesante enriquecer nuestro dataset con dicha información.

La aplicación generada dispone además de la posibilidad de introducir por código el número de páginas sobre las que se quiere realizar web scraping. Por defecto se ha marcado a 20, por considerar esa cantidad suficiente para hacer demostración de funcionalidad, pero la idea sería poder introducir tanto la web de referencia como el número de páginas como parámetro y así no tener que modificar el código.

