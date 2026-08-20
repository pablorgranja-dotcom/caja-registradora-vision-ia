# Tema: El Detector Mágico - Caja registradora inteligente en tiempo real con visión por computadora

Este proyecto implementa un sistema de punto de venta (POS) automatizado capaz de reconocer 7 productos de supermercado en tiempo real utilizando cámaras web y Redes Neuronales Convolucionales (CNN) con **Transfer Learning**.

## Instrucciones de Ejecución

Este proyecto se encuentra diseñado para ejecutarse de forma sencilla y directa en **Google Colab**, aprovechando su entorno en la nube con soporte de GPU/CPU y captura de webcam en el navegador.

### Opción 1: Ejecución directa en Google Colab (Recomendada)

1. **Abrir el Notebook:**
   * Sube el archivo `Detector_Supermercado.ipynb` a tu Google Drive o ábrelo directamente en [Google Colab](https://colab.research.google.com/).
2. **Cargar los datos de entrenamiento:**
   * Asegúrate de tener la estructura de carpetas de las 7 clases cargada en tu Google Drive o sube las imágenes en el entorno temporal de Colab.
3. **Ejecutar el pipeline completo:**
   * En el menú superior de Colab, selecciona **Entorno de ejecución > Ejecutar todas** (`Ctrl + F9`).
4. **Interacción en tiempo real:**
   * **Punto de Venta (Gradio):** Ve a la celda de la interfaz interactiva para probar el escáner con imágenes o cámara web y generar el ticket acumulativo.
   * **Escáner en VIVO:** En la última celda, otorga permisos de cámara a tu navegador para activar la transmisión en tiempo real. Para finalizar, presiona el botón **🔴 APAGAR CÁMARA** o detén la ejecución de la celda.

---

### Opción 2: Ejecución en Entorno Local (VS Code / Jupyter)

 Si prefieres ejecutar el proyecto localmente en tu computadora:

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/TU_USUARIO/caja-registradora-vision-ia.git](https://github.com/TU_USUARIO/caja-registradora-vision-ia.git)
   cd caja-registradora-vision-ia

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
* *Nota:* Puede acceder al conjunto de imágenes de entrenamiento en este [Enlace a Google Drive](https://drive.google.com/drive/folders/1W_-IwRmWlyT8vmCjPC_q0miJzHAj8ILT?usp=sharing).
