
# Ansible_Docker
Script de automação no Ansible

Objetivo: 

Configurar um ambiente novo Linux (CentOS), instalando as ferramentas necessárias para atuação diárias. 

Implementado código para instalar o Docker e a ferramenta de gerenciamento de containers Web.

# Código 
---
- hosts: 
     {Altere e coloque o nome do grupo de hosts}
		 
  remote_user: 
					{Usuário para efetuar a comunicação e executar os scripts}
		
  roles:
    - Docker
    - Portainer

---
Explicação sobre cada item:

- Hosts: 
	
  Neste campo coloque o nome do grupo que você definiu no arquivo de configuração host.yml
	
- remote_user: 

  Usuário cadastrado na máquina destino para efetuar a comunicação e execução dos scripts
	
- roles: 

  Logo abaixo desse campo seguido - informe o nome das regras que será acionada. 
  
# Etapa de instalação  
---  

1º Passo

- Copie o link do repositório no seu Git Hub

2º Passo

- Dentro do servidor onde está instalado o Ansible, rode o comando: git clone {LINK DO REPOSITÓRIO COPIADO}

3º Passo

- Rode um comando editor de texto de sua preferência (vim,nano ou vi) e o nome do arquivo docker.yml

4º Passo

- Conforme definido no arquivo hosts.yml, copie o nome do grupo onde você colocou o IP da máquina que deseja realizar essas instalações.
- Coloque o nome do usuário com permissões no visudo para realizar a comunicação entre os servidores via ssh.

######  Preferência não utilize usuário root nesse campo ######

5º Passo

- Depois dessas alterações rode comando para executar a sua playbook

	 Command: ansible-playbook docker.yml 
	
######  Caso queira debugar o arquivo pode rodar conforme abaixo ######	

	Command: ansible-playbook docker.yml -vvv
	
![ansible-playbook](https://user-images.githubusercontent.com/90550531/135503485-ef4e3111-fcc8-434a-bf79-5945027ad803.png)
