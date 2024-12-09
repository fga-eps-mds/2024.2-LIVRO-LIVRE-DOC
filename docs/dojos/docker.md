# Guia Completo de Docker e Docker-Compose

## Versão

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| Dojo Docker    | Subindo documento versão 1                    | Mateus Maia | 09 de dezembro de 2024 |

## Docker

### O que é Docker?
O Docker é uma plataforma de software que permite criar e gerenciar contêineres: ambientes isolados e portáteis para rodar aplicações. Isso facilita o desenvolvimento, a distribuição e a execução de aplicações em diferentes ambientes.

### Guia de Instalação
* **Linux:**
    ```bash
    # Instalação Ubuntu/Debian
    sudo apt-get update
    sudo apt-get install docker.io

    # Instalação CentOS/Fedora
    sudo yum install docker-ce docker-ce-cli containerd.io
    ```
* **macOS:**
    * Instalar o Docker Desktop para Mac através do site oficial.
* **Windows:**
    * Instalar o Docker Desktop para Windows através do site oficial.

### Dockerfile
Um Dockerfile é um arquivo de texto que contém todas as instruções para criar uma imagem Docker. Ele define a base da imagem, os comandos a serem executados e os arquivos que serão copiados para a imagem.
* **Exemplo básico:**
    ```dockerfile
    FROM ubuntu:latest
    RUN apt-get update && apt-get install -y nginx
    EXPOSE 80
    CMD ["nginx", "-g", "daemon off;"]
    ```

### Comandos Básicos
* **`docker run`:** Executa um container a partir de uma imagem.
* **`docker ps`:** Lista os containers em execução.
* **`docker images`:** Lista as imagens disponíveis localmente.
* **`docker stop`:** Para um container em execução.
* **`docker rm`:** Remove um container.
* **`docker build`:** Cria uma imagem a partir de um Dockerfile.

## Docker-Compose

### O que é Docker-Compose?
O Docker Compose é uma ferramenta para definir e executar aplicações Docker multi-container usando um arquivo YAML. Ele facilita a criação de ambientes complexos com múltiplos serviços.

### Guia de Instalação
* **Instalação:**
    ```bash
    sudo curl -L "[https://github.com/docker/compose/releases/download/1.29.2/docker-compose-linux-x86_64](https://github.com/docker/compose/releases/download/1.29.2/docker-compose-linux-x86_64)" -o /usr/local/bin/docker-compose
    sudo chmod +x /usr/local/bin/docker-compose
    ```

### Comandos Básicos
* **`docker-compose up`:** Inicia os serviços definidos no arquivo docker-compose.yml.
* **`docker-compose down`:** Para e remove os containers e redes criados.
* **`docker-compose build`:** Reconstrói as imagens dos serviços.

**docker-compose.yml:**
```yaml
version: '3.7'
services:
  web:
    build: .
    ports:
      - "5000:5000"