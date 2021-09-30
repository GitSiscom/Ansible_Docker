# Ansible_Docker
Script de automação no Ansible

Objetivo: Configurar um ambiente novo Linux (CentOS), instalando as ferramentas necessárias para atuação diárias. 
          Implementado código para instalar o Docker e a ferramenta de gerenciamento de containers Web.

---
- hosts: 
     {Altere e coloque o nome do grupo de hosts}
  remote_user: 
    {Usuário para efetuar a comunicação e executar os scripts}
  roles:
    - Docker
    - Portainer


Explicação sobre cada item:

Hosts: 
  {Neste campo coloque o nome do grupo que você definiu no arquivo de configuração host.yml}
remote_user: 
  {Usuário cadastrado na máquina destino para efetuar a comunicação e execução dos scripts}
roles: 
  {Logo abaixo desse campo seguido - , informe o nome das regras que será acionada. 
  
  
