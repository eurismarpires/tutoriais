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
