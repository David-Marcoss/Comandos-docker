# Docker

O docker é uma ferramenta muito util na construção  de sistemas, pois ele cria um ambiente de desenvolvimento isolado para a aplicação, garantindo consistência em diferentes ambientes, 

## Principais conceitos do docker:

Imagem: Uma imagem é um pacote de software leve, independente e executável que inclui tudo o que é necessário para executar um pedaço de software.

Contêiner: Um contêiner é uma instância em execução de uma imagem Docker. Ele encapsula o aplicativo e suas dependências, executando em um ambiente isolado.

Dockerfile: Um Dockerfile é um script que contém instruções para construir uma imagem Docker. Ele define a imagem base, configura o ambiente e especifica os comandos a serem executados quando o contêiner é iniciado.

Docker Compose: Docker Compose é uma ferramenta para definir e executar aplicativos Docker com vários contêineres. Ele utiliza um arquivo YAML para configurar os serviços, redes e volumes do aplicativo.

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