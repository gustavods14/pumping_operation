# Punto de Operación de un sistema de bombeo

Este proyecto permite analizar y determinar el punto de operación de bombas centrífugas mediante la intersección entre las curvas de la bomba y la curva resistente del sistema.

## Descripción

La herramienta calcula las curvas características del sistema y la bomba basándose en datos del fabricante y en parámetros hidráulicos de la instalación. Además, genera gráficos interactivos para visualizar el punto de operación y otras características del sistema.

## Cómo Usar el Proyecto en Google Colab

Puedes ejecutar este notebook directamente en Google Colab haciendo clic en el siguiente enlace:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-DxvyLmrv3f1iUN1aAobftsUaLin39ZD/view?usp=sharing)

## Cómo Usar

Sigue estos pasos para configurar y ejecutar el proyecto:

### 1. Configura los parámetros iniciales
Edita los valores de las variables directamente en el código o en el entorno interactivo para personalizar tu análisis:
- **Elevación de succión y descarga**: Define las alturas en metros.
- **Longitud y diámetro de la tubería**: Especifica las dimensiones del sistema.
- **Coeficiente de rugosidad**: Utiliza valores típicos como el de Hazen-Williams (C).

### 2. Proporciona los datos del fabricante
Añade los datos de la curva característica de la bomba:
- **Caudales (Qn)**: Lista de valores en litros por segundo (L/s).
- **Alturas de bombeo (Hn)**: Correspondientes alturas de bombeo en metros de columna de agua (mca).
- **Opcional: Eficiencia (nef)**: Si dispones de la curva de eficiencia, introdúcela como porcentaje (%).

### 3. Ejecuta el análisis
Ejecuta el código para:
- Ajustar las curvas características de la bomba.
- Calcular la curva resistente basada en los parámetros de la instalación.
- Determinar el **punto de operación** resolviendo la intersección entre las curvas.

### 4. Visualiza los resultados
El script genera gráficos interactivos que incluyen:
- La curva característica de la bomba.
- La curva resistente del sistema.
- El punto de operación identificado.
- (Opcional) La curva de eficiencia, si se proporciona.

## Requisitos

Para ejecutar este proyecto necesitas instalar las siguientes dependencias:

- Python 3.x
- Librerías:
  - `numpy`
  - `scipy`
  - `plotly`

Puedes instalar las dependencias ejecutando:
```bash
pip install numpy scipy plotly
