# Caja Registradora Inteligente con Visión por Computadora

Este proyecto implementa un sistema de punto de venta (POS) automatizado capaz de reconocer 7 productos de supermercado en tiempo real utilizando cámaras web y Redes Neuronales Convolucionales (CNN) con **Transfer Learning**.

## Demostración
*(Inserta aquí un GIF o captura de la pantalla del escáner en vivo y la interfaz de Gradio)*

## Características
* **Reconocimiento en tiempo real:** Detección frame por frame con superposición de precios y porcentaje de confianza.
* **Modelo Ligero:** Basado en **MobileNetV2** adaptado para 7 categorías de productos.

## Categorías y Precios
| Producto           | Precio ($) |
| :---               | :---       |
| Alimento para Gato | $1.25      |
| Arena para Gato    | $3.00      |
| Shampoo            | $4.50      |
| Peluche Garfield   | $3.50      |
| Vaso de Vidrio     | $2.10      |
| Libro              | $15.00     |
| Zapato             | $20.00     |

## 🛠️ Tecnologías Utilizadas
* Python 3
* TensorFlow / Keras
* MobileNetV2 (Transfer Learning)
* OpenCV
* Gradio

## Dataset
El dataset contiene fotografías tomadas manualmente organizadas por categorías. 
* *Nota:* Puede acceder al conjunto de imágenes de entrenamiento en este [Enlace a Google Drive](https://drive.google.com/drive/folders/1W_-IwRmWlyT8vmCjPC_q0miJzHAj8ILT?usp=drive_link).