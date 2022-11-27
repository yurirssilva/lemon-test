# Índice - Teste Lemon Shortlinks
* [Infraestrutura de Nuvem](#Infraestrutura-de-Nuvem)
* [Custos - Infra AWS](#Custos-Infra-AWS)
* [Camadas de Código](#Camadas-de-Codigo)
* [Estrutura de Dados](#Estrutura-de-Dados)

# Infraestrutura de Nuvem
![Diagrama - AWS Infra](https://user-images.githubusercontent.com/5217635/204121771-cdc4f0ce-6f1a-47db-8923-646794b0fc1f.png)

# Custos - Infra AWS
## Custos Lambda

Duration	| Requests | Memory	| Total Compute	| Compute Charges	| Total Compute * Charges	| Charge/Request	| Charge/Request * Requests 	| Total Cost
--- | --- | --- | --- | --- | --- | --- | --- | ---
0,5s	| 102010	| 512 MB	| 25502,50 GB	| $0,0000166667	| $0,4250425168	| $0,0000002	| $0,020402	| $0,4454445168

## Custos DynamoDB

Writes	| Reads	| Write Cost (1,25 / 1M)	| Total Write Cost	| Read Cost (0,25 / 1M)	| Total Read Cost	| Total Cost
--- | --- | --- | --- | --- | --- | ---
102010	| 101000	| $0,00000125	| $0,1275125	| $0,00000025	| $0,02525	| $0,1527625

## Custos API Gateway

Public Requests	| Total Cost
--- | ---
100000	| $1,00

## Custos Totais

Serviço | Valor
--- | ---
Lambda	| $0,4454445168
DynamoDB	| $0,1527625
API Gateway	| $1
Custo Total	| $1,598207017

# Camadas de Código
## Diagrama de Sequência
![image](https://user-images.githubusercontent.com/5217635/204122671-546cea2a-7216-4339-85e4-6c437a28efd7.png)

## Diagramas de Sequência - Lambdas
LambdaGet

![image](https://user-images.githubusercontent.com/5217635/204122693-4562be3c-4c00-445c-a0f8-c9d2b8267489.png)

## LambdaPost

![image](https://user-images.githubusercontent.com/5217635/204122705-67f6693c-8629-4586-8706-7a298c61b6c3.png)

## LambdaPut

![image](https://user-images.githubusercontent.com/5217635/204122713-49b37f3a-55aa-4316-8bd5-bed1e982a636.png)

## LambdaGetMetrics

![image](https://user-images.githubusercontent.com/5217635/204122719-b8add165-6f1b-4a39-9ec8-b01f21790376.png)

# Estrutura de Dados
