# Centro Universitário UniOpet

### Curso: ADS / EGS

**Disciplina:** Desenvolvimento Orientado a Reuso de Software
**Professor:** Pedro Vinícius Eckel

---

# 📘 Revisão – Desenvolvimento Orientado a Reuso de Software

## Parte I – Questões Objetivas

**1.** Qual das alternativas representa melhor uma *vantagem prática* do reuso de software em projetos reais?
A) Maior esforço de manutenção de sistemas.
B) Aumento do tempo de desenvolvimento inicial.
C) Redução de retrabalho e aproveitamento de código já testado.
D) Eliminação de toda a documentação de sistemas.
E) Padronização e aceleração do desenvolvimento.

---

**2.** Um hospital comprou um sistema pronto de gestão de pacientes, mas precisou alterar a forma como os atendimentos eram registrados para se adaptar ao software. Esse caso ilustra:
A) Benefício do reuso de software.
B) Uso de microserviços.
C) Problema de adaptação de requisitos a sistemas de aplicação.
D) Desenvolvimento ágil.
E) Integração de bibliotecas externas.

---

**3.** Qual das opções está mais associada ao modelo **incremental** de desenvolvimento de software?
A) Entregas parciais de funcionalidades com feedback contínuo dos usuários.
B) Execução linear e rígida de fases.
C) Maior dificuldade de adaptação a mudanças.
D) Eliminação total da dívida técnica.
E) Exclusivo para projetos acadêmicos.

---

**4.** Uma característica marcante do modelo **cascata** é:
A) Flexibilidade total a mudanças de requisitos a qualquer momento.
B) Desenvolvimento simultâneo de todas as etapas.
C) Protótipos rápidos entregues de forma contínua.
D) Estrutura sequencial com alto custo de mudanças tardias.
E) Uso obrigatório de microserviços.

---

**5.** A principal vantagem do modelo **espiral** em relação ao cascata é:
A) Custos sempre mais baixos em qualquer cenário.
B) Integração automática com sistemas prontos.
C) Eliminação da necessidade de testes.
D) Simplicidade de implementação em qualquer contexto.
E) Inclusão de análise de riscos e prototipação em cada ciclo.

---

**6.** Qual das alternativas representa uma **desvantagem** no uso de plataformas No Code / Low Code?
A) Maior velocidade na prototipagem de MVPs.
B) Dependência da plataforma, dificultando migrações (vendor lock-in).
C) Redução do tempo para entregar soluções.
D) Possibilidade de integrar APIs externas.
E) Padronização da interface e componentes.

---

**7.** Sistemas ERP normalmente possuem:
A) Banco de dados centralizado para diferentes áreas da empresa.
B) Ausência de módulos configuráveis.
C) Foco exclusivo em pequenas startups.
D) Rejeição a processos de negócio padronizados.
E) Exclusividade para uso acadêmico.

---

**8.** No contexto de integração de sistemas de aplicação, qual é uma recomendação prática?
A) Ignorar contratos de nível de serviço (SLA).
B) Usar apenas planilhas para garantir interoperabilidade.
C) Testar protótipos de integração antes de adotar definitivamente.
D) Evitar documentar decisões de projeto.
E) Impedir o uso de APIs externas.

---

**9.** Qual é um dos *problemas* associados ao reuso de software?
A) Síndrome do "não inventado aqui".
B) Redução do tempo de entrega.
C) Uso eficaz de especialistas.
D) Conformidade com padrões.
E) Maior cobertura de testes.

---

**10.** O que diferencia uma biblioteca de um framework?
A) Ambos funcionam da mesma forma, sem diferenças.
B) Biblioteca é chamada pelo desenvolvedor; framework define o fluxo e chama o código do desenvolvedor.
C) Frameworks nunca podem ser usados em aplicações web.
D) Bibliotecas só funcionam em sistemas operacionais específicos.
E) Frameworks dispensam totalmente o uso de banco de dados.

---

## Parte II – Questões Dissertativas

**11.** Compare os modelos **cascata, incremental e espiral**. Em quais situações cada um é mais adequado e por quê?

---

**12.** Explique o que são **sistemas de aplicação (COTS)**. Cite um exemplo real do mercado e descreva como eles são configurados para diferentes clientes.

---

**13.** Quais são os principais **benefícios e desafios** de usar plataformas **No Code / Low Code** em projetos de software? Dê exemplos de situações práticas em que cada ponto aparece.

---

**14.** Uma empresa comprou um ERP, mas percebeu um grande descompasso entre o modelo do sistema e seus processos internos. Explique:

* Por que isso pode acontecer.
* Quais estratégias poderiam reduzir esse risco antes da adoção do sistema.

---

**15.** Uma universidade pretende substituir o Microsoft Office pelo LibreOffice. Explique por que essa decisão está relacionada ao **reuso de software** e quais seriam as vantagens e limitações dessa escolha.

---

## Parte III – Questão Prática

**16.** Imagine que sua equipe foi contratada para desenvolver um **sistema de cadastro de clientes**.
Cada aluno deve:

1. Escolher **um framework** entre as opções:

   * FastAPI
   * Django
   * Express.js
   * NestJS
   * Next.js

2. Ler a documentação oficial.

3. Identificar como criar **uma rota simples** (`/clientes`) que retorne uma lista em JSON.

4. Responder:

   * Qual framework escolheu.
   * Link da documentação usada.
   * Um pequeno trecho de código de exemplo retirado/adaptado da documentação.

5. **Complemento em segurança:**

   * Pesquisar como o framework escolhido trata **autenticação e login**.
   * Responder:

     * O framework oferece recursos nativos para login e autenticação, ou depende de bibliotecas externas?
     * Esse suporte facilita a vida do desenvolvedor ou exige muito esforço manual?
     * Em sua visão, a segurança nesse framework é mais **padronizada** (soluções prontas para reuso) ou mais **aberta** (cada desenvolvedor deve construir suas próprias soluções)?
