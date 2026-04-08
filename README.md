# SCRAPING_DATA_UP

## What does the project do?
El proyecto tiene como objetivo extraer de la pagina web https://admision.unmsm.edu.pe/Website20262/A/A.html, todos los urls de las diferentes escuelas profesionales para iterar mediante python la data de los resultados del examen de admision 2026-II de cada uno de los urls. Cada url cuenta con una base de datos en formato DataTables (JavaScript pagination) por lo que cuenta con diferentes paginas que mediante selenium hacemos web scrapping para automatizar la busqueda de si existen o no más paginas por cada link.
## How to install the dependencies?
Para este proyecto utilizamos las siguientes librerias.
!pip install selenium
!pip install webdriver-manager
!pip install pandas
!pip install numpy
!pip install unidecode
Luego ejecutamos el scrpit con nombre Scraper.ipynb
## How to run the script?
El script es un script didactico pues cuenta con pasos cuyo objetivo si bien no es hallar la solución general del problema, son pruebas importantes que se realiazon para analizar los posibles errores, la logica detras del comando final y pruebas que se hicieron para un solo link para una sola pagina de los datos, para probar el metodo mas efciente para luego iterarlo para las diversas paginas de los diversos urls. Importante si desea ejecutar el comando sin estos pasos previos, descargar las liberias, ejecutar el codigo que abre la pagina https://admision.unmsm.edu.pe/Website20262/A/A.html, ejecutar el codigo que descarga los urls para finalmente ejecutar los dos ultimos comandos de los cuales el penultimo mediante selenium scrappea la data final y el ultimo comando lo guarda en un excel llamado resultados_sanmarcos.xlsx.
## What does the output contain?
El output contiene un excel donde guarda toda la información url de escuela profesional por url extrayendo para cada uno las diversas paginas que contiene la informacion y mediante append colocando las de la siguiente url, dandonos como resultado la extraccion de 25881 datos en total, siendo las columnas: codigo, apellidos y nombres, escuela, puntaje, mérito p.e. y observación
