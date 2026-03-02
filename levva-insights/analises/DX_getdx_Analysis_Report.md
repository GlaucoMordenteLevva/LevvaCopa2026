# Análise da Plataforma de Inteligência de Engenharia DX (getdx.com)

**Data:** 02 de Março de 2026
**Autor:** Manus AI

---

## Introdução

Este relatório apresenta uma análise detalhada da plataforma de inteligência de engenharia **DX**, disponível em [getdx.com](https://getdx.com). A análise foi conduzida com base nas informações públicas do site da empresa, bem como em fontes externas como Vendr, G2, Reddit e comparativos de mercado, para responder a seis questões estratégicas: métricas disponíveis, customização, preço (incluindo IOF para o Brasil), análise do uso de IA pelos desenvolvedores, segurança das informações e um resumo completo da plataforma.

Um fato relevante a ser considerado é que, em setembro de 2025, a DX foi adquirida pela **Atlassian**, o que sugere uma integração mais profunda com o ecossistema Atlassian (Jira, Confluence, Bitbucket) no futuro e pode impactar o modelo de preços e a estratégia de produto [1].

A DX se posiciona como a "plataforma de inteligência para desenvolvedores da era da IA" e conta com mais de 300 empresas clientes, incluindo nomes como Netflix, Pinterest, Block, Dropbox, Pfizer, Vanguard, eBay, Booking.com e GitHub [2].

---

## 1. Métricas Extraíveis

A DX oferece um conjunto robusto e multifacetado de métricas, combinando dados quantitativos extraídos de sistemas de engenharia com dados qualitativos coletados diretamente dos desenvolvedores. O framework central é o **DX Core 4**, que unifica os conhecidos frameworks DORA, SPACE e DevEx em quatro dimensões complementares [3].

### 1.1 DX Core 4

| Dimensão | Métrica Principal | Descrição |
|---|---|---|
| **Effectiveness** | Developer Experience Index (DXI) | Score composto por 14 fatores que medem a fricção e a satisfação do desenvolvedor no dia a dia. |
| **Speed** | PR Throughput | Quantidade de Pull Requests concluídos por semana, comparada com benchmarks da indústria (P50). |
| **Quality** | Change Fail Percentage | Percentual de alterações que resultam em falha na produção, indicador chave de qualidade de código. |
| **Impact** | Innovation Ratio | Proporção do tempo gasto em novas funcionalidades versus manutenção e correções. |

### 1.2 Developer Experience Index (DXI)

O DXI é um score composto por **14 drivers de eficiência de engenharia**, cada um avaliado individualmente. Esses drivers incluem: Ease of Release, Deep Work, Production Debugging, Build and Test, Documentation, Change Confidence, Planning Process, Incremental Delivery, Incident Handling e Customer Focus, entre outros. A plataforma traduz a fricção identificada em cada driver em termos financeiros (economia de tempo e dólares), permitindo que líderes priorizem investimentos com base em ROI. Como exemplo, a Block identificou mais de 500 mil horas de tempo de desenvolvedor recuperável utilizando o DXI [4].

### 1.3 TrueThroughput™

O **TrueThroughput™** é uma métrica proprietária que utiliza IA para avaliar a complexidade de cada Pull Request, atribuindo pesos automaticamente. Isso fornece uma medida de *output* significativamente mais precisa do que a simples contagem de PRs ou linhas de código, pois considera a real dificuldade e o valor do trabalho entregue [5].

### 1.4 Métricas Adicionais

A plataforma também oferece mais de **80 relatórios pré-construídos** no módulo SDLC Analytics, cobrindo métricas como PR cycle time, sprint analytics, engineering allocation (categorização automática do tipo de trabalho por IA: Features, Fixes, Maintenance) e R&D Capitalization. O módulo de Experience Sampling permite coletar feedback em tempo real dos desenvolvedores via Slack ou Teams, com métricas de taxa de resposta (tipicamente acima de 90%), score de satisfação e resumos gerados por IA dos comentários [6].

### 1.5 Industry Benchmarking

A DX mantém um dataset de mais de **10 milhões de amostras de benchmark**, segmentadas por tamanho da organização, indústria e geografia. Isso permite que as empresas comparem suas métricas não apenas com médias gerais, mas com pools customizados de empresas similares [3].

---

## 2. Customização

A plataforma DX apresenta um alto grau de customização, centrado na funcionalidade de **Custom Reporting** e na flexibilidade de seus dashboards.

> A capacidade de consultar dados usando linguagem natural ou SQL diretamente na plataforma permite que as equipes de engenharia criem relatórios e dashboards totalmente personalizados para suas necessidades específicas [7].

### 2.1 Custom Reporting

O editor de relatórios customizados permite que os usuários construam consultas a partir de diversas fontes de dados integradas, incluindo Claude Code, deployments, GitHub Copilot, incidents, Jira issues, pipeline runs e repositórios. A interface aceita tanto **linguagem natural** (processada por um LLM) quanto **consultas SQL diretas**, oferecendo flexibilidade tanto para líderes não técnicos quanto para analistas de dados. Os relatórios podem ser salvos como privados ou públicos, adicionados a dashboards customizáveis e exportados em formato CSV [7].

### 2.2 Integração com Ferramentas Externas

A DX permite o envio de dados para ferramentas externas de BI e data warehousing como **Looker**, **Snowflake** e **Spotify Backstage**, possibilitando que as organizações incorporem os dados da DX em seus fluxos de análise existentes. A plataforma conta com **mais de 55 conectores** nativos, abrangendo categorias como ferramentas de IA (GitHub Copilot, Cursor, Claude Code, Windsurf), CI/CD (Jenkins, CircleCI, GitHub Actions, GitLab), issue tracking (Jira, Linear, Asana, ClickUp), monitoramento (Datadog, New Relic, Dynatrace) e gestão de incidentes (PagerDuty, Opsgenie, Incident.io) [8].

### 2.3 Controle de Acesso e Governança

A plataforma permite um controle granular sobre quem pode visualizar relatórios ou dados específicos, com permissões baseadas em função (role-based). É importante destacar que os LLMs utilizados na funcionalidade de linguagem natural **nunca treinam nos dados do cliente**, garantindo a privacidade dos dados corporativos [7].

### 2.4 Experience Sampling Customizável

O módulo de Experience Sampling oferece templates out-of-the-box e a possibilidade de criar surveys totalmente customizados, com configurações ajustáveis de frequência e escopo. A API permite capturar insights sobre developer portals, CLI tools e web apps internos [6].

---

## 3. Preço e Considerações para o Brasil

### 3.1 Modelo de Preços

A DX não divulga seus preços publicamente, adotando um modelo de vendas consultivas ("Fale com Vendas"). As principais características do modelo de preços são:

| Aspecto | Detalhe |
|---|---|
| **Modelo de cobrança** | Modular, baseado em licenças por desenvolvedor + tiers de uso para acesso ao MCP server. |
| **Contrato mínimo** | 1 ano. Opções multi-ano flexíveis para empresas maiores. |
| **Desconto por volume** | Sim, para compras multi-produto e equipes maiores. |
| **Proof of Concept** | Oferecido sem custo para um subconjunto da organização. |
| **Serviços profissionais** | Onboarding, customer success, suporte dedicado e pacotes de serviços. |

### 3.2 Estimativas de Preço (Fontes Externas)

Dados do site Vendr, baseados em 14 transações reais, fornecem as seguintes estimativas [9]:

| Faixa | Valor Anual (USD) |
|---|---|
| **Mínimo** | $12,000 |
| **Médio** | $51,862 |
| **Máximo** | $180,000 |

Outra fonte estima que para empresas com 500 a 1.500 engenheiros, o custo pode variar de **$300,000 a $1 milhão anualmente** [10]. O Vendr também reporta que é possível obter um desconto de até 50% na renovação em troca de compromissos multi-ano.

### 3.3 Custo de IOF e Impostos no Brasil

Sendo a DX uma empresa americana sem operação local no Brasil, a contratação por uma empresa brasileira configura uma **importação de serviço/software**, sujeita a uma carga tributária significativa. A tabela abaixo resume os principais tributos aplicáveis:

| Tributo | Alíquota Estimada | Observação |
|---|---|---|
| **IOF** | 3,5% | Sobre operações de câmbio para compras internacionais [11]. |
| **IRRF** | 15% | Sobre remessas ao exterior (25% se o prestador estiver em paraíso fiscal). |
| **PIS-Importação** | 1,65% | Sobre o valor do serviço importado. |
| **COFINS-Importação** | 7,6% | Sobre o valor do serviço importado. |
| **ISS** | 2% a 5% | Depende do município onde a empresa contratante está sediada. |
| **CIDE** | 10% | Aplicável em alguns casos de transferência de tecnologia. |

A carga tributária total pode adicionar de **36% a 40%** sobre o valor do contrato, dependendo da classificação fiscal do serviço e do município. Isso significa que um contrato de $51,862 (valor médio) poderia custar efetivamente entre **$70,500 e $72,600** para uma empresa brasileira, sem considerar a variação cambial.

---

## 4. Análise do Uso de IA pelos Desenvolvedores

A DX possui uma suíte dedicada e extremamente detalhada para medir a adoção e o impacto de ferramentas de IA no desenvolvimento de software, denominada **AI Measurement**. Esta é uma das áreas onde a plataforma se destaca significativamente em relação aos concorrentes [12].

> A plataforma permite não apenas rastrear o uso de assistentes de IA como o GitHub Copilot, mas também analisar o código gerado em nível de linha, identificando o que é escrito por humanos versus o que é gerado por IA.

### 4.1 AI Usage Analytics

O módulo fornece um dashboard unificado para visualizar a adoção de diversas ferramentas de IA, com detalhamento por equipe, cargo e senioridade. As métricas incluem percentual de usuários ativos semanais (WAU%) por ferramenta, número de contribuidores ativos e tendências de adoção ao longo do tempo. Como exemplo, a plataforma pode mostrar que o Cursor tem 74% de contribuidores ativos, enquanto o GitHub Copilot tem 69% e o Windsurf 48%. Isso permite identificar *power users*, champions de adoção e licenças subutilizadas [13].

### 4.2 AI Code Metrics

Uma funcionalidade avançada (marcada como *Coming Soon* no momento da pesquisa) que promete rastrear em nível de linha o código gerado por IA. As métricas incluem: sugestões de IA aceitas, taxa de retenção do código AI, linhas modificadas após sugestão e percentual de código AI-generated por commit, PR e repositório. A plataforma reconhece que desenvolvedores frequentemente reescrevem ou descartam sugestões de IA antes de commitar, e por isso rastreia as "rewrites before commit" para oferecer uma visão realista da utilidade da IA [14].

### 4.3 AI Impact Analysis e Vendor Evaluation

O módulo de AI Impact Analysis correlaciona o aumento no uso de ferramentas de IA com métricas de produtividade (como as do DX Core 4), permitindo análises longitudinais e comparações "before vs. after". O Vendor Evaluation permite realizar testes A/B entre diferentes ferramentas de IA para tomar decisões de compra baseadas em dados de ROI, ajudando a "right-size" o investimento em IA [12].

### 4.4 AI Enablement

Além da medição, a DX oferece um módulo de **AI Enablement** que funciona como um "context engine" para engenharia AI-native. Ele inclui um Systems Catalog automatizado, Context Management para fornecer contexto architecture-aware para agents de IA, scorecards de AI Readiness e ferramentas de Agent Ops. A plataforma se conecta a agents via DX MCP (Model Context Protocol), governando suas ações com padrões de segurança organizacionais [15].

### 4.5 Resultados Reportados por Clientes

| Cliente | Resultado com IA |
|---|---|
| **Booking.com** | Aumento de 65% na adoção de IA pelos desenvolvedores. |
| **Workhuman** | Aumento de 21% no ROI de AI assistants. |
| **Grammarly** | Rastreamento e aumento da adoção de IA em toda a organização. |

---

## 5. Segurança das Informações

A DX demonstra um forte compromisso com a segurança, validado por múltiplas certificações internacionais e uma política de segurança transparente e detalhada, publicada em sua página de Security Measures [16].

### 5.1 Certificações e Compliance

| Certificação/Compliance | Detalhes |
|---|---|
| **SOC 2 Type 2** | Auditoria independente que valida controles de segurança, disponibilidade e confidencialidade. |
| **ISO/IEC 27001:2022** | Certificação internacional de gestão de segurança da informação. |
| **ISO/IEC 27701:2019** | Extensão da ISO 27001 focada em gestão de privacidade da informação. |
| **GDPR** | Conformidade com o Regulamento Geral de Proteção de Dados da União Europeia. |
| **CCPA** | Conformidade com a Lei de Privacidade do Consumidor da Califórnia. |
| **DPF** | Certificação no Data Privacy Framework (EU-US). |

### 5.2 Medidas Técnicas e Organizacionais

A DX implementa um conjunto abrangente de 15 categorias de medidas de segurança, conforme documentado publicamente e atualizado em novembro de 2025 [16]:

**Criptografia e Proteção de Dados**: Os dados são criptografados com **TLS 1.2+** em trânsito e **AES-256** em repouso. Os dados de clientes são logicamente segregados, e dados de produção nunca são utilizados em ambientes de não-produção.

**Controle de Acesso**: A plataforma implementa o princípio de menor privilégio, com MFA obrigatório para todos os funcionários, revisão trimestral de acessos e suporte a SSO via identity providers corporativos. Audit logs detalhados são mantidos em formato read-only.

**Avaliação e Testes**: Penetration testing é realizado anualmente por terceiros, complementado por vulnerability scans regulares e revisão de código seguindo o OWASP Top 10.

**Continuidade de Negócios**: Planos de DR/BC são testados anualmente, com backups diários dos dados.

**Gestão de Pessoal**: Background checks são realizados para todos os funcionários, e o acesso é revogado em até 24 horas após o desligamento.

**Retenção de Dados**: Os dados são retidos durante a vigência do contrato mais 30 dias após o término, quando são eliminados.

### 5.3 Ponto Crítico: Acesso ao Código-Fonte

Um aspecto fundamental para a decisão de adoção é que a DX **não acessa o código-fonte** dos clientes. Toda a análise é feita com base em **metadados** extraídos dos sistemas de engenharia (como timestamps de PRs, contagens de linhas, labels de issues, etc.), o que reduz significativamente o risco de exposição de propriedade intelectual [17].

### 5.4 Clientes de Referência em Segurança

A DX conta com clientes em setores altamente regulados, incluindo **BeyondTrust**, **Visa**, **Vanguard**, **HackerOne** e **Orca Security**, o que reforça a credibilidade de suas práticas de segurança [17].

---

## 6. Resumo Completo

### 6.1 Visão Geral da Plataforma

A DX é uma plataforma de inteligência de engenharia líder de mercado, classificada como **#1 no G2 Fall 2025 Grid** para Software Development Analytics Tools, com 93% de satisfação geral e 281 reviews [18]. Projetada pelos pesquisadores por trás dos frameworks SPACE e DevEx, ela se destaca por combinar métricas quantitativas de sistemas com dados qualitativos coletados diretamente dos desenvolvedores, oferecendo uma visão holística da produtividade e experiência de engenharia.

A plataforma é organizada em cinco pilares principais: Developer Experience, Engineering Productivity, AI Measurement, AI Enablement e DX AI (um copiloto de IA para líderes de engenharia que entrega insights e alerta sobre riscos automaticamente).

### 6.2 Integrações

A DX oferece mais de **55 conectores nativos** que abrangem praticamente todo o ecossistema de ferramentas de engenharia moderno, incluindo ferramentas de IA (GitHub Copilot, Cursor, Claude Code, Windsurf, Amazon Q, Sourcegraph Cody), plataformas Git (GitHub, GitLab, Bitbucket, Gerrit), CI/CD (Jenkins, CircleCI, GitHub Actions, ArgoCD, Buildkite), issue tracking (Jira, Linear, Asana, ClickUp, Shortcut), monitoramento (Datadog, New Relic, Dynatrace), e gestão de incidentes (PagerDuty, Opsgenie, Incident.io, Rootly, Firehydrant) [8].

### 6.3 Casos de Sucesso Documentados

| Cliente | Resultado |
|---|---|
| **Pfizer** | Economia de $5M/ano melhorando workflows de engenharia. |
| **SiriusXM** | $8M em ganhos de produtividade, economia de 4 FTEs. |
| **Block** | Identificação de 500k+ horas de tempo recuperável, 90%+ de taxa de resposta em surveys. |
| **Vercel** | Redução de 43% nos cycle times. |
| **Brex** | Economia de $5M refocando investimentos de engenharia. |
| **Vinted** | Aumento de 58% no PR throughput. |
| **Booking.com** | Aumento de 65% na adoção de IA. |
| **John Lewis** | Aumento de 40% no tempo efetivo de codificação. |
| **Recursion** | Redução de 33% em tech debt. |

### 6.4 Análise SWOT Resumida

| Forças | Fraquezas |
|---|---|
| Framework de métricas academicamente fundamentado (DX Core 4, DXI). | Preço não transparente e potencialmente elevado para empresas menores. |
| Análise de IA abrangente e granular (até nível de linha de código). | Algumas funcionalidades avançadas ainda em desenvolvimento (*Coming Soon*). |
| Segurança robusta com certificações SOC 2, ISO 27001 e 27701. | Falta de funcionalidades *out-of-the-box* em certas áreas (ex: resource allocation por headcount, goals tracking) [19]. |
| Customização profunda via SQL e linguagem natural. | Risco de uso inadequado das métricas para vigilância individual [20]. |
| Aquisição pela Atlassian fortalece posição de mercado. | Carga tributária elevada para empresas brasileiras (36-40% adicional). |

| Oportunidades | Ameaças |
|---|---|
| Integração nativa com ecossistema Atlassian (Jira, Confluence). | Concorrentes como Jellyfish, Sleuth e LinearB disputam o mesmo mercado. |
| Crescente demanda por medição de impacto de IA em engenharia. | Mudanças no modelo de preços pós-aquisição pela Atlassian. |
| Proof of Concept gratuito facilita a adoção. | Resistência cultural de desenvolvedores a ferramentas de métricas. |

### 6.5 Conclusão Final

A DX é uma ferramenta extremamente poderosa e sofisticada para organizações de engenharia maduras que buscam otimizar a produtividade e a experiência de seus desenvolvedores, especialmente no contexto da crescente adoção de IA. A aquisição pela Atlassian solidifica sua posição no mercado e promete uma integração ainda mais forte com ferramentas populares como Jira. Para uma fábrica de software brasileira, o principal desafio será o **custo total de aquisição**, que inclui não apenas o valor do contrato em dólares, mas também a significativa carga tributária de importação de serviços. Recomenda-se fortemente a realização de um **Proof of Concept** (oferecido gratuitamente pela DX) para avaliar o valor prático da ferramenta antes de um compromisso financeiro de longo prazo.

---

## Referências

[1] ICONIQ Capital. (2025, 18 de setembro). *DX Joins Atlassian: Powering Developer Intelligence for the AI Era*. [https://www.iconiqcapital.com/growth/insights/dx-joins-atlassian-powering-developer-intelligence-for-the-ai-era](https://www.iconiqcapital.com/growth/insights/dx-joins-atlassian-powering-developer-intelligence-for-the-ai-era)

[2] DX. (s.d.). *Customers*. [https://getdx.com/customers](https://getdx.com/customers)

[3] DX. (s.d.). *DX Core 4*. [https://getdx.com/dx-core-4](https://getdx.com/dx-core-4)

[4] DX. (s.d.). *Developer Experience Index*. [https://getdx.com/developer-experience-index](https://getdx.com/developer-experience-index)

[5] DX. (s.d.). *TrueThroughput™*. [https://getdx.com/truethroughput](https://getdx.com/truethroughput)

[6] DX. (s.d.). *Experience Sampling*. [https://getdx.com/experience-sampling](https://getdx.com/experience-sampling)

[7] DX. (s.d.). *Custom Reporting*. [https://getdx.com/custom-reporting](https://getdx.com/custom-reporting)

[8] DX. (s.d.). *Connectors*. [https://getdx.com/connectors/](https://getdx.com/connectors/)

[9] Vendr. (2025). *DX Software Pricing 2025*. [https://www.vendr.com/buyer-guides/dx](https://www.vendr.com/buyer-guides/dx)

[10] Exceeds.ai. (2026, 9 de fevereiro). *GetDX Enterprise Pricing 2026*. [https://blog.exceeds.ai/getdx-enterprise-pricing-guide/](https://blog.exceeds.ai/getdx-enterprise-pricing-guide/)

[11] Agência Brasil. (2025, 28 de junho). *Entenda como fica o IOF após derrubada de decreto*. [https://agenciabrasil.ebc.com.br/economia/noticia/2025-06/entenda-como-fica-o-iof-apos-derrubada-de-decreto](https://agenciabrasil.ebc.com.br/economia/noticia/2025-06/entenda-como-fica-o-iof-apos-derrubada-de-decreto)

[12] DX. (s.d.). *AI Measurement*. [https://getdx.com/ai-measurement](https://getdx.com/ai-measurement)

[13] DX. (s.d.). *Usage Analytics*. [https://getdx.com/usage-analytics](https://getdx.com/usage-analytics)

[14] DX. (s.d.). *AI Code Metrics*. [https://getdx.com/ai-code-metrics](https://getdx.com/ai-code-metrics)

[15] DX. (s.d.). *AI Enablement*. [https://getdx.com/ai-enablement](https://getdx.com/ai-enablement)

[16] DX. (2025, 5 de novembro). *DX's Technical and Organizational Measures*. [https://getdx.com/security-measures/](https://getdx.com/security-measures/)

[17] DX. (s.d.). *Security*. [https://getdx.com/security](https://getdx.com/security)

[18] G2. (2025). *DX Platform Reviews*. [https://www.g2.com/products/dx-platform/reviews](https://www.g2.com/products/dx-platform/reviews)

[19] Sleuth. (2025, 11 de março). *Sleuth vs. GetDX vs. Jellyfish*. [https://www.sleuth.io/post/sleuth-getdx-jellyfish/](https://www.sleuth.io/post/sleuth-getdx-jellyfish/)

[20] Reddit. (2025, 19 de novembro). *Developer productivity metrics(getdx)*. [https://www.reddit.com/r/ExperiencedDevs/comments/1p1lxsi/developer_productivity_metricsgetdx/](https://www.reddit.com/r/ExperiencedDevs/comments/1p1lxsi/developer_productivity_metricsgetdx/)
