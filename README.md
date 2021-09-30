# Ansible_Docker
Automatização de Script para configurar o ambiente e instalar a ferramenta Docker

---
- hosts: {Altere e coloque o nome do grupo de hosts}
  remote_user: {Usuário para efetuar a comunicação e executar os scripts}
  roles:
    - Docker
    - Portainer


Hosts: Neste campo coloque o nome do grupo que você definiu no arquivo de configuração host.yml
remote_user: Usuário cadastrado na máquina destino para efetuar a comunicação e execução dos scripts.
roles: 
  {Logo abaixo desse campo seguido - , informe o nome das regras que será acionada. 
  
  
