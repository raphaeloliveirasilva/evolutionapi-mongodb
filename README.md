# Evolution API + MongoDB
Evolution is an Open Source API for sending Whatsapp messages.


### pré-requisito

*instale o docker e docker compose na vps e crie duas networks chamadas nginx e evolutionapi*
 ```sh
   docker network create nginx
   ```
 ```sh
   docker network create evolutionapi
   ```
*instale o nginx proxy manager*
   ```sh
   mkdir nginx && cd nginx
   ```
   ```sh
   git clone https://github.com/raphaeloliveirasilva/nginxproxyreverse.git
   ```
   ```sh
   docker-compose up -d
   ```

### instalação da api + mongodb
*vá para a pasta home do seu usuário ou para a pasta de sua preferência e crie um diretório chamado evolutionapi-mongodb*
```sh
   mkdir evolutionapi-mongodb && cd evolutionapi-mongodb
   ```
*faça o clone do repositório abaixo*
```sh
   git clone https://github.com/raphaeloliveirasilva/evolutionapi-mongodb.git
   ```
*altere seu SERVER_URL e sua AUTHENTICATION_API_KEY no arquivo .env e crie os container com o comando abaixo*

```sh
   docker-compose up -d
   ```
### criando o proxy reverse com nginx proxy manager
*digite no seu navegador http://seuip:81*


