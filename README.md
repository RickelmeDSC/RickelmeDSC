<h1 align="center">Rickelme David</h1>

<p align="center">
  <strong>Analista de Dados & Desenvolvedor</strong><br>
  Dados que sustentam decisões — e sistemas que produzem dados confiáveis
</p>

<p align="center">
  <a href="https://github.com/RickelmeDSC">GitHub</a> •
  <a href="https://www.linkedin.com/in/rickelme-david-75630b203/">LinkedIn</a> •
  <a href="mailto:rickelmepe@gmail.com">Email</a>
</p>

---

## Sobre

Analista de Dados na Health & Safety Tech, atuando em análise, desenvolvimento e qualidade de sistemas corporativos em produção. Meu trabalho é orientado a medição — inclusive quando a medição me contraria, o que já aconteceu algumas vezes e está documentado abaixo.

Cursando Análise e Desenvolvimento de Sistemas na UNIBRA (conclusão em jun/2027).

---

## Trabalho profissional

*Sistemas internos, sem repositório público.*

### HelpHS — sistema principal
`Python` `FastAPI` `React` `TypeScript` `PostgreSQL` `pgvector`

Atuação em análise, engenharia e segurança entre agosto e setembro de 2026.

**Quando a métrica mente**
- Descobri que o indicador de SLA de primeira resposta media o tempo até alguém **clicar**, não até alguém **responder** — respostas por chat não eram contabilizadas, enquanto atribuir ou cancelar um chamado eram. Um erro de ordem na gravação fazia com que respostas atrasadas quase nunca fossem registradas como violação
- Medi o que estava **de fato implantado** — migration do banco, rotas no ar, arquivos do bundle — em vez de deduzir pela árvore de commits. A medição mudou a ordem do que precisava ser feito

**Segurança**
- Fechei um banco de dados de produção que respondia na internet pública, descoberto ao sondar portas vizinhas ao IP do servidor
- Removi a criação automática, a cada reinício do contêiner, de um administrador com senha versionada no repositório
- Corrigi enumeração por tempo no login (1 ms contra 250 ms), recusas que denunciavam a existência de registros alheios, e um cabeçalho HTTP capaz de ocupar o processo por **151 segundos** — reduzido a 0,01 s
- Implantei segundo fator (TOTP) para contas administrativas, rate limiting e correlação de logs

**IA e busca vetorial**
- Construí a busca vetorial (pgvector) de um assistente interno de atendimento, com o corte de relevância derivado de **40 perguntas rotuladas à mão** — os trechos entregues ao modelo caíram de 160 para 25
- A medição derrubou meu próprio desenho: defendi processamento em lote por economia de rede; medido, o custo real era memória (3,7 GB de pico contra 5,1 GB disponíveis)

**Qualidade**
- Testes de backend de **399 para 1.213** (cobertura 89,76%); front-end de **192 para 1.443**
- Encontrei defeitos com data marcada: a numeração de protocolo travaria no 10.000º chamado do ano, e nenhum e-mail seria enviado no dia em que o SMTP fosse ligado

---

### ChamadosHS — sistema de chamados
`React` `TypeScript` `Node.js` `PostgreSQL`

Assumi a manutenção e entreguei **280 alterações em 44 versões** ao longo de 17 dias de trabalho.

- Testes automatizados de **46 para 649**
- Autoria das ações movida para o servidor — a trilha de auditoria deixou de ser falsificável pelo cliente
- Diagnóstico de adesão de 8,3% numa funcionalidade de avaliação (12 de 144 chamados em nove meses), rastreado ao posicionamento na interface
- Recuperação de 4 chamados que sumiam da interface sem sair do estado interno, continuando a contar como pendência no painel
- Validação automática de contraste e daltonismo que reprova a publicação, e suporte a leitor de tela

---

## Projetos públicos

### 🔧 claude-code-hub
*Painel de terminal para navegar repositórios, histórico de sessões e memória de projeto*

