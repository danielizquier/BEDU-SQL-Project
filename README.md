# Venta de videojuegos en volumen 🎮


### Descripción 📋

<img align="right" width="200" height="170" src="https://upload.wikimedia.org/wikipedia/commons/5/50/Tennis_For_Two_on_a_DuMont_Lab_Oscilloscope_Type_304-A.jpg">

La historia de los videojuegos tiene su origen en la década de 1950 cuando, tras el fin de la Segunda Guerra Mundial, las potencias vencedoras de la guerra, construyeron los  primeros superordenadores programables. Los **primeros intentos por implementar programas de carácter lúdico** (inicialmente programas de ajedrez) no tardaron en aparecer, y se fueron repitiendo durante las siguientes décadas. Los primeros videojuegos modernos aparecieron en la década de los 60, y desde entonces el mundo de los videojuegos no ha dejado de crecer y desarrollarse con el único límite que le ha impuesto la creatividad de los desarrolladores y la evolución tecnológica. 

### Objetivo :dart:

Con esta información se pretende analizar el impacto económico que han tenido las consolas y los videojuegos a lo largo de 37 años (1983 - 2017).

### Diseño y Creación 🛠️

Para este proyecto se tomaron en cuenta los datos compartidos de los siguientes repositorios:
- [Dataset Consolas](https://www.kaggle.com/jaimepazlopes/game-console-manufactor-and-sales/version/4)
- [Dataset Videojuegos](https://data.world/julienf/video-games-global-sales-in-volume-1983-2017)

<img align="centre" width="150" height="50" src="https://www.kaggle.com/static/images/site-logo.png"> <img align="centre" width="260" height="70" src="https://miro.medium.com/proxy/1*5A9pRkwKNWlSMUVho372jg.jpeg">

**Justificación:**

Se decidió hacer uso de una **_Base de Datos Relacional_** principalmente por 3 factores importantes:

- Experiencia propia en dicho tipo de DB.
- La naturaleza de los datos, ya que la información se obtuvo de forma independiente entre sí.
- El enfoque que se le quiere dar, esto debido a que se pretende aplicar los conocimientos adquiridos en el proyecto con el cual se colabora con Accenture, en donde actualmente ya se trabaja con el tipo de DB antes mencionada.

Una vez tomada la decisión, se limpiaron los datos de tal forma que tanto el formato como la presentación de dichos datos fuera estructurada, entendible y se pudiera relacionar facilmente.

<img align="centre" width="500" height="200" src=https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/CleaningDataSublime.PNG><img align="centre" width="500" height="200" src=https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/CleaningDataExcel.PNG>

Después, se procedió a realizar el diseño de la DB con la ayuda de la herramienta MySQL Workbench dando como resultado el siguiente diagrama entidad - relación.

![Videogames Sales](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/VideogamesSales_EntidadRelacion.png)

Una vez terminado el diseño y la limpieza de datos, se realizó la creación de la DB en el servidor creado anteriormente en la sesión 4. 

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/Schemas.PNG)

Una vez creadas las tablas, se procedió con la carga de datos. En este punto cabe mencionar que surgieron errores, los cuales ayudaron a corregir discrepancias en el planteamiento inicial del diseño de la DB al igual que la estructura y limpieza de los datos. 

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/LoadingData.PNG)

Finalmente se corroboró que los datos se cargaron correctamente haciendo un conteo de los renglones insertados. En este caso en particular, la carga de datos demoró demasiado por lo cual se optó por cargar un mínimo de al menos 500 registros.

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/count%20of%20sales.PNG)

### Planteamiento de preguntas ❓

Con la ayuda de la DB creada, se requiren responder las siguientes preguntas:

- ¿Cuáles son los 5 juegos mas vendidos?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P1.PNG)

- ¿Cuáles son los 5 juegos menos vendidos?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P2.PNG)

- ¿De qué consolas son los 5 juegos mas vendidos?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P3.PNG)

- ¿De qué consolas son los 5 juegos menos vendidos?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P4.PNG)

- ¿Qué juegos vendieron menos de 5 millones de copias?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P5.PNG)

- ¿Qué juegos de la consola PlayStation 3 son del género Sports?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/P6.PNG)

- ¿Cuál es la consola con mayor ventas de videojuegos en Japón y con qué cifra?

![](https://github.com/danielizquier/BEDU-SQL-Project/blob/main/Pictures/p7.PNG)


### Conclusión
**El conocimiento adquirido en este curso fue de gran valor, personalmente, las bases de datos son un tema que siempre había querido manejar sin embargo no había tenido la oportunidad. Debido a que actualmente me encuentro interactuando constantemente con DB, me comprometí a adquirir mas conocimientos para así poder aplicarlos a mi proyecto actual de Accenture y mejorar mi desempeño en los queries y manejo de estos. Me agradó la idea de crear un proyecto, ya que te obliga de cierta forma a meter las manos e inconscientemente hacer uso de las herramientas y recursos vistos a lo largo del curso.** 

**Considero que ahora tengo un mejor entendimiento y un mejor manejo de la información, conozco conceptos que me eran desconocidos, y el mejor beneficio que percibo es la perspectiva con la que ahora veo la información antes de ejecutar una consulta en una DB.**
