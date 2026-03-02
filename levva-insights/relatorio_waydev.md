# Análise da Plataforma de Inteligência de Engenharia Waydev

**Data:** 02 de Março de 2026

## 1. Resumo Completo

A Waydev é uma plataforma de **Inteligência de Engenharia de Software (Software Engineering Intelligence - SEI)** projetada para fornecer a líderes de engenharia, gerentes e executivos visibilidade sobre o processo de desenvolvimento de software. A plataforma se conecta a diversas ferramentas do ciclo de vida de desenvolvimento (SDLC), como repositórios Git, sistemas de tickets e plataformas de CI/CD, para coletar metadados e gerar insights acionáveis. O objetivo principal é alinhar o trabalho de engenharia com as prioridades de negócio, otimizar a alocação de recursos, acelerar a entrega e melhorar a produtividade geral da equipe de desenvolvimento, sem a necessidade de inputs manuais dos desenvolvedores.

A plataforma se baseia em frameworks reconhecidos pela indústria, como **DORA Metrics** e **SPACE Framework**, para fornecer uma análise completa da performance. Além disso, a Waydev se destaca por suas funcionalidades de análise de adoção de ferramentas de IA (como GitHub Copilot), customização de dashboards e métricas, e um forte compromisso com a segurança, evidenciado pela sua certificação SOC 3. A empresa, co-fundada por Alex Circei e apoiada pela Y Combinator, atende desde pequenas equipes até grandes corporações, incluindo empresas da Fortune 500, com opções de hospedagem na nuvem e on-premise.

## 2. Métricas Extraíveis

A Waydev oferece um conjunto extenso de mais de 70 métricas, que podem ser categorizadas para uma análise detalhada do desempenho da engenharia. A lista completa de métricas foi extraída da documentação oficial e pode ser consultada no arquivo `notas_metricas_completas.md`.

| Categoria | Métricas Principais |
| :--- | :--- |
| **DORA Metrics** | Deployment Frequency, Lead Time for Changes, Change Failure Rate, Mean Time to Recovery (MTTR). |
| **Cycle Time** | Análise detalhada do tempo gasto em cada estágio do desenvolvimento, desde o primeiro commit até o deploy, incluindo tempo de revisão, iteração e espera. |
| **Pull Requests** | Volume de PRs (abertos, fechados, merged), tempo de vida, taxas de falha, métricas de revisão (comentários, tempo para primeira revisão), PRs sem revisão, etc. |
| **Throughput & Efficiency** | Linhas de Código (LoC) por tipo (novo, refatorado, churn), eficiência (relação entre código produtivo e total), e a métrica `tt100` (tempo para 100 alterações). |
| **Atividade do Dev** | Dias de codificação, dias ativos, frequência de commits, e padrões de trabalho semanal. |
| **Análise de Risco** | Classificação de commits por nível de risco (baixo, médio, alto) com base em seu tamanho e impacto. |
| **Alinhamento com Negócio** | Métricas de planejamento como Resource Allocation, Project Costs, e Cost Capitalization. |
| **Análise de Sprints** | Métricas de Sprints Commitment e Velocity Report para acompanhamento de metodologias ágeis. |

## 3. Customização

A customização é um ponto forte da plataforma, especialmente nos planos mais avançados (Premium e Enterprise), através do **Studio Module**.

- **Custom Dashboards:** Permite que os usuários criem painéis de controle totalmente personalizados. É possível selecionar entre mais de 70 métricas, organizar widgets com layouts flexíveis e escolher diferentes tipos de visualização (gráficos, tabelas, heatmaps) para focar nos indicadores mais relevantes para a organização.

- **Custom Metrics:** Usuários podem criar suas próprias métricas usando fórmulas personalizadas. Isso permite alinhar a análise diretamente com os KPIs e objetivos estratégicos específicos da empresa, indo além das métricas pré-definidas.

- **Custom Reports:** Capacidade de construir relatórios complexos utilizando qualquer métrica disponível na plataforma.

- **Targets & Notifications:** É possível definir metas para as equipes e configurar notificações automáticas (via Slack ou email) para acompanhar o progresso e celebrar marcos importantes.

- **Role Management:** O plano Enterprise oferece gerenciamento de papéis e permissões, permitindo controlar quem tem acesso a quais dados e dashboards, garantindo segurança e simplicidade na gestão.

## 4. Preço

A Waydev opera com um modelo de preço por contribuidor ativo, cobrado anualmente. Usuários operacionais (gerentes, executivos) são gratuitos, limitados a 10% do número de contribuidores pagos.

