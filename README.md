# Prueba técnica de Ayuda T Pymes

## Introducción

Este proyecto ha sido desarrollado utilizando Vue3 como framework de Javascript. Se usó Vue3 por encima de otros frameworks como Angular o React por la diferencia de experiencia entre los distintos frameworks.

Para gestionar los estilos de la aplicación, se ha empleado el preprocesador CSS Sass. Además, se ha adoptado la metodología BEM para obtener una estructura de clases mas clara, facilitando así el mantenimiento de los selectores.

El proyecto fue desplegado a traves de Github Pages y su visualización: [Web](https://miguelchorat.github.io/ayudat_prueba/)

## Instalación

### Requisitos previos

-  Git
-  Node.js

### Pasos a seguir

#### Clonar el repositorio

Abrir la linea de comandos del sistema operativo(O en visual studio code) y navegar hasta la carpeta donde desees guardar el proyecto.

A continuación usar el siguiente comando de git para clonar el repositorio del proyecto.

```
git clone https://github.com/Miguelchorat/ayudat_prueba.git
```
#### Acceder al directorio del proyecto

```
cd ayudat_prueba
```
#### Instalar dependecias de node

```
npm i
```
#### Iniciar servidor

Una vez iniciado el servidor con el siguiente comando podras acceder a la web a traves del enlace local administrado por el comando.
```
npm run serve
```

## Desarrollo del proyecto

El proyecto se creo siguiendo una arquitectura basada en componentes, aprovechando las fortalezas de Vue 3. La estructura permitió la creación de componentes reutilizables como botones, tarjetas de reseña, tarjetas de FAQ, etc.

Se desarrollaron componentes simples, como una tarjeta de reseña individual, y se combinaron con un array de datos (simulando una base de datos) para generar dinámicamente múltiples reseñas. En el caso de los botones fueron diseñados para que utilizando variables pueda controlar su apariencia y el enlace al que dirigían.

Se aplicó la metodología BEM para organizar las clases CSS, asegurando un estilo consistente y facilitando el mantenimiento del código. Además, se implementaron mecanismos de comunicación entre componentes padre e hijo, utilizando variables para sincronizar el comportamiento de elementos como el header (que se desplazaba junto con el contenido) y el menú móvil (que se desplegaba al hacer clic).

Y para garantizar una experiencia amigable en diferentes dispositivos, se diseñó la web con un enfoque responsive, adaptando el diseño a distintas resoluciones de pantalla. Se utilizaron unidades relativas (em, rem, vh, vw) y media queries para asegurar que el contenido se ajustara correctamente a cualquier tamaño de pantalla.
