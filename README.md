# E-commerce Microservices Hub

Este repositório centraliza a documentação e organização dos microserviços do backend escalável para e-commerce. O projeto é construído utilizando uma arquitetura distribuída, garantindo alta performance, escalabilidade e confiabilidade.

## 🔧 Tecnologias Utilizadas
- **Spring Boot** - Desenvolvimento dos microserviços
- **PostgreSQL** - Banco de dados relacional
- **Redis** - Cache distribuído
- **RabbitMQ** - Mensageria para comunicação assíncrona
- **JWT** - Autenticação segura
- **API Gateway** - Controle de acesso e roteamento
- **Docker** - Containerização dos serviços
- **Kubernetes (futuro)** - Orquestração dos containers

## 🌐 Arquitetura
O sistema segue uma abordagem baseada em microserviços, separados por domínio para garantir manutenção simplificada e escalabilidade. Cada serviço pode ser desenvolvido, implantado e escalado independentemente.

### API Gateway
A API Gateway foi implementada utilizando **Spring Cloud Gateway**, servindo como ponto único de entrada para os microserviços. Ela gerencia o roteamento das requisições, autenticação, e balanceamento de carga, garantindo segurança e eficiência na comunicação entre os serviços.

🔗 Repositório: [API-Gateway](https://github.com/Cavasini/API-Gateway)


### Microserviços
| Microserviço | Repositório |
|--------------|-------------|
| 🛒 **Carrinho de Compras** | [Cart-Microservice](https://github.com/Cavasini/Cart-Microsservice) |
| 👥 **Autenticação e Usuários** | [Authentication-Service](https://github.com/Cavasini/Authentication-Service) |
| 🛍️ **Gerenciamento de Produtos** | _Em breve_ |
| 💳 **Pagamentos** | _Em breve_ |
| 🚳 **Pedidos e Entregas** | _Em breve_ |

## 🛠️ Configuração e Execução
Cada microserviço possui seu próprio repositório com instruções de instalação e execução. Para configurar todo o ecossistema, siga estes passos:

1. Clone os repositórios individuais.
2. Configure as variáveis de ambiente conforme indicado em cada projeto.
3. Utilize `Docker Compose` para rodar os serviços necessários (RabbitMQ, Redis, PostgreSQL, etc.).
4. Inicie os microserviços individualmente com:

   ```bash
   docker-compose up
   mvn spring-boot:run

---
**Observação:** Este repositório serve apenas como centralização da documentação e dos links dos microserviços.
