# Packer + Ansible + Nginx

Utilizando o software Packer com provisionador Ansible para instalar o NGINX no GCP

## Instalação

Faça a instalação do Packer e Ansible
Packer:
https://www.packer.io/downloads/
Ansible:
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

Para utilizar o Ansible e o GCP deve instalar o pacote do python google-auth
```bash
pip install google-auth
```

## Uso

```bash
#Crie uma pasta para inserir a aplicação
mkdir packer
#Faça o clone da aplicação
git clone https://github.com/matheusmgon/packer-ansible-Nginx packer
#Acesse a pasta
cd packer
#Para iniciar o packer, utilize o comando:
packer build -machine-readable criar-imagem.json
```

