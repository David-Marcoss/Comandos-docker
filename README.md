# Comandos Docker

A seguir estão alguns comandos úteis do Docker, estes comandos ajudarão você a gerenciar suas imagens, containers, volumes e redes no Docker. Adaptar conforme necessário para o seu ambiente e projeto.

## Listar Imagens

```bash
docker images
```

## Criar Imagem a partir de um Dockerfile

```bash
docker build --tag nome-imagem .
```

## Remover Imagem

```bash
docker rmi id-imagem
```

## Executar Imagem

```bash
docker run nome-container
docker run -it nome-container
docker run -d nome-container
```

## Acessar Container em Execução

```bash
docker exec -it id-container bash
```

## Listar Containers em Execução

```bash
docker ps
```

## Listar Todos os Containers

```bash
docker ps -a
```

## Ver Informações do Container

```bash
docker inspect id-container
```

## Remover Container

```bash
docker rm id-container
docker rm id-container --force
```

## Criar Volume (Armazenar dados do container na máquina host)

```bash
docker volume create nome-volume
```

## Remover Volume

```bash
docker volume rm id-volume
```

## Criar Rede (Conectar containers)

```bash
docker network create network-name

```

## Remover Rede

```bash
docker network rm id-rede
```