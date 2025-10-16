# PREMISSAS

## SISTEMAS A SEREM DESENVOLVIDOS

### Login System

### Data
1. Email/Password

## UseCase
1. Recebemos os dados pelo body de um requisição HTTP
 - Endpoint '/login' - Requisição HTTP POST - Email/Password

2. Validar email = externo

3. Buscar dados no Banco

4. Comparar o password informado com o password cadastrado no banco

5. Retornar o status da operação através da riquisição
 - Se os dados estiverem batendo: retorna status de sucesso e o token de authentication para persistencia do login
 - Se há alguma inconsistencia: retorna status de error (email ou senha incorretos) 

- Buscar dados no DB utilizando o email