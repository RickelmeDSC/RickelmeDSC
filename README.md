<h1 align="center">Rickelme David</h1>

<p align="center">
  <strong>Data Analyst & Backend Developer</strong><br>
  Dados que sustentam decisões — e sistemas que produzem dados confiáveis
</p>

<p align="center">
  <a href="https://github.com/RickelmeDSC">GitHub</a> •
  <a href="https://www.linkedin.com/in/rickelme-david-75630b203/">LinkedIn</a> •
  <a href="mailto:rickelmepe@gmail.com">Email</a>
</p>

---

## Sobre

Analista de Dados na Health & Safety Tech, com base em desenvolvimento backend. Trabalho nas duas pontas: extraio, limpo e analiso dados operacionais — e construo os sistemas que geram esses dados.

Cursando Análise e Desenvolvimento de Sistemas na UNIBRA (conclusão em jun/2027).

---

## Trabalho profissional

### ChamadosHS — Sistema de chamados em produção
*Sistema interno, sem repositório público*

Assumi a manutenção de um help desk em operação e entreguei, ao longo de 17 dias de trabalho, **280 alterações em 44 versões publicadas**.

- **Testes automatizados: de 46 para 649**, cobrindo API e front-end
- Fechamento de rotas da API que respondiam sem autenticação
- Autoria das ações movida para o servidor — a trilha de auditoria deixou de ser falsificável pelo cliente
- Diagnóstico de adesão de 8,3% numa funcionalidade de avaliação (12 de 144 chamados em nove meses), rastreado ao posicionamento na interface, com realocação e remedição agendada
- Recuperação de 4 chamados que sumiam da interface sem sair do estado interno — continuavam contando como pendência no painel
- Validação automática de contraste e daltonismo que reprova a publicação, e suporte a leitor de tela

**Stack:** React · TypeScript · Node.js · PostgreSQL

---

## Projetos

### 🔧 claude-code-hub
*Painel de terminal para navegar repositórios, histórico de sessões e memória de projeto*

Ferramenta em PowerShell, sem dependências além de `git`, `gh` e `claude`. **164 testes automatizados** que passam num clone recém-baixado, contra um ambiente sintético — nenhum teste lê dados reais ou acessa a rede.

Otimização guiada por medição: o tempo de abertura caiu de 6–10 segundos para ~440 ms. Nenhuma das três causas estava onde o código parecia lento.

`PowerShell 5.1` · `MIT` · ~3.650 linhas

🔗 https://github.com/RickelmeDSC/claude-code-hub

---

### 📊 Análise da Distribuição de Renda — PNAD 2015
*Análise estatística dos microdados oficiais do IBGE*

Análise descritiva completa da desigualdade de renda no Brasil. Após uma economista PhD apontar a ausência de pesos amostrais na primeira versão, refiz o estudo inteiro em **R com o pacote `survey`**, sobre os 116 mil registros oficiais — o que revelou padrões que a amostra bruta escondia.

Inclui documentação metodológica separada, com fontes, decisões de desenho e limitações conhecidas.

`Python` · `Pandas` · `R` · `SQL`

🔗 https://github.com/RickelmeDSC/analise-descritiva-pnad-2015

---

### 🏛️ ONG CAMM4 — Sistema de gestão em produção
*Plataforma completa para digitalizar a gestão de uma ONG*

Cadastro de crianças e responsáveis, controle de frequência, gestão de doações e dashboard administrativo. Construído do zero, hoje em uso real.

- Autenticação JWT com refresh token rotativo e RBAC (Diretor, Gestor, Voluntário)
- Rate limiting, auditoria de ações e documentação Swagger/OpenAPI
- Arquitetura em camadas (Controller → Service → ORM), API-first

`Node.js` · `NestJS` · `TypeScript` · `Prisma` · `PostgreSQL`

🔗 [Sistema online](https://ongcamm4.vercel.app) · [Repositório](https://github.com/RickelmeDSC/ONGCAMM4)

---

### 🚢 Análise Titanic — SQL e estatística em Python puro
*10 queries analíticas e 5 métricas estatísticas implementadas na mão*

Modelagem e carga em SQLite, com as métricas implementadas manualmente — sem `.mean()` ou `.median()` — e validadas contra as bibliotecas.

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
`Node.js` `NestJS` `TypeScript` `Flask` `PostgreSQL` `MySQL` `Prisma`

**Front-end**
`React` `TypeScript` `Tailwind CSS`

**Ferramentas**
`Git` `Docker` `Linux` `Jupyter` `Swagger`

---

## Como eu trabalho

**Medir antes de concluir.** No claude-code-hub, três decisões de desenho foram revertidas pela medição — em uma delas, 243 arquivos de sessão eram na verdade 47 conversas reais e 196 transcrições aninhadas.

**Teste e documentação fazem parte da entrega.** Cada decisão não óbvia carrega, no código, a razão e o defeito que a motivou.

**Declarar a limitação em vez de contorná-la.** Na análise da PNAD, encontrei 40 mil registros de divergência entre uma base curada e a fonte oficial. Não consegui explicar o gap — então documentei a inconsistência.

---

<p align="center">
  <sub>Recife / Olinda, PE • Aberto a oportunidades em dados e desenvolvimento</sub>
</p>
