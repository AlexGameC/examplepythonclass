
# examplepythonclass
## Alex Gamero

En este README, se proporcionan instrucciones claras sobre cómo construir la imagen Docker, ejecutar el contenedor Docker y dónde encontrar el archivo python.

# Para construir la imagen se debe considerar dentro de la carpeta src/ los archivos model.pkl y normalizador.pkl (No fueron cargador debido a que se solicitó que el gitignore los discriminara), usar el siguiente comando:

```
docker build -t mlpulsar .
```

# Enviar los parametros a la imagen por variable de entorno ejemplo:

```
docker run -e values='-0.234571412,19.11042633,74.24222492' mlpulsar
docker run -e values='1.547196967,61.71901588,3.662680136' mlpulsar
```

[Archivo Jupyter Notebook](https://drive.google.com/file/d/1wJfK9IFE8DQtA71v3V8aJ8fj7xIfK2nA/view?usp=sharing).

