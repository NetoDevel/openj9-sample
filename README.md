# openj9-sample
Exemplo utilizando openjdk e openj9



### Passos para executar

```
mvn clean install
docker-compose build
docker-compose up
```

### Comando para monitorar recursos do container

```
docker stats --no-stream --format "table {{.Container}}\t{{.Name}}\t{{.CPUPerc}}\t{{.MemUsage}}"
```


### Tabela de resultado 

```
CONTAINER           NAME                CPU %               MEM USAGE / LIMIT
a99f82eb3a3a        demo_app-jdk_1      0.10%               210.5MiB / 1.934GiB
188a58b82501        demo_app-openj9_1   0.10%               62.6MiB / 1.934GiB
```
