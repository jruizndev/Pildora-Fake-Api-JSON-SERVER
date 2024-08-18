# Pildora formativa Fake Api: JSON SERVER
![logoJSON](https://miro.medium.com/v2/resize:fit:700/1*o2ATIldynmbje1lV6HN9lg.png)
## Objetivo de la presentación
Explorar cómo crear APIs falsas con JSON Server usando un ejemplo de Pokémon. Aprender a realizar filtrados utilizando el método get.

Presentación canva: https://www.canva.com/design/DAGOMK6THwk/u58-R5NBjX7MpNGyLRV8hQ/edit

## Requisitos previos

Tener instalado Node.js

## Puntos clave de la presentación

- Instalación JSON SERVER a través de terminal
```bash
npm install -g json-server
```

- Creación en Visual Studio Code un archivo .json

- Ejemplo Fake Api Pokemon

- Iniciar el Servidor para testear Api Pokemon

```bash
json-server --watch pokemon.json
```

- Navegar por http://localhost:3000 para ver los endpoints automáticos

- Filtrado utilizando método GET Fake Api Pokemons:

Obtener todos los Pokémon de tipo Water: 
 /pokemons?type=Water

Obtener todos los Pokémon con nivel mayor o igual a 20:  
/pokemons?level_gte=20

Obtener todos los Pokémon entrenados por Misty (trainerId=2):  /pokemons?trainerId=2

Obtener todos los Pokémon ordenados por nivel ascendente:  
/pokemons?_sort=level&_order=asc.

Obtener todas las batallas ganadas por Brock (winnerId=3):  
/battles?winnerId=3

## Ejercicio práctico 
- Creación de un array (clothing) con la siguiente estructura: 

```bash
{
    "clothing": [
        {
            "id": "",
            "item": "",
            "brand": "",
            "size": "",
            "price": ,
            "inStock": true or false,
        },
...
]
}
```
- Iniciar servidor

```bash
json-server --watch clothing.json
```

- Realizar un filtrado por marca (brand)
- Realizar un filtrado por disponibilidad (inStock)
- Realizar un filtrado por precio ascendente (price)
- Realizar un filtrado por tamaño (size)
