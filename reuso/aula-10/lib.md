# Exercício Prático — Reuso de Código com Bibliotecas Externas

## Objetivo
Aplicar o conceito de **reuso de software via bibliotecas externas**, passando por todas as etapas essenciais:
- Busca e comparação de bibliotecas;
- Escolha justificada;
- Implementação prática;
- Documentação técnica do uso e dos critérios de escolha.

---

## Contexto

Você faz parte de uma equipe que está criando um **módulo de integração com APIs externas** para um sistema interno da empresa.  
O time quer criar um **componente reutilizável** capaz de realizar chamadas HTTP, com foco em clareza, manutenção e boas práticas.

Seu papel é selecionar uma **biblioteca externa confiável** para essa comunicação e demonstrar seu uso em um pequeno protótipo funcional.

---

## Parte 1 — Pesquisa e Seleção da Biblioteca

1. Escolha **uma linguagem**:  
   - JavaScript (Node.js)  
   - Python  
   - PHP  

2. Pesquise **duas bibliotecas** 
   Exemplos:  
   - JavaScript → `axios`, `node-fetch`  
   - Python → `requests`, `httpx`  
   - PHP → `guzzle`, `symfony/http-client`

3. Crie um arquivo markdown ou um txt no seu repositório e adicione esta **tabela de comparação** com base nos seguintes critérios:

   | Biblioteca | Última atualização | Downloads/semana | Licença | Complexidade da API | Observações |
   |-------------|--------------------|------------------|----------|---------------------|--------------|
   | ... | ... | ... | ... | ... | ... |

4. Escolha **uma** das bibliotecas e registre sua decisão em um pequeno texto:
Exemplo:
   ### Decisão Técnica

   - **Biblioteca escolhida:** axios  
   - **Motivo:** possui sintaxe simples, ampla documentação, suporte a timeout e interceptores.  
   - **Alternativa descartada:** node-fetch (API mais limitada, sem retry nativo).

---

## Parte 2 — Implementação

Implemente uma função que utiliza a biblioteca escolhida

---

## Parte 3 — Documentação Técnica

No arquivo `README.md`, inclua as seguintes seções, veja o exemplo:

```markdown
# Módulo HTTP Reutilizável

## 📦 Biblioteca utilizada
axios (v1.7.2)

## 🧰 Instalação
npm install axios

## ⚙️ Execução
node test_client.js

## 🧩 Motivação
O módulo foi criado para demonstrar reuso de código através de bibliotecas externas.
A escolha do axios se deu por sua ampla documentação, popularidade e facilidade de configuração.

## 🔍 Saída esperada
[INFO] GET https://localhost:3333/users -> 200 (315 ms)
```


