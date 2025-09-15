# Centro Universitário UniOpet

### Curso: ADS / EGS

**Disciplina:** Desenvolvimento Orientado a Reuso de Software
**Professor:** Pedro Vinícius Eckel

---

# 📘 Revisão – Desenvolvimento Orientado a Reuso de Software

## Parte I – Questões Objetivas

**1.** Qual das alternativas representa melhor uma *vantagem prática* do reuso de software em projetos reais?

A) Maior esforço de manutenção de sistemas.<br>
B) Aumento do tempo de desenvolvimento inicial.<br>
C) Redução de retrabalho e aproveitamento de código já testado.<br>
D) Eliminação de toda a documentação de sistemas.<br>
E) Padronização e aceleração do desenvolvimento.<br>

---

**2.** Um hospital comprou um sistema pronto de gestão de pacientes, mas precisou alterar a forma como os atendimentos eram registrados para se adaptar ao software. Esse caso ilustra:

A) Benefício do reuso de software.<br>
B) Uso de microserviços.<br>
C) Problema de adaptação de requisitos a sistemas de aplicação.<br>
D) Desenvolvimento ágil.<br>
E) Integração de bibliotecas externas.<br>

---

**3.** Qual das opções está mais associada ao modelo **incremental** de desenvolvimento de software?

A) Entregas parciais de funcionalidades com feedback contínuo dos usuários.<br>
B) Execução linear e rígida de fases.<br>
C) Maior dificuldade de adaptação a mudanças.<br>
D) Eliminação total da dívida técnica.<br>
E) Exclusivo para projetos acadêmicos.<br>

---

**4.** Uma característica marcante do modelo **cascata** é:

A) Flexibilidade total a mudanças de requisitos a qualquer momento.<br>
B) Desenvolvimento simultâneo de todas as etapas.<br>
C) Protótipos rápidos entregues de forma contínua.<br>
D) Estrutura sequencial com alto custo de mudanças tardias.<br>
E) Uso obrigatório de microserviços.<br>

---

**5.** A principal vantagem do modelo **espiral** em relação ao cascata é:

A) Custos sempre mais baixos em qualquer cenário.<br>
B) Integração automática com sistemas prontos.<br>
C) Eliminação da necessidade de testes.<br>
D) Simplicidade de implementação em qualquer contexto.<br>
E) Inclusão de análise de riscos e prototipação em cada ciclo.<br>

---

**6.** Qual das alternativas representa uma **desvantagem** no uso de plataformas No Code / Low Code?

A) Maior velocidade na prototipagem de MVPs.<br>
B) Dependência da plataforma, dificultando migrações (vendor lock-in).<br>
C) Redução do tempo para entregar soluções.<br>
D) Possibilidade de integrar APIs externas.<br>
E) Padronização da interface e componentes.<br>

---

**7.** Sistemas ERP normalmente possuem:

A) Banco de dados centralizado para diferentes áreas da empresa.<br>
B) Ausência de módulos configuráveis.<br>
C) Foco exclusivo em pequenas startups.<br>
D) Rejeição a processos de negócio padronizados.<br>
E) Exclusividade para uso acadêmico.<br>

---

**8.** No contexto de integração de sistemas de aplicação, qual é uma recomendação prática?

A) Ignorar contratos de nível de serviço (SLA).<br>
B) Usar apenas planilhas para garantir interoperabilidade.<br>
C) Testar protótipos de integração antes de adotar definitivamente.<br>
D) Evitar documentar decisões de projeto.<br>
E) Impedir o uso de APIs externas.<br>

---

**9.** Qual é um dos *problemas* associados ao reuso de software?

A) Síndrome do "não inventado aqui".<br>
B) Redução do tempo de entrega.<br>
C) Uso eficaz de especialistas.<br>
D) Conformidade com padrões.<br>
E) Maior cobertura de testes.<br>

---

**10.** O que diferencia uma biblioteca de um framework?

A) Ambos funcionam da mesma forma, sem diferenças.<br>
B) Biblioteca é chamada pelo desenvolvedor; framework define o fluxo e chama o código do desenvolvedor.<br>
C) Frameworks nunca podem ser usados em aplicações web.<br>
D) Bibliotecas só funcionam em sistemas operacionais específicos.<br>
E) Frameworks dispensam totalmente o uso de banco de dados.<br>

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
O objetivo é praticar o **reuso de software** por meio de frameworks já consolidados no mercado.

Cada aluno deve:

1. **Escolher um framework** entre as opções abaixo:

**Opções de backend (APIs REST):**
A) [FastAPI](https://fastapi.tiangolo.com/)
B) [Django](https://docs.djangoproject.com/en/stable/)
C) [Express.js](https://expressjs.com/)
D) [NestJS](https://docs.nestjs.com/)

**Opção fullstack (rotas + frontend):**
E) [Next.js](https://nextjs.org/docs)

---

2. Ler a documentação oficial (links acima).

3. Identificar como criar **uma rota simples** (`/clientes`) que retorne uma lista em JSON ou uma tela de (`/clientes`) que retorna uma lista visual.

4. Responder:

* Qual framework escolheu.
* Link da documentação usada.
* Um pequeno trecho de código de exemplo retirado/adaptado da documentação.

---

5. **Complemento em segurança:**
   Pesquise como o framework escolhido trata **autenticação e login**.

Responda de forma breve:

* O framework oferece recursos nativos para login/autenticação ou depende de bibliotecas externas?
* Esse suporte facilita a vida do desenvolvedor ou exige muito esforço manual?
* Em sua visão, a segurança nesse framework é mais **padronizada** (soluções prontas para reuso) ou mais **aberta** (cada desenvolvedor deve construir sua própria solução)?

---

6. **Reflexão sobre reuso:**
   Explique em poucas linhas como o framework escolhido representa **reuso de software**.
