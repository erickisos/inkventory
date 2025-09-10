# Inkventory

Esta es una aplicación para llevar el inventario de material, registro de citas y lo necesario para hacer un inventario en el estudio.

## Cómo usar esta plantilla?

Los siguientes comandos te permitirán generar el directorio `dist` que será utilizado para desplegar el proyecto en AWS.

```bash
mkdir -p dist/python/
poetry export -o requirements.txt
pip install . -t dist/python/
```

### Ejecutar la API localmente

Una vez que has instalado las dependencias, puedes ejecutar la API localmente utilizando el siguiente comando:

```bash
sam local start-api
```

Automaticamente, SAM se encargará de levantar un servidor local en el puerto 3000, y podrás acceder a la API en `http://localhost:3000/`. Además intentará utilizar el Layer definido dentro del archivo `template.yaml`.

## Cómo usarla en AWS?

> Esta sección está en construcción.

```bash
sam deploy --guided
```

O una vez que hayas configurado el archivo `samconfig.toml`:

```bash
sam deploy
```
