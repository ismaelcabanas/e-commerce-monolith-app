# E-commerce monotlih application

<!-- Badger start badges -->

<!-- Badger end badges -->

## The goal of this project

[NAME] APPLICATION



## Domain
El dominio de la aplicación será un e-commerce donde el usuario podrá seleccionar productos de un catálogo e 
incluirlos en un carrito de la compra para poder realizar un pedido de los productos que se encuentren en el 
carrito de la compra.

### Domain description

### Requisitos funcionales

- Como usuario quiero listar productos
- Como usuario quiero filtrar productos por marca y categoría
- Como usuario quiero poner productos en un carrito de la compra para que pueda comprarlos más tarde
- Como usuario quiero aplicar cupones de descuentos y ver el coste total de todos los artículos que están en mi carrito de la compra
- Como usuario quiero comprar los artículos del carrito de la compra y hacer un pedido
- Como usuario quiero tener un listado de mis anteriores pedidos y tener un histórico de los artículos de los pedidos
- Como un usuario logado quiero que cuando acceda al sistema éste me recuerde los artículos que tenía previamente en el carrito de la compra

### Requisitos no funcionales

- Escalabilidad, la aplicación debería ser capaz de servir peticiones a miles de usuarios
- Disponibilidad, la aplicacón debería estar disponible 24x7
- Fiabilidad, la aplicación no debería de caerse 24x7
- Mantenibilidad, la aplicación debería ser fácil de mantener durante años
- Usabilidad
- Eficiencia, la aplicación deberían tener una latencia aceptable por debajo de los 2 segundos.

En cuanto a eficiencia, empezaremos por una aplicación con bajo volumen de usuarios, alrededor de 2k y 0,5K peticiones por segundo.

Conforme la aplicación vaya creciendo iremos aumentando este requisito no-funcional.

## Run

```
docker-compose up -d
./gradlew run
```

## Test

```
./gradlew test
```

## Integration Test

Default [ApplicationIntegrationTest](src/integration-test/java/cabanas/garcia/ismael/meetup/infrastructure/ApplicationIntegrationTest.kt) uses [testcontainers](https://www.testcontainers.org/) and [docker-compose.yml](docker-compose.yml)

You can add additional @Nested testcases sharing the same docker-compose execution or use any other approach to your liking

```
./gradlew integrationTest
```

## Useful links

