# Laboratorio 2 - Analitica de Datos 
##### En este laboratorio, desarrollarás un motor de búsqueda de cursos y un rastreador web que recopila información de un catálogo universitario para construir un índice. El objetivo es brindarte experiencia en programación en Python y trabajar con documentos HTML obtenidos de la web.
#### Autores: Gabriela Mercedes Luigi, David Mateo Henao

- ##### Introducción:
  Para el desarrollo de este taller vamos a estar utilizando como nuestra  base de información el portal Web de la Javeriana para los cursos que la universidad ofrece parte de las carreras de Pregrado, Posgrados y Titulaciones. Este fue el enlace utilizado para el desarrollo de este proyecto: 
  https://educacionvirtual.javeriana.edu.co/temporomandibulares

  Con el fin de lograr este objetivo, desarrollaron tres programas principales: crawler.py, search.py y compare.py, cada uno desempeñando un papel crucial en el proceso de recopilación, búsqueda y comparación de datos.

- ##### Procedimiento:

  En primer lugar, el programa crawler.py se encargó de rastrear el sitio web de la universidad objetivo y extraer información relevante sobre los cursos         disponibles. Utilizando la biblioteca BeautifulSoup para analizar el contenido HTML de las páginas web, el rastreador identificó los elementos que contenían detalles sobre los cursos, tales como el nombre, la duración, el nivel de dificultad, la fecha de inicio y el precio. Luego de recolectar estos datos, los almacenó en un formato estructurado, primero en un archivo JSON para una fácil manipulación y luego exportándolos a un archivo CSV para un análisis más tabular y accesible.

  Con la información recopilada y almacenada, el siguiente paso fue facilitar a los usuarios la búsqueda de cursos relevantes. Para ello, se implementó el programa search.py, que permitió a los usuarios especificar sus intereses mediante una lista de palabras clave. El programa cargó los datos de los cursos desde el archivo JSON generado previamente y realizó una búsqueda exhaustiva, buscando coincidencias entre los intereses proporcionados y los nombres de los cursos. Esto resultó en una lista de cursos que coincidían con los intereses del usuario, lo que simplificó significativamente el proceso de búsqueda y selección de cursos relevantes.

  Finalmente, para brindar una funcionalidad adicional de comparación entre cursos, se desarrolló el programa compare.py. Este programa evaluó la similitud entre dos cursos dados, considerando diferentes atributos como la duración, el nivel de dificultad, la fecha de inicio y el precio. Asignando pesos a cada atributo para reflejar su importancia relativa en la comparación, el programa calculó una puntuación de similitud total, lo que permitió a los usuarios tomar decisiones informadas al elegir entre cursos similares.
  
