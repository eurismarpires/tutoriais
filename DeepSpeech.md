Como Preparar o Ambiente para Rodar o Mozzila/DeepSpeech
---------

### Instalando o Anaconda

    $ wget https://repo.continuum.io/archive/Anaconda3-4.3.0-Linux-x86_64.sh
    $ bash Anaconda3-4.3.0-Linux-x86_64.sh        

<span>

    $ export PATH=$PATH:/home/eurismar/anaconda3/bin	

### Ambiente Conda

    $ conda create -n eurismar python=2.7
    $ source activate eurismar

### TensorFlow
    $ export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-0.12.1-cp27-none-linux_x86_64.whl
    $ pip install --ignore-installed --upgrade $TF_BINARY_URL

### pyxdg
    $ pip install pyxdg
### scipy
    $ pip install scipy
### python_speech_features
    $ wget https://pypi.python.org/packages/fa/3e/f583bc2702caf615fdf00c8eab3334023438d627d4c7e6bcceda429a6811/python_speech_features-0.5.tar.gz#md5=c989f7badfe50f2949464265546566ed
    $ tar -zxvf python_speech_features-0.5.tar.gz 
    $ cd python_speech_features-0.5
    $ python setup.py install

### paramiko
    $ pip install paramiko
### pysftp
    $ pip install pysftp
### bs4
    $ pip install bs4
```
