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

![imagen de entrada](https://github.com/user-attachments/assets/9dcf59cd-8f90-4fd7-818f-efe29db39466)


Salida:

imagen restaurada con detalles faciales reconstruidos por el modelo GFPGAN.
![imagen de salida](https://github.com/user-attachments/assets/6556dd50-2ff3-49c5-8968-c3e6e3f7c91c)


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
```

## 2. Instalar PyTorch con CUDA

Ejemplo para CUDA 11.8:
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

## 3. Abrir el notebook
```
jupyter notebook
DL02_FaceRestoration_local_anaconda_updated.ipynb
```

## 4. Ejecutar las celdas en orden

El notebook realiza:
Diagnóstico del entorno
Configuración de rutas
Clonado de GFPGAN
Instalación de dependencias
Descarga de pesos del modelo
Restauración de imágenes

# Cómo restaurar una imagen

1. Coloca la imagen en:
```
GFPGAN/inputs/user_images/
```
2. Ejecuta la celda de inferencia.

3. El resultado aparecerá en:
```
GFPGAN/results_local/
```

# Créditos
Este proyecto utiliza el modelo GFPGAN desarrollado por Tencent ARC.
Repositorio original:
https://github.com/TencentARC/GFPGAN

# Licencia
Este proyecto se distribuye únicamente con fines educativos y de investigación.
Revisar la licencia oficial del repositorio de GFPGAN para uso comercial.

