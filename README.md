# ep 23 - HELM



## datos de pgadmin a configurar en el chart
#### imagen
dpage/pgadmin4:4.26
https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html

#### variables
- PGADMIN_DEFAULT_EMAIL
- PGADMIN_DEFAULT_PASSWORD


## Crear un nuevo chart

```
$ helm create pgadmin4
```

## Guia para la creacion de charts oficial

https://helm.sh/docs/chart_template_guide/

## empaquetar el chart
```
$ helm package pgadmin4
```

## crear index del repositorio de charts

```
$ helm repo index .
```

## publicar

- subir a git 
```
git add .
git commit -m "publish"
git push origin master
git checkout -b gh-pages
git push origin gh-pages
```
- configurar github pages | rama gh-pages

## agregar repo

```
$ helm repo add nombre-repo URL
```


