# Análise da Plataforma de Inteligência de Engenharia DevStats

## 1. Resumo Completo

O DevStats é uma plataforma de análise de métricas de engenharia de software projetada para fornecer a líderes e equipes de desenvolvimento uma visão clara e acionável sobre seus processos. A ferramenta se posiciona como uma alternativa a dashboards complexos e reuniões de status, focando em métricas objetivas para otimizar o fluxo de trabalho, identificar gargalos e melhorar a previsibilidade das entregas. Fundada por Phil Alves, a empresa tem sede em Utah, EUA, e opera com um modelo *bootstrapped*, ou seja, sem grandes investimentos externos, focando em um público de pequenas e médias empresas (SMBs) [1][2].

A plataforma se integra com as principais ferramentas de desenvolvimento, como GitHub, GitLab, Jira e outras, para coletar metadados e gerar insights sobre o ciclo de desenvolvimento de software. Um dos seus principais diferenciais é a ênfase na simplicidade e clareza, com uma configuração que leva, segundo a empresa, cerca de 10 minutos, sem a necessidade de alterações no código-fonte dos projetos [3].

## 2. Métricas Disponíveis

O DevStats oferece um conjunto abrangente de métricas, organizadas em seis categorias principais, que cobrem todo o ciclo de vida do desenvolvimento de software [4].

| Categoria | Métricas Principais |
| :--- | :--- |
| **Flow (Fluxo)** | PR Cycle Time, Issue Cycle Time, Throughput, Open PRs, Daily WIP, Aging Issues, Aging Branches. |
| **Planejamento & Sprints** | Sprints, Sprint Progress Summary, Planning Accuracy, Work Breakdown. |
| **Investimento & Alocação** | Investment Profile, Engineering Investment, Allocation. |
| **Qualidade & Confiabilidade** | Code Review, DORA Metrics, Deploy, Benchmarks. |
| **Visibilidade & Insights** | Speed, Activity Heatmap, Productivity, Collaboration, Player Dashboard. |
| **Impacto de IA** | AI Usage (Adoção, Ganhos de Produtividade, Qualidade de Código). |

As **Métricas DORA** (Frequência de Deploy, Lead Time, Taxa de Falha e MTTR) são um dos destaques, sendo consideradas o padrão-ouro para mensurar a performance de DevOps [5]. A plataforma também permite o **Benchmarking**, comparando a performance da equipe com milhares de outras organizações, o que ajuda a definir metas realistas e a identificar pontos de melhoria.

## 3. Customização

A plataforma oferece diversas opções de customização para adaptar os relatórios e métricas às necessidades específicas de cada equipe e projeto [6].

- **Configuração de Relatórios:** É possível definir regras para o rastreador de issues (ex: excluir tarefas por tipo ou palavra-chave, excluir subtarefas, definir colunas "Done"), para o Git, para deploys e para o perfil de investimento.
- **Filtros Avançados:** Os relatórios podem ser filtrados por squad, por contribuidores individuais (players), por repositório, por período de tempo e por etapas do fluxo de trabalho.
- **Alertas:** O sistema permite a configuração de alertas via Slack e e-mail para notificar sobre PRs parados, acúmulo de revisões ou quando o trabalho excede os SLAs definidos.
- **API:** Os planos Pro e Enterprise oferecem acesso à API do DevStats, permitindo a extração de dados para a criação de dashboards customizados ou integração com outras ferramentas.
- **Plano Enterprise:** Este plano oferece o nível mais alto de customização, incluindo a criação de métricas e relatórios personalizados, além de integrações sob medida.

## 4. Preço e Cobrança no Brasil

O DevStats adota um modelo de preço por colaborador ativo, definido como um desenvolvedor que realizou ao menos um commit ou PR nos últimos 30 dias. A plataforma oferece planos mensais e anuais, com um desconto de 17% na modalidade anual [7].

**Preços em Dólar (USD) e Real (BRL)**

| Plano | Pagamento Anual (por mês) | Pagamento Mensal |
| :--- | :--- | :--- |
| **Starter** | $15 USD / R$75 BRL | $18 USD / R$90 BRL |
| **Pro** | $27 USD / R$135 BRL | $32 USD / R$160 BRL |
| **Enterprise** | Sob consulta | Sob consulta |

