Predicción del precio por noche en Airbnb Buenos Aires. Proyecto final de Data Science II (Coderhouse), Sofia Algamiz, 2026.

Partí de una pregunta simple: ¿cuánto debería cobrar por noche alguien que publica un alquiler temporario en Buenos Aires? Lo trabajé en dos etapas.

En la primera analicé unos 29.700 avisos de Airbnb (datos de Inside Airbnb, junio de 2026) y los crucé con datos de OpenStreetMap, como restaurantes y estaciones cerca de cada barrio, para ver qué se relaciona con el precio: la zona, las reseñas y las comodidades. También armé una presentación para un público que no es técnico.

En la segunda armé un modelo que predice el precio de un aviso y comparé varios algoritmos. El mejor se equivoca alrededor de un 17% en un aviso típico y queda dentro de un margen del 20% en más de la mitad de los casos. Lo que más explica el precio es el tamaño del alojamiento. Estar cerca de restaurantes o del transporte casi no agrega nada una vez que se sabe dónde queda el aviso, y comodidades como el gimnasio o la pileta suman bastante menos de lo que parecía: el gimnasio compartido pasa de +28% a +6% cuando se compara con propiedades parecidas. Al final uso el modelo para marcar los avisos que están publicados muy por debajo del precio que se esperaría para ellos.

Lo que hay en el repositorio:

- `Entrega_Final_Algamiz.ipynb`: el notebook de la entrega final, con el análisis, el modelo y las conclusiones. Se abre en Colab desde https://colab.research.google.com/github/sofidemier/DSII-Algamiz/blob/main/Entrega_Final_Algamiz.ipynb
- `data/`: los datos que usa el notebook.

La presentación de la primera entrega está en la carpeta de Drive y también en Google Slides: https://docs.google.com/presentation/d/1KqLvCPrA6Zr8B3nwIzc5SkPubbZXmISF/edit

Algunas cosas para tener en cuenta. El precio es el que figura publicado, no necesariamente el que se terminó cobrando. Los datos son de una sola ciudad y de una sola fecha, y los precios están en pesos, así que el modelo habría que actualizarlo con datos nuevos. Y lo que muestra el análisis son relaciones entre variables.

Los datos vienen de Inside Airbnb (insideairbnb.com) y de OpenStreetMap (a través de overpass-api.de). Material adicional en Google Drive: https://drive.google.com/drive/folders/1HV95MBVnrz2DqzGquyyj3ZNavTA09pyL?usp=drive_link
