# Trabajando con los repositorios

Un repo de charts de Helm es un sitio HTTP simple que proporciona un archivo index.yaml y charts empaquetados .tar.gz. El comando helm tiene subcomandos disponibles para ayudar a empaquetar charts y crear el archivo index.yaml necesario. En cualquier servidor web, servicio de almacenamiento de objetos o sitio estático, como las páginas GitHub, se pueden proporcionar estos archivos.

## Listar repositorios

Vamos a ver los repositorios de donde descargaremos nuestras aplicaciones.Nos la va a mostrar vacia porque acabamos de instalar helm.

``` ruby 
helm repo list
```
![repo](https://github.com/victorsanmar/helm/blob/main/imagenes/list.png)

## Añadir repositorios

Como nuestra lista esta vacia vamos a añadir un repositorio para poder descargar aplicaciones.En nuestro caso usaremos los de Bitnami.

``` ruby 
helm repo add nombre_repo direccion_repo
```
![repo](https://github.com/victorsanmar/helm/blob/main/imagenes/add.png)

## Quitar repositorios

Explicaremos el siguiente el comando por si el repositorio da cualquier fallo a la hora de desplegar aplicaciones.

``` ruby 
helm repo remove nombre_repo
```
![repo](https://github.com/victorsanmar/helm/blob/main/imagenes/remove.png)

## Buscar charts

Para buscar charts lo podemos hacer de dos modos:

### Linea de comandos

Que sería con la siguiente sintaxis

``` ruby 
helm search repo nombre_app
```
![repo](https://github.com/victorsanmar/helm/blob/main/imagenes/search.png)

### Gráfica

Mediante https://artifacthub.io/ podemos encontrar la aplicación que queramos.

![repo](https://github.com/victorsanmar/helm/blob/main/imagenes/artifact.png)




