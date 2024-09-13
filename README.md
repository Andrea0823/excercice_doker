# excercice_doker

## 2. Visuaizar lista de paquetes

```bash
pip freeze
```

## 3. Instalar todos los paquetes necesarios

```bash

```
## 6. Actualizar el repositorio

```bash
git add .
git commit -m "CREATED hola mundo"
git push -u origin main
```

-------------------------------------------------------------------------------
## Crear imagen

```bash
docker build -t image:tag .
```

## Correr contenedor

```bash
docker run -p 8080:8080 andrea:v3
```

## Muestra contenedores dormidos

```bash
docker ps -a
```
## Contenedores activos

```bash
docker ps
```

## Apagar los contenedores
```bash
docker kill (nombre del contenedor)
```
## Muestra en interactivo

```bash
docker start -i (nombre del contenedor)
```
## Iniciar el contenedor
```bash
docker start (nombre del contenedor)
```

## Iniciar sesion
```bash
docker login
```

## Crear etiqueta
```bash
docker tag (nombre de la imagen) usuario/ponerle un nombre:latest
```

## Subir imagen
```bash
docker push nombredelusuario/nombredelaimagen
```
