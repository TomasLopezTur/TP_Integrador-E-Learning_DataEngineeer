# Trabajo integrador del curso de Data Engineering de UTN E-Learning

### Funcionalidades

* Extracción de datos desde la API de CoinCap utilizando la biblioteca requests
* Conversión de los datos a DataFrames de Pandas
* Almacenamiento de los datos en archivos Delta Lake utilizando la biblioteca deltalake
* Implementación de un sistema para evitar duplicados al almacenar nuevos datos

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
Este proyecto se diseñó para ser utilizado como una practica de cómo implementar la extracción y almacenamiento de datos utilizando la API.
