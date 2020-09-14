# Práctica 8
# Jekyll

### 1. Pre requisitos

Instalación de Ruby y para manejar sus dependencias
```
sudo apt-get install ruby
gem install bundler
```

Para la instalación de Jekyll, se sigue la guía dada en la [web oficial][jekyll]

[jekyll]: https://jekyllrb.com/docs/installation/ubuntu/

Una vez realizados todos los pasos allí indicados, se procede a instalar Jekyll
 
```
gem install jekyll bundler
```

### 2. Creación del proyecto

Se realiza la instalación del proyecto básico

```
jekyll new myJekyllWeb
```

y posteriormente para la compilación del proyecto y obtener el sitio en **"_site"**

```
jekyll build
```

### 3. Componentes del proyecto

Dependencias de GulpFile

    -Gulp
    -Sass
    -Browser-sync
    -Run

Con el objetivo de que Gulp se encargue de ejecutar algunas tareas de Jekyll. Si bien, jekyll realiza la compilación de los archivos Sass añadiendole unicamente el Front Matter al arhivo principal **.Scss**, también se añadió una tarea en el gulfile para que compile los archivos **.Scss** directamente en la carpeta **"_site"**

### 4. Tareas de gulp

**Jekyll:** La construcción del sitio se realiza a traves de una tarea de gulp, lanzandola en el shell con el comando gulprun.

**Sass:** Compilación de los archivos scss

**Serve:** Lanzar el servidor

**Default:** Se ejecutan en orden: Construcción del sitio, compilación de archivos Scss y por último lanzar el servidor

## TravisCI

## Despliegue Netfly

https://elastic-hugle-6284f9.netlify.app/