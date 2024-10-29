# Procesamiento de Imágenes con Suavizado y Afilado 
Este proyecto implementa un sistema de procesamiento de imágenes con una interfaz de usuario que permite aplicar técnicas avanzadas de optimización para el suavizado y afilado de imágenes. Se utilizan dos algoritmos metaheurísticos, Evolución Diferencial y Búsqueda Tabú, para maximizar la relación señal-ruido (SNR) de las imágenes, logrando una mejora notable en la claridad y calidad visual.

## Tabla de Contenidos 
- [Introducción](#introducción)
- [Funcionalidades](#funcionalidades)
- [Requisitos](#requisitos)
- [Estructura del Código](#estructura-del-codigo)
- [Configuración e Instalación](#configuracion-e-instalacion)
- [Uso de la interfaz](#uso-de-la-interfaz)
- [Detalles Técnicos](#detalles-tecnicos)
- [Demostracion del resultado](#demostracion-del-resultado)
- [Créditos](#creditos)

## Introducción 
El procesamiento de imágenes es esencial en diversos campos, desde la fotografía digital hasta la visión artificial. Este proyecto proporciona una herramienta interactiva de procesamiento de imágenes, centrada en el suavizado y afilado mediante algoritmos de optimización metaheurística. La Evolución Diferencial se emplea para mejorar el suavizado de la imagen, mientras que la Búsqueda Tabú optimiza el afilado, ajustando iterativamente las máscaras de filtrado.

## Funcionalidades

 1. **Interfaz de Usuario:** Interfaz gráfica simple e intuitiva que permite cargar una imagen, ejecutar los algoritmos de suavizado y afilado, y visualizar el progreso.
 2. **Suavizado con Evolución Diferencial:** Algoritmo de optimización poblacional para el ajuste fino de la máscara de suavizado.
 3. **Afilado con Búsqueda Tabú:** Algoritmo de búsqueda que evita soluciones repetitivas y estancamiento, optimizando la máscara de afilado para mejorar el SNR.
 4. **Indicador de Progreso:** Barra de carga que muestra el avance en tiempo real de los algoritmos aplicados.
 5. **Resultados:** Generación de una imagen procesada con ajuste controlado de suavizado y nitidez.


## Requisitos
Este proyecto requiere Python 3.7 o superior y las siguientes bibliotecas:

 - `numpy`
 - `opencv-python`
 - `Pillow`
 - `tkinter`
 - `customtkinter`
 
Instala estas dependencias usando:

    pip install customtkinter opencv-python pillow numpy

## Estructura del Código
El proyecto se compone de los siguientes módulos clave:

 - **proyectoGUI.py:** Controla la interfaz de usuario y la visualización de la barra de progreso.
 - **eliminacionRuido_DE.py:** Implementa el suavizado de imágenes usando Evolución Diferencial.
 - **taboo_img.py:** Optimiza el afilado mediante Búsqueda Tabú.

## Configuración e Instalación

 1. **Clona el Repositorio:**
     `git clone https://github.com/xCrisFlores/ProyectoMetaheuristicos`

 3. **Navega al Directorio del Proyecto:**
    `cd ProyectoMetaheuristicos`

 4. **Instala las Dependencias:**
    `pip install customtkinter opencv-python pillow numpy`

## Uso de la interfaz

1. Selecciona una imagen desde tu sistema para procesarla.
2. Introduce las cantidades de iteraciones deseadas para cada imagen producida.
3. Presiona continuar y esperar a su ejecucion, la barra de carga demostrara el progreso.
4. La interfaz mostrará la imagen procesada comparada con su versiones con suavizado y afilado.

## Detalles Técnicos
### Interfaz de Usuario
La interfaz, diseñada en proyectoGUI.py, permite al usuario interactuar con el sistema de procesamiento de imágenes. Consta de opciones para cargar imágenes y controles para ajustar el suavizado y afilado, además de mostrar una barra de progreso en tiempo real.

### Algoritmo de Suavizado: Evolución Diferencial
La Evolución Diferencial (ED) es un algoritmo de optimización basado en poblaciones, diseñado para encontrar los mejores parámetros de suavizado de la imagen. Inicializa una población de máscaras y aplica operadores de mutación y cruzamiento para mejorar el ajuste, logrando reducir el ruido en la imagen.

### Algoritmo de Afilado: Búsqueda Tabú
La Búsqueda Tabú es un procedimiento metaheurístico que utiliza memoria adaptativa para evitar soluciones repetitivas. Optimiza los parámetros de afilado aplicando una máscara adaptativa que maximiza la nitidez. Las iteraciones controlan las mejoras en el SNR, garantizando un aumento de claridad sin distorsiones.

## Demostracion del resultado
![Interfaz del Proyecto](https://drive.google.com/uc?id=1dGm3yCAPW_VVDtDOMaSQhhI3ITBvHIhK)


## Créditos

<p align="center">
  <img src="https://practicas.cucei.udg.mx/dist/imagenes/logo_cucei_blanco.png" alt="Logo CUCEI" width="350">
</p>

<div align="center">
  <table>
    <tr>
      <td align="center"><strong>Flores Rosales Cristian Alejandro</strong></td>
    </tr>
    <tr>
      <td align="center"><strong>Guerrero Sulvaran Ángel Jesús</strong></td>
    </tr>
    <tr>
      <td align="center"><strong>Gutierrez Vazquez Paul</strong></td>
    </tr>
    <tr>
      <td align="center"><strong>López Núñez Sergio Jair</strong></td>
    </tr>
    <tr>
      <td align="center"><strong>Orozco Mariscal Daniel Alejandro</strong></td>
    </tr>
  </table>
</div>
