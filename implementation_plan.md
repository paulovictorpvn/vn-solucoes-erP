# Evolução VN Soluções — Gestão do Site, Equipe Interna, Fluxo de Caixa & Retaguarda Didática

Este plano estrutura a criação do módulo central de **Configurações do Site, Credenciais e Equipe Interna da VN**, a implantação do módulo dedicado de **Fluxo de Caixa (Diário/Mensal, Previsto vs. Realizado e Projeção)** por empresa cliente, e a reorganização da **Retaguarda VN Gestão** com guias didáticos passo a passo e fluxos de alta produtividade.

## User Review & Critical Decisions

> [!IMPORTANT]
> As escolhas confirmadas abaixo orientam a implementação e refletem exatamente as prioridades definidas para a operação da VN Soluções.

- **Decisão Confirmada 1 — Central de Configurações do Site & Gestão de Usuários Internos da VN**: Um módulo administrativo unificado onde a direção da VN controla em tempo real os textos, contatos/WhatsApp, links da Bio do Instagram, serviços exibidos, perguntas frequentes (FAQ), regras do programa de parcerias, visibilidade das seções, cores de destaque, credenciais das empresas clientes e o **cadastro/permissões dos colaboradores internos da VN Soluções** que operam o sistema.
- **Decisão Confirmada 2 — Módulo Dedicado de Fluxo de Caixa por Empresa Cliente**: Painel financeiro completo com alternância entre visão **Diária e Mensal**, comparativo lado a lado de **Previsto vs. Realizado**, **Projeção de Saldo Bancário** para 15/30/60/90 dias, alertas de descasamento de caixa e lançamento rápido integrado tanto na retaguarda quanto na Área do Cliente.
- **Decisão Recomendada 3 — Estrutura Didática e Produtiva da Retaguarda**: Reorganização do menu lateral por jornada operacional BPO com contadores ao vivo, barra de comando rápida no topo e um **Guia Didático Passo a Passo ("Como usar este módulo em 3 passos")** integrado ao cabeçalho de cada tela para orientar analistas e supervisores sem fricção.

---

## 1. Overview & Core Concept

- **O Que Entrega**:
  1. **Módulo de Configurações do Site, Acessos & Equipe VN**: Permite editar qualquer conteúdo público do site institucional sem tocar em código, emitir e revogar senhas exclusivas das empresas clientes e gerenciar a equipe interna da VN (analistas, supervisores, gestores) com definição de alçada e carteira de clientes atribuída.
  2. **Módulo de Fluxo de Caixa Multiempresa e por Cliente**: Oferece controle diário e mensal de entradas, saídas, saldo inicial, saldo operacional do dia e saldo acumulado projetado, destacando variações entre o valor previsto e o efetivamente realizado/conciliado.
  3. **Retaguarda Reestruturada e Didática**: Transforma a experiência operacional com navegação intuitiva, instruções práticas passo a passo em cada módulo, atalhos diretos de criação de lançamentos e zero erros de sincronização.
- **Público-Alvo**:
  - **Diretoria e Gestores da VN Soluções**: governança da equipe interna, rentabilidade da carteira, personalização do site comercial e liberação de acessos.
  - **Supervisores e Analistas BPO da VN**: operação diária de contas a pagar/receber, fluxo de caixa, conciliação, fechamento de DRE e atendimento de chamados.
  - **Empresas Clientes e Parceiros**: acesso ao site público (via link da Bio/redes sociais) e à Área do Cliente autenticada para consulta de fluxo de caixa, DRE e aprovação de lotes.

---

## 2. User Experience & Visual Design

