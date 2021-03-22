# Operación fuego de Quasar
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Información

QuasarApp es un Api Rest que provee servicios para la interpretación de mensajes recibidos por los satelites (kenobi, skywalker y sato) y a partir de estos determinar la posicion del emisor de estos mensajes.

## Features

Se encuentra desarrollado en C# .Net Core y como base de datos Sql Server. El servicio se encuentra alojado en AWS

La aplicacion cuenta con: 

- MiddlewareException y CustomExceptions
- EntityFramework 
- AmazonLamda

## Ejecución

Puede descargar el collection de postman desde este [ enlace](https://www.getpostman.com/collections/05efd7c963977732a7c3)


| url      | descripción                       |
|:--------------|:----------------------------------|
| `/topsecret`      | Devuelve la posicion y mensaje a partir de la distancia y mensajes recibidos
| `/topsecret_split/{satelliteName}`    | Actualiza la posicion y mensaje que recibe un satelite en particular
| `/topsecret_split` | Devuelve la pocicion y mensaje a partir de los datos enviados por el método `/topsecret_split/{satelliteName}`  |
