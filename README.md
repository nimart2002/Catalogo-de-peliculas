# Catalogo-de-peliculas
Este proyecto es una herramienta de análisis de datos de películas. Utiliza **Pandas** para procesar y analizar un dataset local, se conecta a la API de **The Movie Database (TMDB)** para extraer información adicional (como las sinopsis) y utiliza la Inteligencia Artificial de **Google Gemini** para traducir y resumir esos textos automáticamente al español.
## 1. Cómo clonar el repositorio

Para obtener una copia local de este proyecto, abre tu terminal y ejecuta el siguiente comando:
```bash
# Clona el repositorio en tu equipo
git clone [PÓN AQUÍ_EL_ENLACE_A_TU_REPOSITORIO_DE_GITHUB]

# Entra en la carpeta del proyecto
cd [PON_AQUI_EL_NOMBRE_DE_LA_CARPETA_DEL_PROYECTO]
```
## 2. Instalar dependencias
Es recomendable ejecutar este proyecto dentro de un entorno virtual para no interferir con otras librerías de tu sistema. Ejecuta los siguientes comandos en tu terminal para crear el entorno e instalar los paquetes necesarios:

```
# 1. Crea el entorno virtual
python -m venv venv

# 2. Activa el entorno virtual
# En Windows:
venv\Scripts\activate

# 3. Instala todas las dependencias
pip install -r requirements.txt
```
## 3. Configurar las claves de acceso (API keys)
Este proyecto necesita conectarse a servicios externos, por lo que requiere credenciales privadas. Por motivos de seguridad, estas claves nunca deben subirse al repositorio. crea un archivo llamado exactamente `.env` y añade allí tus API keys:

```
TMDB_API_KEY=tu_clave_de_api_de_tmdb_aqui
GEMINI_API_KEY=tu_clave_de_api_de_google_ai_studio_aqui

```

## 4. Cómo ejecutar el proyecto
El flujo de trabajo principal está contenido en el Jupyter Notebook. Para ejecutarlo: asegúrate de que tu entorno virtual sigue activado (venv) y abre el archivo principal de Notebook. Selecciona el kernel correspondiente a tu entorno virtual y ejecuta las celdas en orden. El Notebook se encargará de leer los archivos `.csv` locales, realizar las peticiones HTTP a la API de TMDB y enviar los textos a la IA de Gemini para su traducción/resumen.
