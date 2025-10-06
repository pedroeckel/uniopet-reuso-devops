# Atividade Prática — API de Produtos Reutilizável

## Objetivo Geral
Desenvolver uma **API simples e modular** em **Express com TypeScript**, aplicando o conceito de **reuso de software** e a **organização em camadas** (modelo, controlador e rota).  
Além disso, você deverá **adicionar e configurar uma biblioteca externa via NPM**, aprendendo na prática como o ecossistema **Node.js** gerencia dependências reutilizáveis.

---

## Contexto

A empresa **Gestão Quanti** deseja criar uma pequena **API para gerenciar produtos e usuários**.  
O objetivo é demonstrar que a estrutura modular criada para usuários pode ser **reutilizada facilmente para outros domínios**, como produtos, sem a necessidade de reescrever código.

Você será responsável por **ampliar o sistema existente**, aplicando boas práticas de modularização e reutilização de componentes.

---

## Requisitos Funcionais

### RF01 — Modelo de Produto
O sistema deve possuir um **modelo de dados** chamado `Product` contendo:
- Um identificador numérico (`id`);
- Um nome (`name`);
- Um preço (`price`).

---

### RF02 — Listagem de Produtos
O sistema deve disponibilizar um **endpoint HTTP GET** que retorne todos os produtos existentes.

---

### RF03 — Detalhamento de Produto
O sistema deve disponibilizar um **endpoint HTTP GET com parâmetro de rota `/products/:id`**, que retorne um produto específico com base em seu identificador.

---

### RF04 — Validação de Produto inexistente
Caso o produto solicitado não exista, a API deve retornar:
```json
{ "message": "Produto não encontrado" }
````

com o **status HTTP 404 (Not Found)**.

---

### RF05 — Integração com o Módulo Existente

O novo módulo de produtos deve **reutilizar a mesma arquitetura** adotada para o módulo de usuários:

* Um **modelo** em `/src/models`
* Um **controller** em `/src/controllers`
* Um **arquivo de rotas** em `/src/routes`
* E deve ser **integrado ao servidor principal** no arquivo `server.ts`.

Essa estrutura modular deve permitir **reutilizar o mesmo padrão de código** para diferentes entidades.

---

### RF06 — Middleware Global de Log (`morgan`)

O sistema deve **registrar todas as requisições HTTP no console**, utilizando uma **biblioteca externa de middleware**.

O nome da biblioteca é **`morgan`**, e ela deve ser **instalada, configurada e aplicada globalmente**.

#### O que é o Morgan?

`morgan` é uma **biblioteca de logging HTTP para Express**.
Ela atua como um **middleware**, ou seja, intercepta todas as requisições e gera logs com informações como:

* Método HTTP (`GET`, `POST`, etc.);
* Caminho da rota (`/users`, `/products/:id`, etc.);
* Status da resposta (`200`, `404`, `500`);
* Tempo de resposta do servidor.

Essas informações são essenciais para **monitorar e depurar** o comportamento da aplicação — e demonstram claramente o conceito de **reuso de software**, já que o desenvolvedor não precisa criar um logger do zero.

---

## ⚙️ Requisitos Técnicos

### RT01 — Estrutura do Projeto

O projeto deve seguir a mesma organização modular da Aula 8:

```
src/
 ├── controllers/
 ├── middlewares/
 ├── models/
 ├── routes/
 └── server.ts
```

---

### RT02 — Instalação de Dependências

O projeto deve estar configurado com **TypeScript** e **Express**, e agora incluir a biblioteca de logs **`morgan`**.

#### Passo 1 — Instalar o Morgan

No terminal, execute:

```bash
npm install morgan
```

Esse comando adiciona o `morgan` como uma **dependência de produção** (ou seja, usada quando o servidor está em execução).

#### Passo 2 — Instalar as definições de tipos

Como estamos utilizando **TypeScript**, precisamos instalar também as definições de tipo da biblioteca para que o compilador reconheça suas estruturas:

```bash
npm install --save-dev @types/morgan
```

O sufixo `--save-dev` indica que esta é uma dependência **apenas de desenvolvimento**.

#### Passo 3 — Verificar o arquivo `package.json`

Após a instalação, verifique se o `morgan` aparece na seção `dependencies` e o `@types/morgan` em `devDependencies`.

---

### RT03 — Scripts do `package.json`

Certifique-se de que o projeto possui os seguintes scripts:

```json
"scripts": {
  "dev": "ts-node-dev --respawn --transpile-only src/server.ts",
  "build": "tsc",
  "start": "node dist/server.js"
}
```

Esses comandos permitem:

* **`npm run dev`** → Executar em modo de desenvolvimento (com recarga automática);
* **`npm run build`** → Compilar o código TypeScript;
* **`npm start`** → Executar a versão compilada em produção.

---

### RT04 — Configuração e Uso do Morgan

Após instalar a biblioteca, configure-a no **arquivo `server.ts`**.

#### Etapa 1 — Importar a biblioteca

No topo do arquivo `server.ts`, importe o `morgan`:

```typescript
import morgan from "morgan";
```

#### Etapa 2 — Aplicar como middleware global

Antes de registrar as rotas, use o `app.use()` para aplicar o `morgan` em toda a aplicação:

```typescript
app.use(morgan("dev"));
```

O parâmetro `"dev"` é um **formato pré-definido** que gera logs compactos e coloridos, ideais para ambiente de desenvolvimento.
Exemplo de saída no console:

```
GET /products 200 12.345 ms - 58
GET /users 304 3.241 ms - -
```

---

### RT05 — Portas e Inicialização

O servidor deve iniciar na **porta 3000** e exibir uma mensagem indicando o funcionamento correto, por exemplo:

```
Servidor rodando na porta 3000 🚀
```

---

## Entregável

1. Projeto completo e funcional, executando com `npm run dev`;
2. Print do terminal mostrando:

   * Logs gerados pelo middleware `morgan`;
   * Resposta dos endpoints `/users` e `/products`;
3. Respostas (curtas e objetivas) para as seguintes perguntas:

   * Onde se aplicou o conceito de **reuso de software**?
   * Qual a importância de utilizar bibliotecas externas (como `morgan`) em um projeto Node.js?
