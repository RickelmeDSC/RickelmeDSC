<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=215&color=0:07111F,45:0F766E,100:2563EB&text=Rickelme%20David&fontColor=FFFFFF&fontSize=52&fontAlignY=36&desc=Dados%20%C2%B7%20Backend%20%C2%B7%20IA%20Aplicada%20%C2%B7%20Qualidade%20de%20Software&descAlignY=58&descSize=18&animation=fadeIn"/>

<div align="center">

<a href="https://github.com/RickelmeDSC">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&duration=3200&pause=900&color=14B8A6&center=true&vCenter=true&width=760&lines=Python+%C2%B7+SQL+%C2%B7+React+%C2%B7+FastAPI;An%C3%A1lise+de+dados%2C+estat%C3%ADstica+e+ETL;Backend%2C+APIs+e+sistemas+em+produ%C3%A7%C3%A3o;RAG%2C+embeddings+e+IA+aplicada;Medir+antes+de+concluir.+Testar+antes+de+confiar." alt="Apresentação profissional de Rickelme David" />
</a>

Analista de Dados na Health & Safety Tech · Pernambuco, Brasil
<sub>Transformo dados em evidência e problemas de software em sistemas mais confiáveis.</sub>




</div>

Sobre mim
Atuo na interseção entre análise de dados, desenvolvimento backend, qualidade de software, segurança e IA aplicada.
Meu foco não é apenas fazer uma solução funcionar. Gosto de entender o que está sendo medido, onde o dado pode estar errado, quais hipóteses realmente se sustentam e como transformar isso em software auditável e confiável.
No trabalho e nos projetos pessoais, já atuei com:
- Python, SQL, R, TypeScript e JavaScript
- FastAPI, NestJS, Flask e React
- PostgreSQL, MySQL, SQLite, Prisma e SQLAlchemy
- Power BI, Power Query, pandas, NumPy e SciPy
- RAG, embeddings, pgvector e ONNX Runtime
- testes automatizados, revisão de código e segurança de aplicações
- Docker, Git, GitHub e documentação técnica
Alguns números
<table align="center">
  <tr>
    <td align="center" width="210">
      <h2>399 → 1.314</h2>
      <sub>testes de backend<br><b>HelpHS</b></sub>
    </td>
    <td align="center" width="210">
      <h2>46 → 649</h2>
      <sub>testes automatizados<br><b>ChamadosHS</b></sub>
    </td>
    <td align="center" width="210">
      <h2>6–10 s → ~440 ms</h2>
      <sub>tempo de abertura<br><b>claude-code-hub</b></sub>
    </td>
    <td align="center" width="210">
      <h2>151 s → 0,01 s</h2>
      <sub>mitigação de comportamento abusivo<br><b>HelpHS</b></sub>
    </td>
  </tr>
</table>

O que eu faço
<table>
  <tr>
    <td width="50%" valign="top">

📊 Dados & Analytics
- Análise exploratória e estatística aplicada
- SQL para investigação e análise
- ETL e tratamento de dados com Python
- Power BI e Power Query
- Qualidade, reconciliação e rastreabilidade de dados
- R com desenho amostral complexo
    </td>
    <td width="50%" valign="top">
⚙️ Backend & Sistemas
- APIs REST com FastAPI, NestJS e Flask
- PostgreSQL, SQLAlchemy e Prisma
- Autenticação com JWT e controle de acesso
- Regras de negócio e integrações
- Arquitetura em camadas
- Sistemas internos em produção
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
🤖 IA Aplicada
- Retrieval-Augmented Generation (RAG)
- Embeddings e busca vetorial
- pgvector e distância cosseno
- Calibração de limiar de relevância
- ONNX Runtime
- Avaliação de comportamento de sistemas com IA
    </td>
    <td width="50%" valign="top">
🛡️ Qualidade & Segurança
- Testes automatizados
- Testes por mutação
- Code review
- Auditoria de segurança
- Investigação de falhas silenciosas
- Documentação técnica e decisões baseadas em evidência
    </td>
  </tr>
</table>

Projetos em destaque
🧩 HelpHS
Plataforma de atendimento, SLA, conhecimento e IA
Sistema principal da Health & Safety Tech, com backend em Python/FastAPI, frontend em React e banco PostgreSQL.
Entre as frentes em que atuei:
- evolução da suíte de backend de 399 para 1.314 testes
- diagnóstico e correção de um indicador de SLA que media o evento errado
- auditoria de segurança em rotas e infraestrutura
- identificação de enumeração por tempo no login
- mitigação de um caso de processamento abusivo de cabeçalho HTTP de 151 s para 0,01 s
- desenvolvimento e avaliação da busca semântica da assistente Helô
- calibração de corte de relevância com perguntas rotuladas manualmente
Stack: Python · FastAPI · React · PostgreSQL · SQLAlchemy · pgvector · ONNX Runtime · Docker

