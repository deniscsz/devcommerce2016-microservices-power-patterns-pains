[DEVCOMMERCE 2016](http://devcommerce2016.imasters.com.br) Microservices - Poderes, padrões e dificuldades
---
por [Marcos Barbero](http://linkedin.com/in/marcosbarbero)

O que são micro-serviços?
---
>In short, the microservice architectural style is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweight mechanisms, often an HTTP resource API. These services are built around business capabilities and independently deployable by fully automated deployment machinery. There is a bare minimum of centralized management of these services, which may be written in different programming languages and use different data storage technologies.
>
>-- James Lewis and Martin Fowler

Pre-requisitos / Desafios
---
  - Edge Services: Micro Proxies and API Gateways
  - Configurações centralizadas
  - Service Discovery & Registration
  - Routing/Load Balacing
  - Fault Tolerance (Circuit Breakers)
  - Monitoring
  - Distributed Tracing
  - Security and Single Sign-On

O que *NÃO* são micro-serviços?
---
Quebrar uma aplicação em vários serviços menores não significa que você esteja em uma arquitetura de micro-serviços. Esse é apenas o primeiro passo.

Welcome to the jungle Pattern
---
![Pattern 01](https://github.com/marcosbarbero/devcommerce2016-microservices-power-patterns-pains/wiki/jungle-pattern-01.png)
  - Segundo cenário
![Pattern 02](https://github.com/marcosbarbero/devcommerce2016-microservices-power-patterns-pains/wiki/jungle-pattern-02.png)

API Gateway Pattern
---
![API Gateway](https://github.com/marcosbarbero/devcommerce2016-microservices-power-patterns-pains/wiki/api-gateway-pattern-01.png)

Configurações
---
Uma das boas praticas fornecidas pelo manifesto [12factor](http://12factor.net/) é a externalização de configurações do build, assim o mesmo build poderá ser promovido qualquer ambiente: Dev, QA, Prod.  
  
Tools:
  - Spring Cloud Config
  - Netflix Archaius
  - Apache Zookeeper
  - HashiCorp Consul
 
![Cloud Bus Flow](https://github.com/marcosbarbero/devcommerce2016-microservices-power-patterns-pains/wiki/cloud-bus-flow.png)  

A sobrevivência não é obrigatória
---
>It is not necessary to change. Survival is not mandatory. -W. Edwards Deming



Links
---
```
{
 "microservices": {
    "definition": "http://martinfowler.com/microservices",
    "trade-offs": "http://martinfowler.com/articles/microservice-trade-offs.html",
    "prerequisites": "http://martinfowler.com/bliki/MicroservicePrerequisites.html"
    "12factor": "http://12factor.net"
  },
 "reference": "https://dzone.com/articles/the-power-patterns-and-pains-of-microservices"
 "email": "marcos.hgb@gmail.com"
 "linkedin": "http://linkedin.com/in/marcosbarbero"
} 
``` 
