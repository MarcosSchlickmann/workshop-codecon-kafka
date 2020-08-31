# Workshop: Event-driven architecture with Kafka

## Dependências

Os exemplos de código desse repositório dependem  do OpenJDK 11 e
os serviços que precisamos executar do Docker.

* [OpenJDK 11](https://adoptopenjdk.net/installation.html#x64_linux-jdk)
* [Docker](https://docs.docker.com/get-docker/)

## Configuração

```sh
git clone git@github.com:magrathealabs/workshop-codecon-kafka.git
cd workshop-codecon-kafka
```

## Executando serviços

Inicie os serviços executando no terminal:

```sh
docker-compose up -d
```

Para finalizar os serviços, vá para janelas abertas com instâncias de producers, consumers ou shells e aperte `CTRL+C` e finalize os containers com `CTRL+D`. Finalize então a stack de serviços executando:

```sh
docker-compose down
```

## Exemplos

1. [Introdução ao Kafka](./kafka-introduction/README.md)
2. [Escrevendo Produtores e Consumidores](./kafka-consumer-producer-application/README.md)

## Comandos básicos

Para fechar o console do consumer e producer do Kafka use `CTRL+C`.

Para fechar o shell do container do Docker use `CTRL+D`.

Para iniciar uma sessão bash no broker do Kafka digite:

```sh
docker-compose exec broker bash
```
