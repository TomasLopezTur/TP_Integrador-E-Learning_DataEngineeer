# Trabajo integrador del curso de Data Engineering de UTN E-Learning

### Proyecto de Extracción y Almacenamiento de Datos 

Este proyecto tiene como objetivo desarrollar un sistema para extruir datos desde una API (en este caso, la API de CoinCap) y almacenarlos en un formato de archivo Delta Lake en version bronze y despues modificar los datos y prepararlos para guradarlos en otro Delta Lake version silver

<hr>

### Funcionalidades

* Extracción de datos desde la API de CoinCap utilizando la biblioteca requests
* Conversión de los datos a DataFrames de Pandas
* Almacenamiento de los datos en archivos Delta Lake utilizando la biblioteca deltalake
* Implementación de un sistema para evitar duplicados al almacenar nuevos datos
* Convertir columnas a tipos orrectos
* Modificar valores nulos a 0
* Crear columnas que indique qe los precios superan cierto limite y otra que indique el volumen del mercado es significativo
* Hacer un merge (JOIN) entre assets y markets basado en el símbolo base (base_asset)
* Calcular el volumen total en dólares y el promedio de transacciones por mercado


<hr>

### Componentes del Proyecto

* Modulo de extracción de datos (get_data.py): se encarga de realizar la petición a la API y convertir los datos en DataFrames
* Módulo de conversión a Delta Lake (save_data_as_delta.py): se encarga de almacenar los datos en archivos Delta Lake
* Módulo de upsert (actualizar o insertar) de datos (upsert_data_as_delta.py): se encarga de evitar duplicados al almacenar nuevos datos

<hr>

### Uso del Proyecto

1. Clonar el repositorio en tu entorno local
2. Instalar las dependencias requeridas mediante el comando pip install -r requirements.txt
3. Ejecutar los scripts de extracción y almacenamiento de datos (get_data.py y save_new_data_as_delta.py)
4. Verificar que los datos estén siendo almacenados correctamente en archivos Delta Lake

   <hr>
Notas
Este proyecto se diseñó para ser utilizado como una practica de cómo implementar la extracción, almacenamiento  y manipulacion de datos utilizando la API.
