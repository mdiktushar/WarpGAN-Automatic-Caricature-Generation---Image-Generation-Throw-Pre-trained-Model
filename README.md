# WarpGAN-Automatic-Caricature-Generation---Image-Generation-Through-Pre-trained-Model

WarpGAN is a deep learning model that transforms real face images into caricature-style outputs. It combines texture stylization with geometric warping to exaggerate facial features, producing expressive cartoon-like results. The model can generate multiple variations from a single input using different style samples.

---

## 📥 Pre-trained Model Download

Download the pre-trained model weights from the links below:

- 🔗 Google Drive: [Generator](https://drive.google.com/file/d/1XwjMGcYIg2qwEKHsC7uSmZayHvnEFhyg/view)
- 🔗 Google Drive: [Discriminator](https://drive.google.com/file/d/1hcxr7yCiS8om59deMrRXFBYNJSrKtqNT/view)

> 📌 After downloading, place the model files inside the `models/` directory.

---

## ⚙️ Environment Setup

### Create environment
```
conda create -n warpgan_tf1 python=3.7 -y
```

### Activate environment
```
conda activate warpgan_tf1
```

### Upgrade pip
```
python -m pip install --upgrade pip
```

### Install CUDA + cuDNN (inside Conda)
```
conda install -c conda-forge cudatoolkit=10.0 cudnn=7.6.5 -y
```

### Install TensorFlow (GPU)
```
pip install tensorflow-gpu==1.15.0
```

### Install dependencies
```
pip install opencv-python pillow scipy tqdm imageio matplotlib
```

### (Optional) Install project requirements
```
pip install -r requirements.txt
```

### Install Jupyter Notebook + kernel
```
conda install notebook ipykernel -y
```

### Register kernel
```
python -m ipykernel install --user --name warpgan_tf1 --display-name "Python (warpgan_tf1)"
```

### Verify TensorFlow + GPU
```
python -c "import tensorflow as tf; print(tf.__version__); print(tf.test.is_gpu_available())"
```
