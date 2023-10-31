#  Robot Trading | Python | Data Science | Alura
<br>
<ul align = center>
<img src="https://github.com/Valamca/Robot_Trading/assets/129345721/f457dc3e-d900-4bf8-be4e-906275c275ba"/><br>
<img src="https://img.shields.io/badge/_Python-f7e172?style=flat&logo=python" />
  <img src="https://img.shields.io/badge/_Jupyter_Notebook-767677?style=flat&logo=jupyter"/>
  <img src="https://img.shields.io/badge/_Pandas-e00484?style=flat&logo=pandas"/>
  
</ul>


## Descripción: :page_facing_up: 🤖
Este programa en Python capaz de tomar decisiones de compra y venta de Bitcoin en tiempo real, ¿Interesante verdad?.

### Configuración del ambiente: :computer: 
Para empezar, se puede utilizar cualquier entorno de Python, tan sólo asegúrate que sea una versión 3.X, el base es Jupyter Notebook, también necesitarás instalar algunas librerías de Python que son esenciales para este proyecto, como: <br>
<br>
- Pandas 
- Numpy 
- Matplotlib
- Yfinance
- Time
- BeautifulSoup
- Request

### Obtención de datos: :page_with_curl: 
Para la obtención de datos se recurrió al uso de la API llamada YFinance que proporciona los datos históricos de precios de Bitcoin y muchas mas monedas en formato JSON. Su documentación la encontrarán en el siguiente enlace: https://pypi.org/project/yfinance/ <br> 

![image](https://github.com/Valamca/Robot_Trading/assets/129345721/b296ee83-768f-4269-a5d0-f451be1b0850)

Por otro lado, se realiza Web Scraping en un sitio de noticias para obtener el precio actual y algunos indicadores de tendencias del Bitcoin <br>
El sitio elegido fue: https://coinmarketcap.com <br>
<br>
![image](https://github.com/Valamca/Robot_Trading/assets/129345721/4f3e3df5-1afe-4c40-8610-9589e6d8c10e)

### Limpieza de datos: :mag_right:
Una vez se tienen los datos históricos, se cargan en un DataFrame de Pandas para poder manipularlos y analizarlos, dónde se identifican y eliminan los outliers, además de tratar cualquier valor nulo o duplicados en la base. Finalmente, con la base limpia, se calcula el precio promedio del Bitcoin.

### Tomar decisiones: :bangbang:
Con la obtención del precio promedio, se compara con el precio actual y tendencia del Bitcoin, que previamente se obtuvo con Web Scraping. Si el precio actual es mayor/igual que la media y la tendencia es de baja, entonces se debe vender, pero si el precio actual es menor que la media y la tendencia es de alta, entonces se debe comprar, si ninguna condición se cumple, la instrucción es esperar.

### Visualización: :bar_chart:
Se utiliza la librería Matplotlib para crear un gráfico donde se muestre la evolución del precio del Bitcoin durante el periodo seleccionado, y una línea recta que pase sobre el precio medio. Por último, se muestra un mensaje en el gráfico que indique “Vender”, “Comprar” o “Esperar” según sea la decisión del algoritmo.<br>
<br>
![image](https://github.com/Valamca/Robot_Trading/assets/129345721/59c4e4ce-a0f7-4acb-b4dd-1a93f1dced2c)


### Automatización: :arrows_counterclockwise:
Finalmente, ahora que se tienen: la extracción de información,  la limpieza de datos, la visualización, y el algoritmo de decisión, es hora de automatizar el proceso. Se utiliza la librería de Python "time" para ejecutar el algoritmo de decisión cada 5 minutos y actualizar el gráfico, además del método clear_output para limpiar el gráfico antes de volver a iniciar el ciclo.<br>
<br>


**Desarrollador** :wink: 

 <img src="https://avatars.githubusercontent.com/u/129345721?v=4" width=115>
 
 **Francisco Valam Cortes**  <br>[<sub>GitHub</sub>](https://github.com/ValamCA) <img src="https://i.postimg.cc/hPxhb2YB/icons8-github-50.png" width =16>
 <br>[<sub>Linkedin </sub> ](https://www.linkedin.com/in/franciscovalamca/)<img src="https://i.postimg.cc/C5LJHycc/icons8-linkedin-48.png" width =16 ><br>
 [<sub>Twitter</sub>](https://twitter.com/FNiggalam)<img src="https://i.postimg.cc/xTrL2ND9/icons8-twitter-48.png" width =16 ><br>
