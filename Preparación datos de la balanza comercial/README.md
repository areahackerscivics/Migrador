# Descripción del contenido

- **Datos en bruto**: Aquí se encontrará el enlace a los datos públicos que se han empleado para la generación de la información relevante a la balanza comercial, los datos proceden de la *Agencia Tributaria*.

- **Scripts**: En esta carpeta se encuentran los scripts que se han usado para generar la tabla que posteriormente se ha usado para crear las visualizaciones con *Tableau*.
  - **R**: Se han creado dos scripts diferentes:
    - *script_creacion_tabla_agencia_trib_y_tabla_scrapeo.Rmd*: En este script se leen los datos procedentes de la *Agencia Tributaria*, se filtran dejando solo los datos de la ciudad de València y se almacenan en una misma tabla. Se codifica el codigo de país de Namibia (NA) para que no sea reconocido como un valor faltante *NA*, se seleccionan las variables que nos interesan y se guarda la tabla resultante con el nombre *tabla_productos_codigo_nc.csv*. *Nota: Esta tabla no ha sido dejada en la carpeta de tablas generadas, ya que ocupa 99,4 MB*. Por otro lado se obtiene una tabla que se ha llamado *codigo_nc_scrapeo.csv* con los códigos de los productos importados y/o exportados, que posteriormente se ha usado con la librería *Scrapy* de *Python* para obtener las categorías de los productos scrapeando la página [European Customs Portal](https://www.tariffnumber.com/).
    - *script_creacion_tabla_agencia_trib - anual - agrupaciones.Rmd*: En este script 
