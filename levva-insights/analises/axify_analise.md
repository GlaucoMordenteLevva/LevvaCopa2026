# Análise da Plataforma de Inteligência de Engenharia Axify

## Introdução

Este relatório apresenta uma análise detalhada da plataforma de inteligência de engenharia de software Axify, com base em informações públicas coletadas de seu site oficial (axify.io) e fontes externas. A análise foi estruturada para responder a questões específicas sobre métricas, customização, preços, análise de uso de IA, segurança da informação e um resumo completo da ferramenta.

## 1. Métricas Extraíveis

A Axify oferece um conjunto abrangente de métricas, com foco em eficiência, qualidade, e bem-estar das equipes de desenvolvimento. As métricas são agrupadas em categorias e dashboards específicos, sendo as principais:

| Categoria | Métricas Principais |
| :--- | :--- |
| **DORA Metrics** | Deployment Frequency, Lead Time for Changes, Change Failure Rate, Failed Deployment Recovery Time (MTTR). |
| **Métricas de Fluxo (VSM)** | Cycle Time (detalhado por fase), Work in Progress (WIP), Throughput, Work Item Age. |
| **Qualidade de Código** | Code Churn, Refactor Ratio, Defect Density, Test Coverage. |
| **Produtividade e Processo** | Pull Request Size, Time Spent in Review, Pull Request Merge Rate, Service Level Expectation (SLE), Workflow Stability. |
| **Bem-Estar da Equipe** | Métricas baseadas em 5 pilares: resiliência, motivação, inclusão, segurança e alinhamento. |
| **Impacto de IA** | Adoção de IA (uso, confiança, hábito), correlação do uso de IA com métricas de produtividade (cycle time, throughput, etc.). |

Além dessas, a plataforma oferece um dashboard geral de "Engineering Metrics" que consolida muitos desses indicadores, permitindo uma visão holística da saúde dos projetos e das equipes.

## 2. Customização

A plataforma Axify demonstra um bom nível de customização e flexibilidade para se adaptar a diferentes contextos de equipes e projetos.

- **Planos e Módulos:** A estrutura de preços é modular (Accelerate, AI Impact, Bundle), permitindo que as empresas contratem as funcionalidades que fazem mais sentido para suas necessidades. O plano Enterprise oferece a maior flexibilidade, com desenvolvimento customizado e a opção de instalação on-premise.
- **Value Stream Mapping (VSM):** A ferramenta de VSM permite a visualização e análise do ciclo de desenvolvimento de software de ponta a ponta. Os usuários podem customizar a visualização do período observado e analisar os tempos de ciclo por fase, o que indica a capacidade de adaptar o mapa ao fluxo de trabalho específico da equipe.
- **Integrações:** A Axify se integra com uma variedade de ferramentas populares de gerenciamento de projetos, SCM, CI/CD e comunicação, como Jira, Azure DevOps, GitHub, GitLab, Slack e Microsoft Teams. O uso de webhooks também sugere a possibilidade de integrações customizadas.
- **Relatórios e Dashboards:** Embora os dashboards principais pareçam padronizados, a capacidade de filtrar por equipes, projetos e períodos de tempo oferece um grau de customização na análise dos dados.

## 3. Preço e IOF

Os preços da Axify são transparentes e baseados no número de contribuidores ativos. A empresa opera com Dólares Americanos (USD) e Canadenses (CAD).

| Plano | Preço (USD/contribuidor/mês) | Mínimo de Contribuidores | Custo Mensal Mínimo (USD) |
| :--- | :--- | :--- | :--- |
| **Free Forever** | $0 | N/A | $0 |
| **Accelerate** | $19 | 5 | $95 |
| **AI Impact** | $19 | 5 | $95 |
| **Bundle** | $32 | 5 | $160 |
| **Enterprise** | Sob consulta | N/A | Sob consulta |

**Custo de IOF para Compras no Brasil:**

