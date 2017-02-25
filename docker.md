Docker
---------

### comando sem argumentos para ver as opções disponíveis
    $ docker
### ver versão instalada
    $ docker version    
### Roda um Cria um container
    $ docker run -t -i ubuntu:14.04 /bin/bash
### Listar containers que estão rodando e que não esto rodando
    $ docker ps -l
### Para sair, não use exit. Use ctrl+p+q. O exit sai do container colocando ele em stop.    

### Voltar ao container
    $ docker attach fd05e571c1e2
### Ver a quantidade de coisas adicionadas
    $ docker diff fd05e571c1e2
### Salvar a versão
    $ docker commit fd05e571c1e2 eurismar/ubuntupython:14.04
    
### Referencia:
   -   https://www.ricardomartins.com.br/2014/09/11/docker-tutorial-mao-na-massa/
   
   
  
### Docker NVIDIA(GPU)
    $ sudo nvidia-docker commit -m 'instalado o git' -a 'eurismarpires@gmail.com' d65875fedef5 eurismar/sugartensor:latest-cpu
    $ sudo nvidia-docker run -t -i 3eef40b88a9d
    $ sudo nvidia-docker run -it sugartensor/sugartensor 
    $ sudo nvidia-docker ps
    $ sudo nvidia-docker cp oi.txt 308d6a701a39:/root/sugartensor/example
    $ sudo nvidia-docker attach 308d6a701a39
 - https://github.com/NVIDIA/nvidia-docker

