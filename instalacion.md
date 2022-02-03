# Instalación de Helm

Para instalar helm lo vamos a hacer mediante un script y el comando curl.Esto nos permitira automatizar la instalación haciendo que sea de la forma más liviana posible.

El contenido del script es:

``` ruby 
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```
