![CleanOceanicGreenBlue](https://github.com/CleanOceanic/disruptive_architectures/assets/80494196/65e0a5d3-30b6-4802-8d6a-4a199cd8c5c7)

## Introdução

Este projeto oferece uma solução baseada em IA para ajudar a limpar os oceanos, identificando e categorizando vários tipos de resíduos usando visão computacional. O projeto inclui uma API para processar imagens e uma interface front-end para interação do usuário.

## Integrantes do Grupo

- Kaique Santos de Andrade - RM99562
- Marcelo Augusto de Mello Paixão - RM99466
- Rodrigo Batista Freire - RM99513
- Thiago Martins Bezerra - RM98644
- Vinicius Oliveira de Almeida - RM97967
#

## Construir e Enviar Imagens Docker

### Imagem Docker da API
- Nome da Imagem: marceloamellopaixao/cleanoceanic-cv_api:latest
- URL do Dockerhub: cleanoceanic-cv_api

```bash
  docker build -t marceloamellopaixao/cleanoceanic-cv_api:latest .
  docker login
  docker push marceloamellopaixao/cleanoceanic-cv_api:latest
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

### 4º - Abra no seu navegador a url: 

```bash
  localhost:5173
```

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
