# Ejecución de Tests Funcionales del Modelo de Crédito

### Paso 0: Ingrese al Escritorio remoto

### Paso 1: Levantar el contenedor de Python

```
docker run -it --rm -p 8888:8888 jupyter/pyspark-notebook
```

### Paso 2: Configurar git

Abra una Terminal en JupyterLab e ingrese los siguientes comandos

```
git config --global user.name "<USER>"
git config --global user.email <CORREO>
```


### Paso 3: Clonar el Proyecto desde su propio Github

```
git clone https://github.com/<USER>/trabajo-final-mle.git
```


### Paso 4: Instalar los pre-requisitos

```
cd trabajo-final-mle/

pip install -r requirements.txt
```


### Paso 5: Ejecutar las pruebas en el entorno

```
cd src

python make_dataset.py

python train.py

python evaluate.py

python predict.py

cd ..
```


### Paso 6: Guardar los cambios en el Repo

```
git add .

git commit -m "Pruebas Finalizadas"

git push

```
