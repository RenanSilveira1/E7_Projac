# E7_Projac

# Principais serviços e dependências
1. Config Server
    Porta padrão: 8888
    Descrição: Fornece a configuração centralizada para os outros microserviços.
    Dependências: Spring Cloud Config Server, Git (para armazenar configurações externas).
2. Discovery Server (Eureka)
    Porta padrão: 8761
    Descrição: Registro de serviços (Service Registry) que permite a descoberta de serviços em tempo de execução.
    Dependências: Spring Cloud Netflix Eureka.
3. Customers Service
    Porta padrão: 8081
    Descrição: Gerencia dados dos clientes (proprietários dos pets).
    Dependências: Spring Data JPA, MySQL.
4. Vets Service
    Porta padrão: 8083
    Descrição: Gerencia dados dos veterinários.
    Dependências: Spring Data JPA, MySQL.
5. Visits Service
    Porta padrão: 8082
    Descrição: Gerencia informações sobre as visitas médicas dos pets.  
    Dependências: Spring Data JPA, MySQL.
6. API Gateway
    Porta padrão: 8080
    Descrição: Ponto de entrada único para o cliente, roteia as requisições para os microserviços apropriados.
    Dependências: Spring Cloud Gateway.
7. Tracing Server (Zipkin)
    Porta padrão: 9411
    Descrição: Fornece rastreamento distribuído para monitorar chamadas entre microserviços.
    Dependências: Spring Cloud Sleuth, Zipkin.
8. Grafana e Prometheus
    Portas padrão: Grafana: 3000, Prometheus: 9090
    Descrição: Monitoramento e visualização de métricas de performance.