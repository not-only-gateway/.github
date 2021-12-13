# API gateway

### Objetivos
- Facilitar o gerênciamento de multiplos serviços
> Com o aumento da complexidade de sistemas de grande porte surge a necessidade de uma plataforma para o gerênciamento centralizado desses serviços.
>
> Estes serviços tem como objetivo fornecer uma arquitetura flexível e facil de implementar dentro do seu ambiente de trabalho.

### Features 
- API Gateway.
- Loadbalance.
- Escalabilidade.
- Históricode transções e atividades .
- Análise de dados.
- Análise de performace.

### Dependências 
- **Python** - Linguagem *backend*.
  - Flask
  - SQLalchemy
  - pika
- **RabbitMQ** - Message-broker.
- **NextJS** - Framework *frontend*.

### Padrões
- APIs Restful.
- Micro-serviços
  - [CQRS](https://microservices.io/patterns/data/cqrs.html)
  
### Topologia dos serviços

- **gateway** - Protal de tratamento dos requests.
- **statistics** - Histórico de transações das APIs, análise dos dados e gestor do *loadbalance*.
- **data-buffer** - Registro dos dados das transações / Histórico e rascunhos
- **service** - Service - Gerênciamento de serviços, instancias etc.

