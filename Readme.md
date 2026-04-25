# Tech Challenge – Fase 1 - Postech FIAP - DevOps & Arquitetura Cloud
## Projeto: ToggleMaster (Feature Flag as a Service)

Este repositório contém a entrega da **Fase 1 do Tech Challenge**, cujo objetivo é executar, analisar e implantar um **MVP monolítico** da aplicação **ToggleMaster**, aplicando conceitos de **Cultura DevOps**, **Arquitetura de Aplicações** e **Cloud Computing na AWS**.

---

## 📌 Visão Geral do Projeto

O **ToggleMaster** é uma API responsável por gerenciar *feature flags*, permitindo ativar ou desativar funcionalidades dinamicamente, sem a necessidade de realizar um novo deploy da aplicação cliente.

Nesta fase do projeto, a aplicação é mantida como **monolítica**, priorizando simplicidade, baixo custo e rapidez de entrega, características adequadas para um MVP.

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Postman
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
- Sub-redes públicas e Sub-redes privadas
- Instâncias EC2 para execução da API
- Banco de dados RDS PostgreSQL em sub-rede privada
- Internet Gateway
- NAT Gateway
- Application Load Balancer
- Auto Scaling

Essa arquitetura garante isolamento do banco de dados, acesso controlado à aplicação e preparação para escalabilidade futura.


## 🖼️ Diagrama de Arquitetura
🔗 Link do diagrama (Miro):
https://miro.com/app/board/uXjVGqtu7ks=/?share_link_id=559977596492

<img width="518" height="358" alt="PrintDiagrama" src="https://github.com/user-attachments/assets/de660ecf-ad82-4976-9539-b71bde75c249" />



## 🎥 Vídeo de Demonstração
O vídeo de demonstração apresenta:

- Execução da aplicação localmente
- Explicação da arquitetura
- Aplicação e arquitetura reduzida rodando na AWS
- Demonstração das feature flags

👉 Link do vídeo:
Explicação do diagrama - https://drive.google.com/file/d/1rkr-TtKCaSTRzxvVXevZVCIifhMew99g/view?usp=sharing
Execução da aplicação localmente - https://drive.google.com/file/d/1McAn4H9ARL89jzKWHGuvZ2iePwYjPGar/view?usp=sharing
Aplicação e arquitetura reduzida rodando na AWS - 

## ⚠️ Desafios e Decisões Tomadas
Os principais desafios enfrentados durante o Tech Challenge foram:

- Compreensão da arquitetura monolítica da aplicação
- Configuração correta de variáveis de ambiente e security groups
- Definição de uma arquitetura segura na AWS


## 👥 Participantes

Lucas Soares do Santos
