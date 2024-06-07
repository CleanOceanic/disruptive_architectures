# Projeto Clean Oceanic CV

## Introdução

Este projeto oferece uma solução baseada em IA para ajudar a limpar os oceanos, identificando e categorizando vários tipos de resíduos usando visão computacional. O projeto inclui uma API para processar imagens e uma interface front-end para interação do usuário.

## Construir e Enviar Imagens Docker

### Imagem Docker da API
- Nome da Imagem: marceloamellopaixao/cleanoceanic-cv_api:latest
- URL do Dockerhub: cleanoceanic-cv_api

```bash
  docker build -t marceloamellopaixao/cleanoceanic-cv_api:latest .
  docker login
  docker push marceloamellopaixao/cleanoceanic-cv_api:latest
```

### Imagem Docker do Front-End
- Nome da Imagem: marceloamellopaixao/cleanoceanic-cv_front:latest
- URL do Dockerhub: cleanoceanic-cv_front

```bash
  docker build -t marceloamellopaixao/cleanoceanic-cv_front:latest .
  docker login
  docker push marceloamellopaixao/cleanoceanic-cv_front:latest
```

# Executando a Aplicação Localmente
## API
### 1º - Baixe a imagem mais recente da API:

```bash
  docker pull marceloamellopaixao/cleanoceanic-cv_api:latest
```

### 2º - Execute o contêiner da API:

```bash
  docker run -d -p 5000:5000 marceloamellopaixao/cleanoceanic-cv_api
```

## Front-End
Você tem duas opções para executar o front-end: usando Docker ou executando localmente.

### 1º - Baixe a imagem mais recente do Front-End:

```bash
  docker pull marceloamellopaixao/cleanoceanic-cv_front:latest
```

### 2º - Execute o contêiner do Front-End:

```bash
  docker run -d -p 8080:8080 marceloamellopaixao/cleanoceanic-cv_front
```

## Executando Localmente

### 1º - Navegue até o diretório do projeto front-end:

```bash
  cd caminho/para/projeto-front-end
```

### 2º - Instale as dependências:

```bash
  npm install
```

### 3º - Inicie o servidor de desenvolvimento:

```bash
  npm start dev
```

### 4º - Abra o seu navegador e acesse: localhost:5173

#

## Usando a Aplicação

### 1º - Abra a aplicação front-end no seu navegador.

### 2º - Faça o upload de uma imagem contendo um dos seguintes tipos de resíduos:
  - Garrafas
  - Tecidos (Roupas, Tênis, etc.)
  - Vidros
  - Latas
  - Plásticos
  - Baterias
### 3º - A aplicação processará a imagem e categorizará o resíduo.