PowerShell, sem dependências além de `git`, `gh` e `claude`. **164 testes automatizados** que passam num clone recém-baixado, contra um ambiente sintético — nenhum teste lê dados reais ou acessa a rede.

Otimização guiada por medição: a abertura caiu de 6–10 segundos para ~440 ms, e três decisões de desenho foram revertidas pelo que a medição mostrou.

`PowerShell 5.1` · `MIT` · ~3.650 linhas

🔗 https://github.com/RickelmeDSC/claude-code-hub

---

### 📊 Análise da Distribuição de Renda — PNAD 2015
*Análise estatística dos microdados oficiais do IBGE*

Após uma economista PhD apontar a ausência de pesos amostrais na primeira versão, refiz o estudo inteiro em **R com o pacote `survey`**, sobre os 116 mil registros oficiais. Identifiquei e documentei uma divergência de 40 mil registros entre uma base curada de terceiros e a fonte oficial.

`Python` · `Pandas` · `R` · `SQL`

🔗 https://github.com/RickelmeDSC/analise-descritiva-pnad-2015

---

### 🏛️ ONG CAMM4 — Sistema de gestão em produção
*Plataforma completa para digitalizar a gestão de uma ONG*

Construída do zero: API REST modular, autenticação JWT com refresh token rotativo, RBAC, rate limiting, auditoria e documentação Swagger. Arquitetura em camadas, API-first.

`Node.js` · `NestJS` · `TypeScript` · `Prisma` · `PostgreSQL`

🔗 [Sistema online](https://ongcamm4.vercel.app) · [Repositório](https://github.com/RickelmeDSC/ONGCAMM4)

---

### 🚢 Análise Titanic — SQL e estatística em Python puro
10 queries analíticas e 5 métricas estatísticas implementadas na mão, validadas contra as bibliotecas.

`Python` · `SQLite` · `SQL`

🔗 https://github.com/RickelmeDSC/analise-titanic-sql-estatistica

---

### ✅ TaskFlow — Gerenciador de tarefas
API CRUD com arquitetura organizada por camadas.

`Flask` · `MySQL`

🔗 https://github.com/RickelmeDSC/TaskFlow

---

## Stack

**Dados**
`Python` `Pandas` `NumPy` `SciPy` `R` `SQL` `Power BI` `Excel`

**Backend**
`FastAPI` `Node.js` `NestJS` `TypeScript` `PostgreSQL` `MySQL` `SQLAlchemy` `Prisma`

**Front-end**
`React` `TypeScript` `Tailwind CSS`

**Qualidade e infra**
`Testes automatizados` `Teste por mutação` `Git` `Docker` `Linux` `CI/CD`

---

## Como eu trabalho

**Medir antes de concluir — e aceitar quando a medição me contraria.** Defendi processamento em lote num serviço de IA por economizar viagens de rede. Medido, o custo real era memória: 3,7 GB de pico num servidor com 5,1 GB livres. O lote foi reduzido.

**Teste por mutação, porque o verde esconde coisa.** Já escrevi um teste chamado "o mesmo desafio não serve duas vezes" que passava — e provava outra coisa. Mutar o código mostrou que ele nunca testou o que o nome dizia.

**Desconfiar da régua, não só do resultado.** `tsc --noEmit` reportava "limpo" e olhava zero arquivos. A cobertura da suíte inteira estava abaixo do real porque o coverage perdia o rastro a cada await. A pergunta que encontra esse tipo de coisa: *sobre o que exatamente esta régua opera?*

**Declarar a limitação em vez de contorná-la.** Na análise da PNAD, encontrei 40 mil registros de divergência entre uma base curada e a fonte oficial. Não consegui explicar o gap — então documentei a inconsistência em vez de reconciliá-la em silêncio.

---

<p align="center">
  <sub>Recife / Olinda, PE • Aberto a oportunidades em dados e desenvolvimento</sub>
</p>
