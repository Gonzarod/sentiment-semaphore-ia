# sentiment-semaphore-ia

## Requisitos

- Node & npm
- Yarn (optional)
- Python 3.x
- Pip

## Pasos para ejecutar en modo desarrollo

- Descargar el repositorio o clonarlo

### Pobrar el código de generación de modelos (opcional)
- Descargar el archivo de Glove Embeddings de `http://dcc.uchile.cl/~jperez/word-embeddings/glove-sbwc.i25.vec.gz`
- Descomprimir el archivo descargado (900 mb) y colocarlo en la siguiente ruta: `minsa-twitter-sentiment-analysis\model_processing\glove`
- Abrir el archivo .ipynb de cualquiera de los 3 modelos y ejecutar

### Servidor

- `python3 -m venv venv`
- `source venv/bin/activate`
- `pip install -r requirements.txt`
- Ir a la ruta base del proyecto y ejecutar `python3 app.py` (es importante que se ejecute desde la ruta base, de otro modo no detectará los archivos del modelo pre entrenado)
- Ahora el servidor corre en la dirección `http://0.0.0.0:5000/`