- **Fluxos Principais do Usuário**:
  1. **Gestão de Equipe Interna da VN e Credenciais de Clientes**: O gestor acessa *Configurações do Site & Acessos*, cadastra um novo analista ou supervisor da VN, define seu perfil de acesso (Gestor, Supervisor, Analista BPO, Comercial), vincula quais empresas clientes ele atende e gera seu login interno. Na aba vizinha, gera o kit de acesso exclusivo de uma empresa cliente para envio via WhatsApp.
  2. **Personalização Instantânea do Site & Links Sociais**: O gestor altera o número de WhatsApp oficial, edita o título Hero, ativa/desativa seções do site (ex.: *Diagnóstico*, *Programa de Parcerias*, *FAQ*), edita itens de serviços ou perguntas frequentes e vê a mudança refletida imediatamente no Website Público (`?view=site`).
  3. **Operação do Fluxo de Caixa (Diário/Mensal e Previsto vs. Realizado)**: O analista seleciona a empresa cliente, escolhe a visão *Diária* ou *Mensal*, analisa o gráfico de evolução de saldo e a grade detalhada com colunas de *Entradas Previstas*, *Entradas Realizadas*, *Saídas Previstas*, *Saídas Realizadas*, *Geração Líquida de Caixa* e *Saldo Final Projetado*, podendo registrar ou liquidar um título direto da tela.
  4. **Navegação Guiada e Didática**: Ao entrar em qualquer módulo da retaguarda, o colaborador visualiza um painel didático enxuto com o passo a passo da rotina (Passo 1 -> Passo 2 -> Passo 3) e botões de ação direta que executam a tarefa ou levam ao próximo estágio do processo.

- **Identidade Visual & Tema**:
  - *Direção Estética*: SaaS Financeiro Corporativo de Alta Precisão combinado com a identidade oficial da VN Soluções.
  - *Paleta de Cores*:
    - `--navy`: `#052557` (Azul Marinho Institucional VN)
    - `--dark`: `#031B4A` (Fundo da barra lateral e cabeçalhos executivos)
    - `--blue`: `#0571ED` (Ações primárias, destaques de navegação e indicadores de liquidez)
    - `--org`: `#FA670D` (Acentos de conversão, alertas prioritários e chamadas de ação)
    - `--surf`: `#F4F7FB` (Superfície limpa de alto contraste para leitura confortável de tabelas)
    - Cartões puros em `#FFFFFF` com bordas sutis `#E2E8F0`.
  - *Tipografia & Hierarquia*: `Plus Jakarta Sans` para títulos e interface operacional, `Caveat` para destaques institucionais da marca no site e cabeçalho, e `JetBrains Mono` com `tabular-nums` para todos os valores monetários, saldos de caixa, protocolos e códigos fiscais.

---

## 3. Key Product Decisions & Trade-Offs

- **Decisão 1: Configurações Dinâmicas do Site + Gestão de Equipe Interna em Tempo Real**
  - *Abordagem Escolhida*: Centralizar tanto o CMS do Website quanto a gestão de usuários internos da VN e credenciais de clientes em um estado compartilhado e persistido, refletindo alterações instantaneamente no Website Público e no cabeçalho de alçadas da retaguarda.
  - *Por Quê*: Permite que a própria equipe da VN atualize campanhas do Instagram, telefones, serviços e acessos de novos colaboradores ou clientes em segundos, sem depender de manutenção técnica.
- **Decisão 2: Motor de Fluxo de Caixa Conectado aos Lançamentos Reais**
  - *Abordagem Escolhida*: Calcular o Fluxo de Caixa Diário, Mensal e a Projeção futura diretamente a partir da base viva de Contas a Receber, Contas a Pagar, Lotes e Conciliações de cada empresa cliente, somado ao saldo bancário inicial configurável por cliente.
  - *Por Quê*: Garante integridade contábil absoluta — qualquer boleto incluído, editado ou baixado atualiza imediatamente o fluxo de caixa na retaguarda e no Portal do Cliente.

---

## 4. Technical Architecture & Data Strategy

