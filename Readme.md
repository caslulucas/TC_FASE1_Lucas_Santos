# Tech Challenge – Fase 1 - Postech FIAP - DevOps & Arquitetura Cloud
## Projeto: ToggleMaster (Feature Flag as a Service)

Este repositório contém a entrega da **Fase 1 do Tech Challenge**, cujo objetivo é executar, analisar e implantar um **MVP monolítico** da aplicação **ToggleMaster**, aplicando conceitos de **Cultura DevOps**, **Arquitetura de Aplicações** e **Cloud Computing na AWS**.

---

## 📌 Visão Geral do Projeto

O **ToggleMaster** é uma API REST responsável por gerenciar *feature flags*, permitindo ativar ou desativar funcionalidades dinamicamente, sem a necessidade de realizar um novo deploy da aplicação cliente.

Nesta fase do projeto, a aplicação é mantida como **monolítica**, priorizando simplicidade, baixo custo e rapidez de entrega, características adequadas para um MVP.

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Flask  
- Docker  
- Docker Compose  
- PostgreSQL  
- AWS EC2  
- AWS RDS  
- AWS VPC  
- Git e GitHub 
- Linux Ubuntu  

---

## 🔗 Código-base Utilizado

Este projeto foi desenvolvido utilizando como base o repositório fornecido para o Tech Challenge:

👉 **Repositório do código-base:**  
    https://github.com/dougls/toggle-master-monolith

---

## ▶️ Execução Local da Aplicação

A aplicação pode ser executada localmente por meio do Docker Compose:

```bash
docker-compose up --build 
```

Após a inicialização, o funcionamento pode ser validado através do endpoint de health check:

http://localhost:5000/health


## ☁️ Arquitetura na AWS
A arquitetura proposta para a aplicação ToggleMaster na AWS segue boas práticas de segurança, isolamento de rede e alta disponibilidade, incluindo:

- VPC dedicada
- Sub-redes públicas e privadas
- Instâncias EC2 para execução da API
- Banco de dados RDS PostgreSQL em sub-rede privada
- Internet Gateway
- NAT Gateway
- Application Load Balancer

Essa arquitetura garante isolamento do banco de dados, acesso controlado à aplicação e preparação para escalabilidade futura.


## 🖼️ Diagrama de Arquitetura
🔗 Link do diagrama (Miro):
https://miro.com/app/board/uXjVGqtu7ks=/


## 🎥 Vídeo de Demonstração
O vídeo de demonstração apresenta:

- Execução local da aplicação
- Explicação da arquitetura
- Aplicação rodando na AWS
- Demonstração das feature flags
- Discussão sobre os princípios do 12-Factor App

👉 Link do vídeo:
INSERIR AQUI O LINK DO VÍDEO (YouTube ou Google Drive)


## ⚠️ Desafios e Decisões Tomadas
Os principais desafios enfrentados durante o Tech Challenge foram:

- Compreensão da arquitetura monolítica da aplicação
- Configuração correta de variáveis de ambiente
- Definição de uma arquitetura segura na AWS

Optou-se por manter a arquitetura monolítica nesta fase por se tratar de um MVP, priorizando simplicidade, velocidade de entrega e validação do modelo de negócio.


## 👥 Participantes

Lucas Soares do Santos 