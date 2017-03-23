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
    $ pip install python_speech_features

### paramiko
    $ pip install paramiko
### pysftp
    $ pip install pysftp
### bs4
    $ pip install bs4
### html5lib
    $ pip install --upgrade html5lib==1.0b8
### Caso ocorra algum erro de SSL em alguns pacotes acima, instalar as bibliotecas abaixo:
    $ sudo apt-get install build-essential libssl-dev libffi-dev python-dev
    $ pip install cryptography
### instalar o git-lfs https://github.com/git-lfs/git-lfs/releases/download/v2.0.1/git-lfs-linux-amd64-2.0.1.tar.gz
    $ tar -zxvf git-lfs-linux-amd64-2.0.1.tar.gz 
    $ cd git-lfs-2.0.1/
    $ sudo ./install.sh 
    $ sudo git lfs install
    $ sudo git lfs update    
    $ git lfs track "*.psd"
    $ sudo git add .gitattribute
    $ #dentro do diretorio DeepSpeech
    $ sudo git lfs fetch
    $ sudo git lfs checkout
    
### instalar o pyaudio
    $ sudo apt-get install python-pyaudio 
    
```
