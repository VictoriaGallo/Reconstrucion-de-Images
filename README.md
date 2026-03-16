# Face Restoration con GFPGAN (Local)

Proyecto para restauración de rostros usando **GFPGAN** ejecutado localmente mediante **Anaconda + Jupyter Notebook**.  
Permite mejorar fotos antiguas, borrosas o de baja resolución utilizando modelos de deep learning.

El notebook automatiza:

- Verificación del entorno (Python, Torch, CUDA, GPU)
- Configuración de rutas del proyecto
- Instalación de dependencias
- Clonado del repositorio GFPGAN
- Descarga de pesos del modelo
- Restauración de imágenes
- Visualización antes/después

---

# Ejemplo

Entrada:

imagen con rostro degradado o borroso.

Salida:

imagen restaurada con detalles faciales reconstruidos por el modelo GFPGAN.

---

# Requisitos

Recomendado:

- Python 3.10
- GPU NVIDIA (opcional pero recomendado)
- CUDA compatible con PyTorch
- Anaconda o Miniconda
- Jupyter Notebook o JupyterLab

Dependencias principales:

- torch
- torchvision
- basicsr
- facexlib
- realesrgan
- opencv
- numpy

---

# Instalación

## 1. Crear entorno con Anaconda

```bash
conda create -n gfpgan python=3.10
conda activate gfpgan