⚡ claude-code-hub
Painel de terminal para produtividade com Claude Code
Ferramenta em PowerShell que organiza repositórios, sessões e contexto de projetos do Claude Code.
- cerca de 3.650 linhas
- 164 testes automatizados
- testes executados contra ambiente sintético
- abertura otimizada de 6–10 segundos para aproximadamente 440 ms
- decisões de arquitetura revistas com base em medição real
Stack: PowerShell · Testes automatizados · Git · Claude Code

📈 Análise da Distribuição de Renda — PNAD 2015
Estatística aplicada com Python, R e microdados oficiais do IBGE
Projeto que começou como análise descritiva e evoluiu para um estudo com desenho amostral complexo após uma revisão metodológica pública.
- análise inicial com Python
- reimplementação em R com o pacote survey
- pesos amostrais, estratificação e conglomeração
- uso dos microdados oficiais do IBGE
- documentação explícita de uma divergência de 39.627 registros entre bases
- resultados revisados publicamente após crítica técnica
Stack: Python · R · survey · dplyr · ggplot2 · SQL

🏠 ONG CAMM4
Sistema full stack de gestão para uma ONG
Plataforma desenvolvida para digitalizar processos administrativos da ONG CAMM4.
Recursos principais:
- cadastro de crianças e responsáveis
- controle de frequência
- gestão de doações
- dashboard administrativo
- autenticação JWT com refresh token rotativo
- RBAC para Diretor, Gestor e Voluntário
- rate limiting
- auditoria automática
- documentação Swagger/OpenAPI
Stack: NestJS · TypeScript · PostgreSQL · Prisma · JWT · React

🚢 Titanic — SQL & Estatística
Projeto analítico com 891 passageiros, modelagem em SQLite e estatística implementada manualmente em Python.
- 10 consultas SQL analíticas
- GROUP BY, CASE, agregações e cruzamentos
- 5 métricas estatísticas implementadas do zero
- validação dos resultados contra bibliotecas
- comparação prática entre média e mediana
Stack: Python · SQL · SQLite · Estatística

🧰 Tecnologias
<div align="center">

Linguagens
<img src="https://skillicons.dev/icons?i=python,ts,js,r,powershell" alt="Python, TypeScript, JavaScript, R e PowerShell" />




Backend & Frontend
<img src="https://skillicons.dev/icons?i=fastapi,nestjs,nodejs,flask,react,tailwind" alt="FastAPI, NestJS, Node.js, Flask, React e Tailwind" />




Dados & Bancos
<img src="https://skillicons.dev/icons?i=postgres,mysql,sqlite,prisma" alt="PostgreSQL, MySQL, SQLite e Prisma" />




DevOps & Ferramentas
<img src="https://skillicons.dev/icons?i=docker,git,github,linux,vscode" alt="Docker, Git, GitHub, Linux e VS Code" />

</div>


<div align="center">








</div>

Experiência
Health & Safety Tech
Analista de Dados · 2026 — atual
Atuação envolvendo análise de dados, desenvolvimento de sistemas internos, backend, qualidade de software, segurança da informação e IA aplicada.

Conorte
Estagiário de TI · 2025 — 2026
Atuação com Power BI, Excel, SQL, estruturação de dados operacionais e infraestrutura de TI.
Formação
🎓 Análise e Desenvolvimento de Sistemas — UNIBRA
Conclusão prevista para 2027.
Como eu trabalho
Medir antes de concluir. Desconfiar da régua, não apenas do resultado. Documentar a limitação em vez de escondê-la.

Alguns princípios que carrego para os projetos:
- decisões técnicas devem ter evidência
- testes precisam provar o comportamento que dizem provar
- métricas precisam medir exatamente o que prometem
- uma limitação documentada é melhor que uma certeza inventada
- código confiável depende tanto de engenharia quanto de observação
GitHub
<div align="center">

<img height="165" src="https://github-readme-streak-stats.herokuapp.com?user=RickelmeDSC&theme=tokyonight&hide_border=true" alt="GitHub streak de RickelmeDSC" />

</div>

<div align="center">

Vamos conversar?



<sub>Dados · Engenharia · IA aplicada · Qualidade</sub>
</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=115&color=0:2563EB,50:0F766E,100:07111F&section=footer"/>
