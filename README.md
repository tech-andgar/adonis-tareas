# Una simple lista de tareas construida con AdonisJS

## Cómo empezar

Clone el repositorio del proyecto ejecutando el siguiente comando si utiliza SSH

```
git clone git@github.com:andgar2010/adonis-tareas.git
```

Si usa https, use esto en su lugar

```
git clone https://github.com/andgar2010/adonis-tareas.git
```

## Configuración

Ejecute el siguiente comando para instalar dependencias

```
npm install
# or "yarn install"
```

### Descarga del navegador

Dado que este repositorio depende de[puppeteer] (https://github.com/GoogleChrome/puppeteer) para realizar las pruebas, se requiere una versión de `Chromium` incluida.

La instalación de **Chromium** puede tardar un poco y opcionalmente puede omitirla ejecutando el siguiente comando.

```
PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true npm install
```


### Variables de entorno

Duplicar `.env.example` y renombrarlo `.env`.


### Migraciones

Configure su base de datos e introduzca lo siguiente en `.env

```
DB_CONNECTION=mysql
DB_HOST=localhost
DB_DATABASE=adonis-tareas
DB_USER=root
DB_PASSWORD=
```

Ejecute el siguiente comando para ejecutar la migración.

```
adonis migration:run
```

Por último, inicie la aplicación:

```
adonis serve --dev
```

y visite http://127.0.0.1:3333/ para ver la aplicación en acción.