### Diagrama de Arquitetura e Módulos

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                       PLATAFORMA INTEGRADA VN SOLUÇÕES                           │
├───────────────────────────┬──────────────────────────┬───────────────────────────┤
│   RETAGUARDA VN GESTÃO    │  FLUXO DE CAIXA CLIENTE  │  SITE & GESTÃO DE ACESSOS │
│  (Menu Didático + Guias)  │ (Diário/Mensal/Projeção) │ (CMS + Equipe VN + Portal)│
└─────────────┬─────────────┴────────────┬─────────────┴─────────────┬─────────────┘
              │                          │                           │
              ▼                          ▼                           ▼
┌───────────────────────────┐ ┌────────────────────────┐ ┌─────────────────────────┐
│ Guia Passo a Passo (1-2-3)│ │ Previsto vs. Realizado │ │ Editor Visual do Site   │
│ + Atalhos de Produtividade│ │ + Saldo Inicial Banco  │ │ (Textos, Bio, FAQ, Cor) │
│ + Seletor de Operador VN  │ │ + Simulador 15/30/60d  │ │ + Visibilidade Seções   │
└─────────────┬─────────────┘ └──────────┬─────────────┘ └───────────┬─────────────┘
              │                          │                           │
              └──────────────────────────┼───────────────────────────┘
                                         ▼
┌──────────────────────────────────────────────────────────────────────────────────┐
│           MOTOR DE DADOS & API EXPRESS + POSTGRESQL / ESTADO SINCRONIZADO        │
│ • Empresas Clientes, Contratos, Plano de Contas e Lançamentos (Pagar / Receber)  │
│ • Equipe Interna VN (Colaboradores, Cargos, Alçadas SoD, Carteira de Clientes)   │
│ • Credenciais Exclusivas de Clientes (Usuário, Senha, Código VN-AUTH)            │
│ • Configurações do Website Institucional & Chamados com Protocolo VN-AAMMDD      │
└──────────────────────────────────────────────────────────────────────────────────┘
```

### Modelo de Dados e Mapeamento de Estado Interativo

1. **Equipe Interna da VN Soluções (`VnStaffMember`)**:
   - Campos: `id`, `code`, `name`, `email`, `role` (`gestor` | `supervisor` | `analista` | `comercial` | `engenharia`), `department`, `assignedClientIds`, `status` (`Ativo` | `Férias` | `Bloqueado`), `accessPin`, `lastActiveAt`.
   - Interações: Criar novo colaborador da VN, editar cargo/alçada, vincular empresas clientes sob sua responsabilidade, ativar/bloquear acesso e alternar o operador ativo na barra superior da retaguarda.
2. **Configurações do Website Institucional (`WebsiteCmsConfig`)**:
   - Campos: `heroBadge`, `heroTitle`, `heroSubtitle`, `whatsappNumber`, `commercialEmail`, `instagramHandle`, `addressText`, `accentColor`, `partnerBonusPercent`, `visibleSections` (controle individual de *Quem Somos*, *Princípios*, *Serviços*, *Metodologia*, *Parcerias*, *Diagnóstico*, *Atendimento*, *Guia Rápido* e *FAQ*), além das listas editáveis de `services` e `faqs`.
   - Interações: Edição em tempo real por abas, botões de ligar/desligar seções, adição/remoção de perguntas frequentes ou serviços, e restauração dos padrões originais com 1 clique.
3. **Fluxo de Caixa por Empresa Cliente (`CashFlowModule`)**:
   - Modos de visualização: *Diário (Dia a Dia)*, *Mensal (Consolidado por Competência)* e *Projeção de Liquidez (15, 30, 60 e 90 dias)*.
   - Visão *Previsto vs. Realizado*: separa títulos liquidados/conciliados (*Realizado*) de títulos em aberto/agendados (*Previsto*), exibindo percentual de realização, geração líquida de caixa, ajuste de saldo inicial por conta bancária, lançamento rápido de entrada/saída e exportação/impressão do relatório para o cliente.
