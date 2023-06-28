# Dev-Setup

A idéia do dev-setup é que o desenvolvedor possa testar os serviços via **docker** com apenas um comando.

A exclusão dos serviços seguem a mesma idéia removendo com um único comando inclusive os volumes docker onde eventuais dados estejam armazenados.

***

## Binários disponíveis  
***
> ### Elasticsearch
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 2.5G
> - Versão: 7.17.10
> #### *Acesso local* 
> - http://localhost:9200
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/elasticsearch \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/elasticsearch \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Git-init
> #### *Observações*
> - Inicia o git com as configurações de nome, email e armazenamento de senha em cache permanente.
> #### *Comando para iniciar* 
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/git-init \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd "Seu nome completo" "seu@email" && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Install-php
> #### *Observações*
> - Instala o php + extensões + composer + symfony
> #### *Comando para instalar* 
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/install-php \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd && \ ```  
> ``` sudo rm ./cmd ```
***

> ### kafka
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 400M
> - Dependente do Zookeeper, portando inicie o Zookeeper primeiro.
> - Versão: 7.3.2
> #### *Acesso local* 
> - http://localhost:9092
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kafka \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kafka \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### kibana
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 320M
> - Dependente do Elasticsearch, portanto inicie o Elasticsearch primeiro.
> - Versão: 7.17.10
> #### *Acesso local* 
> - http://localhost:5601
> - Usuário: <não precisa>  
> - Senha: <não precisa>  
> #### *Comando para subir* 
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kibana \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/kibana \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Mysql
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 400M
> - Versão: latest
> #### *Acesso local* 
> - mysql://localhost:3306
> - Usuário: admin  
> - Senha: admin  
> - Senha de root: root
> - Banco de dados: db
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/mysql \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/mysql \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Nifi
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 1.5G
> - Versão: latest
> #### *Acesso local* 
> - https://localhost:8443
> - Usuário: admin  
> - Senha: 123456789012  
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/nifi \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/nifi \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Pihole
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 90M
> - Versão: latest
> #### *Acesso local* 
> - http://localhost:8020/admin
> - Usuário: admin  
> - Senha: 123456  
> - Porta de serviço: 531
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/pihole \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/pihole \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***
> ### Portainer
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 12M
> - Versão: latest
> #### *Acesso local* 
> - https://localhost:9443
> - Usuário: admin  
> - Senha: 123456789012  
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/portainer \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/portainer \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Postgres
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 35M
> - Versão: latest
> #### *Acesso local* 
> - pgsql://localhost:5432
> - Usuário: postgres  
> - Senha: postgres  
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/postgres \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/postgres \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Rabbitmq
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 170M
> - Versão: 3-management
> #### *Acesso local* 
> - http://localhost:15672  
> - Usuário: guest  
> - Senha: guest  
> - Porta de serviço: 5672
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/rabbitmq \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/rabbitmq \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***
> ### Redis
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 4M
> - Versão: latest
> #### *Acesso local* 
> - Usuário: <não precisa>  
> - Senha: redis  
> - Porta de serviço: 6379
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/redis \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/redis \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***

> ### Update-Linux
> #### *Observações*
> - Atualização do linux debian/ubuntu para quem esta tendo problemas na sua atualização automática e erros na snap-store. 
> #### *Comando para atualizar*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/update-linux \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd && \ ```  
> ``` sudo rm ./cmd ```
***
> ### Zookeeper
> #### *Observações*
> - Consumo mínimo aproximado de memória RAM: 180M
> - Versão=7.3.2
> #### *Comando para subir*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/zookeeper \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd up && \ ```  
> ``` sudo rm ./cmd ```
> #### *Comando para excluir o container e seus volumes*  
> ``` curl \ ```  
> ``` https://raw.githubusercontent.com/ascajas/dev-setup/main/bin/zookeeper \ ```  
> ``` -o cmd && \ ```  
> ``` sudo chmod +x ./cmd && \ ```  
> ``` sudo ./cmd down && \ ```  
> ``` sudo rm ./cmd ```
***
