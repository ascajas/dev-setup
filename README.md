# Dev-Setup

A idéia do dev-setup é que o desenvolvedor possa testar os serviços via **docker** com apenas um comando.

A exclusão dos serviços seguem a mesma idéia removendo com um único comando inclusive os volumes docker onde eventuais dados estejam armazenados.

Quando um comando é executado ele remove qualquer container, e seus volumes, que por ventura exista relacionado a ele e que tenha subido em uma execução anterior do comando. Portanto não é recomendado o uso em produção pois há risco de perda de dados.
***

## Binários disponíveis  
***
> ### Elasticsearch
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 2.5G
> #### *Acesso local* 
> - http://localhost:9200
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/elasticsearch | sudo bash ```
***

> ### Git-init
> #### *Observações*
> - Inicia o git com as configurações de nome, email e armazenamento de senha em cache permanente.
> #### *Comando para iniciar* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/git-init | sudo bash ```
***

> ### Install-php
> #### *Observações*
> - Instala o php + extensões + composer + symfony
> #### *Comando para instalar* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/install-php | sudo bash ```
***

> ### kafka
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 400M
> - Dependente do Zookeeper, portando inicie o Zookeeper primeiro.
> #### *Acesso local* 
> - http://localhost:9092
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kafka | sudo bash ```
***

> ### kibana
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 320M
> - Dependente do Elasticsearch, portanto inicie o Elasticsearch primeiro.
> #### *Acesso local* 
> - http://localhost:5601
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kibana | sudo bash ```
***

> ### Nifi
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 1.5G
> #### *Acesso local* 
> - https://localhost:8443
> - Usuário: admin  
> - Senha: 123456789012  
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/nifi | sudo bash ```
***

> ### Pihole
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 90M
> #### *Acesso local* 
> - http://localhost:8020/admin
> - Usuário: admin  
> - Senha: 123456  
> - Porta de serviço: 531
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/pihole | sudo bash ```
***
> ### Portainer
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 12M
> #### *Acesso local* 
> - https://localhost:9443
> - Usuário: admin  
> - Senha: 123456789012  
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/portainer | sudo bash ```
***
> ### Rabbitmq
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 170M
> #### *Acesso local* 
> - http://localhost:15672  
> - Usuário: guest  
> - Senha: guest  
> - Porta de serviço: 5672
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/rabbitmq | sudo bash ```
***
> ### Update-Linux
> #### *Observações*
> - Atualização do linux debian/ubuntu para quem esta tendo problemas na sua atualização automática e erros na snap-store. 
> #### *Comando para atualizar* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/update-linux | sudo bash ```
***
> ### Zookeeper
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 180M
> #### *Comando para subir* 
> ``` curl https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/zookeeper | sudo bash ```
***