Como a Axify é uma empresa canadense e a cobrança é feita em moeda estrangeira (USD ou CAD), as transações para o Brasil estão sujeitas à tributação. A compra de software como serviço (SaaS) de empresas estrangeiras por meio de cartão de crédito internacional implica a cobrança do **Imposto sobre Operações Financeiras (IOF)**. A alíquota atual, padronizada desde 2025, é de **3,5%** sobre o valor da transação. Além do IOF, é importante considerar o spread cambial praticado pela instituição financeira do cartão de crédito, que pode adicionar um custo extra à conversão da moeda.

## 4. Análise do Uso de IA dos Desenvolvedores

Sim, a Axify possui uma funcionalidade robusta e dedicada para a análise do uso de IA, chamada **AI Adoption and Impact**. Este módulo vai além da simples contagem de licenças de ferramentas de IA e foca em medir o impacto real na produtividade e qualidade.

- **Métricas de Adoção:** A plataforma mede a adoção de IA com base em três dimensões definidas pelo DORA em seu relatório "State of AI-assisted Software Development":
    1.  **Uso Real:** Frequência e data da última utilização.
    2.  **Nível de Confiança:** Taxa de aceitação das sugestões geradas pela IA.
    3.  **Uso Habitual:** Número de interações com a ferramenta de IA.
- **Análise de Impacto:** A Axify correlaciona os dados de adoção de IA com métricas de engenharia (como cycle time, throughput, rework) para quantificar o impacto na performance. Isso permite comparar o desempenho de tarefas realizadas com e sem o auxílio de IA.
- **ROI e Ferramentas:** A funcionalidade permite calcular o ROI do investimento em assistentes de IA e rastrear o uso de ferramentas específicas como GitHub Copilot, Cursor e Claude Code, identificando quais geram mais valor.

## 5. Segurança das Informações

A Axify demonstra um forte compromisso com a segurança da informação, validado por certificações e práticas robustas.

- **Certificações e Compliance:** A plataforma possui a certificação **SOC 2 Type II** e é **compatível com o GDPR**, garantindo um alto padrão de segurança e privacidade de dados.
- **Proteção de Dados:** Os dados dos clientes são criptografados tanto em trânsito (TLS) quanto em repouso. A empresa segue as melhores práticas de desenvolvimento seguro, como as diretrizes do OWASP Top 10, e não acessa o código-fonte dos clientes, utilizando apenas metadados de pull requests e outros itens de trabalho.
- **Infraestrutura:** A infraestrutura da Axify é hospedada na AWS no Canadá, que por sua vez possui certificações SOC 1 e SOC 2. O acesso à infraestrutura é rigorosamente controlado por meio de VPN, chaves SSH e bastions.
- **Gestão de Acesso:** O acesso interno é gerenciado via AWS SSO com autenticação multifator, e os tokens de acesso dos clientes são criptografados e inacessíveis para a equipe de desenvolvimento.

## 6. Resumo Completo

A Axify se posiciona como uma plataforma de inteligência de engenharia de software completa e madura, projetada para fornecer visibilidade e insights acionáveis para líderes de engenharia, produto e operações. Sua principal força reside na capacidade de correlacionar uma vasta gama de métricas de processo e qualidade com o bem-estar da equipe e, mais recentemente, com o impacto da inteligência artificial no ciclo de desenvolvimento.

A estrutura de preços modular, incluindo um plano gratuito funcional, torna a ferramenta acessível para equipes de diferentes tamanhos. A funcionalidade de análise de IA é um diferencial significativo, permitindo que as organizações meçam o ROI real de seus investimentos em ferramentas de IA para desenvolvedores.

Do ponto de vista de segurança, a certificação SOC 2 Type II e a conformidade com o GDPR, aliadas a uma arquitetura segura na AWS, transmitem confiança para empresas que manuseiam dados sensíveis. Para empresas no Brasil, o principal ponto de atenção é o custo adicional de IOF e taxas de câmbio na contratação do serviço.

Em suma, a Axify é uma ferramenta poderosa para organizações que buscam otimizar seus processos de desenvolvimento de software com base em dados, melhorar a produtividade e a satisfação de suas equipes, e navegar estrategicamente na era da IA no desenvolvimento de senvolvimento de software.

