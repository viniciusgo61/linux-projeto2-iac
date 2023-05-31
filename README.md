# DIO Bootcamp Linux & AWS

## 💻 Projeto 2
Neste projeto iremos criar um script onde será provisionado um servidor web automaticamente. Um servidor web é um software e hardware que usa HTTP (Hypertext Transfer Protocol) e 
outros protocolos para responder a solicitações de clientes feitas pela World Wide Web.
O principal trabalho de um servidor da web é exibir o conteúdo do site por meio do armazenamento, processamento e entrega de páginas da web aos usuários.
## Pré-requisitos:

Linux e GitHub;

## Definições 

Para o projeto iremos restaurar o snapshot criado anteriormente no virtualbox, atualizar o servidor,instalar o apache2,instalar o unzip,baixar a aplicação disponivel no endereço
da DIO e baixar ele no diretório /tmp.Depois iremos copiar os arquivos da aplicação no diretório padrão do apache e subir o arquivo de script para o repositório do GITHUB.

## Passo a Passo 


# apos restaurar o snapshot, logar como root  e por a senha

ip a →192.168.10.13

Abrindo o putty

logando como root,

criamos um diretorio mkdir /scripts2

cd /scripts2/

nano script-iac2.sh

# no nano


![image](https://github.com/viniciusgo61/linux-projeto2-iac/assets/69882802/982281a1-e526-4d16-ab94-0b22a8d52ea6)
lembrando q em cd linux-site-dion-main (devemos alterar isso)

dps ctrl + o e dps ctrl + x

dps escrevemos chmod +x script-iac2.sh para dar permissao de execucao do arquivo

dps é so executar ./script-iac2.sh

após executar,nos testamos em

cd /var/html/

ls

vemos q o arquivo foi baixado e descompatado, digitamos o valor de IP no computador e pronto

por ultimo subimos o arquivo para o github

echo "# linux-projeto2-iac" >> http://README.md
git init
git add http://README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/viniciusgo61/linux-projeto2-iac.git “https://github.com/viniciusgo61/linux-projeto2-iac.git"
git push -u origin main

<hr/>