| Plano | Preço (por contribuidor/mês) | Principais Características |
| :--- | :--- | :--- |
| **Pro** | $29 | Funções essenciais de visibilidade, módulos Delivery e Health, 50 repositórios, 6 meses de retenção de dados. |
| **Premium** | $54 | Todas as features do Pro, mais módulos Planning e Automation, DORA e DX, API, AI Adoption, dashboards limitados, 300 repositórios, 36 meses de retenção. |
| **Enterprise** | Customizado | Todas as features do Premium, mais Studio Module completo, AI Predictability, SSO, Self-hosting (on-premise), repositórios e retenção ilimitados, suporte premium. |

### Custo de IOF para Compras no Brasil

Como a Waydev é uma empresa sediada nos EUA e a cobrança é feita em dólares (USD) através do Stripe, a transação é considerada uma compra internacional. Com base na legislação brasileira (Decreto nº 12.466 de 2025), incidirá uma alíquota de **IOF (Imposto sobre Operações Financeiras) de 3,5%** sobre o valor total da assinatura. É importante notar que, além do IOF, outros tributos de importação de serviço como IRRF, PIS/COFINS-Importação e ISS podem ser aplicáveis, dependendo da estrutura fiscal da empresa contratante.

## 5. Análise do Uso de IA dos Devs

Sim, a Waydev possui uma funcionalidade dedicada a isso, chamada **AI Adoption**, disponível nos planos Premium e Enterprise. Esta funcionalidade permite medir o impacto e o retorno sobre o investimento (ROI) de ferramentas de IA generativa no processo de desenvolvimento.

- **Ferramentas Monitoradas:** A plataforma rastreia o uso de ferramentas como **GitHub Copilot, Cursor, Claude, Windsurf** e métricas nativas da própria Waydev.

- **Métricas de Adoção e Uso:**
    - **Engajamento:** Mede usuários ativos e engajados, identificando quem está de fato utilizando as ferramentas de IA.
    - **Taxa de Adoção:** Mostra a porcentagem da equipe que adotou as ferramentas.
    - **Silent Users:** Identifica desenvolvedores que interagem com a IA (recebem sugestões) mas não as aceitam.
    - **Uso Efetivo:** Analisa a quantidade de sugestões de código geradas, a taxa de aceitação e o volume de código aceito.

- **Análise de Impacto:** A plataforma permite comparar métricas de engenharia (como Cycle Time, Churn, Coding Time) **antes e depois** da adoção da IA, fornecendo uma visão clara do impacto na produtividade e eficiência.

## 6. Segurança das Informações

A segurança é um dos principais focos da Waydev, que possui a certificação **SOC 3**, o que atesta um alto nível de confiança e transparência em seus controles de segurança, disponibilidade e confidencialidade.

- **Tratamento de Código-Fonte:** A Waydev **não armazena cópias do código-fonte** dos repositórios. A plataforma realiza um `bare clone` para extrair apenas os metadados da pasta `.git` e deleta essa pasta em tempo real logo após a análise. Nenhum código é persistido nos servidores da Waydev.

- **Transmissão e Autenticação:** A conexão com os provedores Git é feita exclusivamente via **tokens de acesso temporários (OAuth)**, que são rotacionados frequentemente. Toda a comunicação é criptografada com SSL de 256 bits (HTTPS).

- **Hospedagem e Acesso:** A infraestrutura é hospedada na AWS. O plano Enterprise oferece a opção de **hospedagem on-premise (self-hosted)**, dando ao cliente controle total sobre o ambiente. A plataforma também possui controle de acesso rigoroso, com destaque para o **SSO/SAML** e **2FA** disponíveis.

- **Compliance com GDPR:** A política de privacidade da Waydev menciona a implementação de medidas técnicas e organizacionais para proteger dados pessoais, indicando conformidade com regulações de privacidade como o GDPR.

- **Segurança de Pagamentos:** Os pagamentos são processados pela **Stripe**, que possui certificação PCI Service Provider Level 1, o mais alto padrão da indústria de pagamentos.

---

### Referências

[1] Waydev Official Website. (https://waydev.co)
[2] Waydev Pricing Page. (https://waydev.co/pricing/)
[3] Waydev Security Page. (https://waydev.co/security/)
[4] Waydev AI Adoption Page. (https://waydev.co/ai-adoption/)
[5] Waydev Integrations Page. (https://waydev.co/integrations/)
[6] Waydev Documentation - Security. (https://docs.waydev.co/docs/security)
[7] Waydev Capterra Reviews. (https://www.capterra.com/p/179273/Waydev/reviews/)
[8] PayPro Global - Brazil's IOF Tax Changes. (https://blog.payproglobal.com/pt-br/brazils-iof-tax-changes)
