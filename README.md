# Tema: El Detector Mágico - Caja registradora inteligente en tiempo real con visión por computadora

Este proyecto implementa un sistema de punto de venta (POS) automatizado capaz de reconocer 7 productos de supermercado en tiempo real utilizando cámaras web y Redes Neuronales Convolucionales (CNN) con **Transfer Learning**.

---

## Instrucciones de Ejecución

Este proyecto se encuentra diseñado para ejecutarse de forma sencilla y directa en **Google Colab**, aprovechando su entorno en la nube con soporte de aceleración gráfica (GPU/CPU) y captura de cámara web desde el navegador.

### Opción 1: Ejecución directa en Google Colab (Recomendada)

1. **Apertura del Notebook:**
   * Cargar el archivo `Detector_Supermercado.ipynb` en Google Drive o abrirlo directamente en [Google Colab](https://colab.research.google.com/drive/1dkBr97Y_EAqrSxkCP8gJmnTsNsvuw-0p?usp=sharing).
2. **Carga de los Datos de Entrenamiento:**
   * Verificar que la estructura de carpetas de las 7 clases se encuentre alojada en Google Drive (https://drive.google.com/drive/folders/1W_-IwRmWlyT8vmCjPC_q0miJzHAj8ILT?usp=sharing) o subir las imágenes al almacenamiento temporal del entorno de Colab.
3. **Ejecución del Pipeline Completo:**
   * En el menú superior de Colab, seleccionar la opción **Entorno de ejecución > Ejecutar todas** (`Ctrl + F9`).
4. **Interacción en Tiempo Real:**
   * **Punto de Venta (Gradio):** Acceder a la celda de la interfaz interactiva para realizar pruebas con imágenes o cámara web y generar el ticket acumulativo.
   * **Escáner en VIVO:** En la última celda, otorgar los permisos de acceso a la cámara en el navegador para activar la transmisión en tiempo real. Para finalizar la captura, presionar el botón **🔴 APAGAR CÁMARA** o interrumpir la ejecución de la celda.

---

### Opción 2: Ejecución en Entorno Local (VS Code / Jupyter)

En caso de requerir la ejecución en un entorno local:

1. **Clonación del Repositorio:**
   ```bash
   git clone [https://github.com/pablorgranja-dotcom/caja-registradora-vision-ia/blob/main/README.md](https://github.com/pablorgranja-dotcom/caja-registradora-vision-ia/blob/main/README.md)
   cd caja-registradora-vision-ia

## Instalación de Dependencias:
install tensorflow opencv-python numpy gradio matplotlib seaborn

## Ejecución del Código:
Abrir Detector_Supermercado.ipynb desde Jupyter Notebook o VS Code y ejecutar las celdas en orden secuencial. 

Características Principales
**Reconocimiento en tiempo real:**
 Detección fotograma a fotograma con superposición de precios, nombre del producto y porcentaje de confianza.
 **Modelo Ligero y Eficiente:** 
 Basado en la arquitectura MobileNetV2 adaptada específicamente para 7 categorías de productos de supermercado.
 **Manejo de Falsos Positivos:** 
 Filtrado lógico por umbral de confianza ($\ge 60\%$) para mantener la pantalla limpia cuando no hay productos frente a la cámara.
 
 ## Categorías y Precios
 Producto            Precio ($)
 Alimento para Gato  $1.25
 Arena para Gato     $3.00
 Shampoo             $4.50
 Peluche Garfield    $3.50
 Vaso de Vidrio      $2.10
 Libro               $15.00
 Zapato              $20.00 
 
 ## Tecnologías Utilizadas
 * Lenguaje: Python 3
 * Framework de Deep Learning: TensorFlow / Keras
 * Arquitectura: MobileNetV2 (Transfer Learning)
 * Procesamiento de Video e Imágenes: OpenCV / PIL
 * Despliegue Web: Gradio
 * Análisis de Datos: NumPy, Matplotlib, Seaborn 
 
 ## Dataset
 El conjunto de datos contiene fotografías capturadas manualmente y organizadas jerárquicamente por categorías.Acceso al Dataset: Se puede acceder al conjunto de imágenes de entrenamiento a través del siguiente Enlace a Google Drive (https://drive.google.com/drive/folders/1W_-IwRmWlyT8vmCjPC_q0miJzHAj8ILT?usp=drive_link).