A existência de preços em Reais (BRL) no site em português é um forte indicativo de que a empresa possui um mecanismo de cobrança local para o mercado brasileiro. A análise da conversão mostra uma taxa de câmbio implícita de aproximadamente R$5,00 por dólar, que parece ser fixa e não flutua com o mercado. Se a cobrança for processada no Brasil em Reais, **não haverá incidência de IOF** (Imposto sobre Operações Financeiras) de 6,38%, que é aplicado em compras internacionais. No entanto, é recomendável confirmar com a empresa se a transação é de fato local para garantir a isenção do imposto [8].

## 5. Análise do Uso de IA dos Devs

Sim, o DevStats possui uma funcionalidade dedicada à análise do uso de ferramentas de Inteligência Artificial pelos desenvolvedores, disponível nos planos Pro e Enterprise. O **AI Usage Dashboard** monitora a adoção, o impacto na produtividade e as tendências de uso de IA ao longo do tempo [9].

**Ferramentas de IA Suportadas:**
- GitHub Copilot
- Claude for Developers (Claude Code)
- Cursor
- Amazon Q
- Cody
- Windsurf

**Métricas de IA Coletadas:**
- **Code Suggestions:** Total de sugestões de código geradas pela IA.
- **Suggestions Accepted:** Número de sugestões que foram aceitas e inseridas no código.
- **Chat Sessions:** Total de interações via chat com a IA (perguntas, debugging, etc.).
- **Code Insertions:** Quantidade de trechos de código inseridos diretamente a partir do chat da IA.
- **PR Summaries Created:** Número de resumos de Pull Request gerados automaticamente pela IA.

Essas métricas permitem que os gestores entendam não apenas a frequência de uso, mas também a relevância e a eficácia das ferramentas de IA no fluxo de trabalho da equipe.

## 6. Segurança das Informações

A segurança é um ponto de destaque na comunicação da DevStats. A empresa possui a certificação **SOC 2 Tipo II**, que atesta seus controles de segurança no tratamento e proteção de dados. Além disso, realiza testes de penetração anuais por terceiros e garante um SLA de 99,9% de disponibilidade [10].

Os principais pilares de segurança da plataforma são:

- **Acesso Somente Leitura:** A ferramenta solicita apenas permissões de leitura nos repositórios, não podendo escrever ou modificar o código.
- **Sem Acesso ao Código-Fonte:** O DevStats declara explicitamente que **nunca armazena, processa ou acessa o código-fonte** dos clientes. A análise é feita exclusivamente sobre os metadados (timestamps de commits, dados de PRs, etc.).
- **Criptografia:** Todos os dados são criptografados em trânsito (TLS 1.3) e em repouso (AES-256). As credenciais são armazenadas em um cofre dedicado com Módulos de Segurança de Hardware (HSM).
- **Controle de Acesso:** O plano Enterprise oferece suporte a SSO/SAML, e a plataforma disponibiliza autenticação de dois fatores (2FA) e controle de acesso baseado em função (RBAC).
- **Transferência Internacional de Dados:** Conforme a Política de Privacidade, os servidores da empresa estão localizados nos Estados Unidos, o que implica a transferência internacional de dados para clientes no Brasil [11].

## Referências

[1] [DevStats. Sobre Nós.](https://devstats.com/pt/about)
[2] [Caselli, R. (2023). DevStats MVP Design: Streamlining Engineering Management. Medium.](https://medium.com/@raonicaselli/devstats-mvp-design-streamlining-engineering-management-7fd2914bca6e)
[3] [DevStats. Página Principal.](https://devstats.com/pt)
[4] [DevStats. Funcionalidades.](https://devstats.com/pt/features)
[5] [DevStats. O que são as Métricas DORA.](https://www.devstats.com/blog/what-are-the-dora-metrics)
[6] [DevStats Docs. Settings.](https://docs.devstats.com/getting-started/settings)
[7] [DevStats. Preços (PT).](https://devstats.com/pt/pricing)
[8] [DevStats. Pricing (EN).](https://www.devstats.com/pricing)
[9] [DevStats Docs. AI Usage.](https://docs.devstats.com/metrics-and-definitions/ai-usage)
[10] [DevStats. Segurança.](https://devstats.com/pt/security)
[11] [DevStats. Política de Privacidade.](https://devstats.com/pt/privacy)
