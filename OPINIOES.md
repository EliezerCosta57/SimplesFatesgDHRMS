# OPINIOES

## i. Qual tecnologia de comunicação o servidor de cálculo utiliza?

O servidor de cálculo utiliza comunicação via Socket TCP/IP para troca de mensagens entre aplicações distribuídas.

---

## ii. Qual protocolo de mensagem o servidor de cálculo utiliza?

O servidor de cálculo utiliza o protocolo JSON-RPC para envio e recebimento das mensagens entre cliente e servidor.

---

## iii. Qual tecnologia de comunicação o servidor de dados utiliza?

O servidor de dados utiliza Java RMI (Remote Method Invocation), permitindo chamadas remotas de métodos entre aplicações Java distribuídas.

---

## iv. Qual estilo arquitetural o projeto web_api implementou para expor suas funcionalidades?

O projeto web_api implementou o estilo arquitetural REST API, expondo endpoints HTTP para acesso aos serviços distribuídos do sistema.

---

## v. Arquitetura do sistema

A arquitetura do sistema é composta pelos seguintes componentes:

- web_api
- servidor_de_dados
- servidor_de_calculos
- MySQL Server

Relacionamentos:

- web_api consome servidor_de_dados via RMI
- web_api consome servidor_de_calculos via Socket TCP/IP + JSON-RPC
- servidor_de_dados acessa MySQL
- servidor_de_calculos consome servidor_de_dados