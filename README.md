# a443-MLOps
Ini adalah repositori untuk latihan pada kelas Machine Learning Operations (MLOps)

## Machine Learning Pipeline 

I'm using Python 3.10.5

Build virtual env and install library

```bash
python -m venv nama_env

pip install -r requirements.txt
```

Activate and use it

```bash
nama_env\Scripts\activate
```

## Model Serving use Flask

```bash
set FLASK_APP=main.py

flask run
```

## TF-Serving Deployment use Docker

Membuat docker image 

```bash
docker build -t fashion-mnist-tf-serving .
```

Menjelankan docker image dan menentukan port. Ingat bahwa di dalam docker container TF Serving menggunakan port 8501.

```bash
docker run -p 8080:8501 fashion-mnist-tf-serving
```
