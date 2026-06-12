# Product Backlog — Inversia Marketplace de Oportunidades

**Projeto:** Inversia (protótipo ResolvAI)  
**Período acadêmico:** 2026.1 (03/02 – 17/06/2026)  
**Última atualização:** Junho/2026  
**Documento relacionado:** [SPRINT_PLANNING.md](SPRINT_PLANNING.md)

---

## Visão do produto

O **Inversia** é um marketplace digital de serviços de manutenção residencial (infiltração, alvenaria, hidráulica, impermeabilização, pintura) que conecta **contratantes** e **prestadores** de forma rápida, transparente e segura.

O diferencial do protótipo **ResolvAI** inclui IA conversacional para estruturação de escopos, propostas padronizadas, smart contracts, pagamento com retenção (escrow) e painel administrativo para curadoria e disputas.

**Meta do semestre:** validar o modelo de negócio por meio de artefatos de engenharia de software e protótipos WEB e MOBILE de alta fidelidade navegáveis — sem desenvolvimento de backend em produção.

---

## Equipe

| Integrante | Papel principal | Foco de entrega |
|------------|-----------------|-----------------|
| **Danilo** | Product Owner / Gestão | Backlog, sprint planning, PM Canvas, documentação, apresentações |
| **Ygor** | UX/Dev — Visão Contratante | `cliente.html`, `cliente-web.html`, fluxos C1–C11 |
| **Rafael** | UX/Dev — Visão Prestador | `fornecedor.html`, `fornecedor-web.html`, fluxos P1–P9 |
| **Gabriel** | UX/Dev — Admin e Integração | `admim.html`, `index.html`, consistência de dados, correções transversais |

---

## Glossário

| Termo | Definição |
|-------|-----------|
| **Contratante / Cliente** | Usuário que publica demanda de serviço e contrata prestadores |
| **Prestador / Fornecedor** | Profissional autônomo ou empresa que envia propostas e executa serviços |
| **Escrow** | Retenção do pagamento até confirmação de conclusão pelo contratante |
| **Smart Contract** | Contrato digital gerado automaticamente com escopo, termos e assinatura |
| **Escopo** | Descrição estruturada do serviço, gerada via chat com IA no protótipo |
| **Proposta padronizada** | Oferta com preço, prazo, descrição e garantia obrigatória |
| **PM Canvas** | Product Management Canvas — artefato de concepção do produto |
| **Story Point (SP)** | Unidade de estimativa de esforço relativo (Fibonacci: 1, 2, 3, 5, 8) |

---

## Critérios de priorização

### MoSCoW (escopo do semestre)

| Prioridade | Critério |
|------------|----------|
| **Must** | Artefatos de concepção, requisitos, backlog, sprint plan, protótipos WEB e MOBILE navegáveis, apresentações nas datas de avaliação |
| **Should** | Correções de `Correções_Prototipo.txt`, consistência de dados entre views, documentação completa |
| **Could** | Telas admin avançadas (A5–A6), animações, polish visual extra |
| **Won't (semestre)** | Backend, APIs reais, deploy em produção, blockchain on-chain |

### Ordem de desempate

1. Marco acadêmico mais próximo  
2. Dependência bloqueante para outras stories  
3. Valor para demonstração nas avaliações  

---

## Épicos por fase acadêmica

| Epic | Fase | Tema | Período | Stories |
|------|------|------|---------|---------|
| **E01** | Concepção | Ideação, definição do projeto e PM Canvas | Fev/2026 | US-001 – US-008 |
| **E02** | Concepção | Processo de software, ferramentas e elicitação | Fev/2026 | US-009 – US-014 |
| **E03** | Planejamento | Escopo, requisitos e gestão de riscos | Mar/2026 | US-015 – US-017, US-020 |
| **E04** | Planejamento | Product Backlog, sprint planning e métricas | Mar/2026 | US-018 – US-019 |
| **E05** | Protótipo WEB | Visão Administrador (A1–A6) | Abr/2026 | US-027, US-028, US-036 |
| **E06** | Protótipo WEB | Visão Contratante web (C1–C11) | Abr/2026 | US-029 – US-033 |
| **E07** | Protótipo WEB | Visão Prestador web (P1–P9) | Abr/2026 | US-034 – US-035 |
| **E08** | Protótipo MOBILE | Visão Contratante mobile (C1–C11) | Mai/2026 | US-039 – US-040, US-043 |
| **E09** | Protótipo MOBILE | Visão Prestador mobile (P1–P9) | Mai/2026 | US-044 – US-045 |
| **E10** | Validação | Correções, consistência, documentação e avaliações | Mai–Jun/2026 | US-021 – US-026, US-038, US-041 – US-054 |

---

## User Stories

### E01 — Ideação e Definição do Projeto (Sprint 1)

#### US-001 — Definir problema e proposta de valor Inversia
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** Product Owner, **quero** documentar o problema e a proposta de valor do Inversia, **para** alinhar a equipe e comunicar o projeto à turma.
- **Critérios de aceite:**
  1. Problema central descrito (5 dores de `DECLARACAO_DE_NECESSIDADES.md` §3).
  2. Proposta de valor diferenciada (IA, escrow, smart contract).
  3. Documento revisado por todos os integrantes.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** Declaração §2–§3 | Cronograma 12/02

#### US-002 — Mapear stakeholders e personas
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe de produto, **quero** mapear stakeholders e personas (cliente, prestador, admin), **para** orientar requisitos e protótipos.
- **Critérios de aceite:**
  1. Três personas documentadas com necessidades principais.
  2. Stakeholders internos e externos identificados (Declaração §4).
  3. Personas vinculadas às três visões do protótipo.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** Declaração §4 | Cronograma 12/02

#### US-003 — Pesquisa de mercado e concorrentes
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** pesquisar o mercado de manutenção residencial e concorrentes, **para** definir diferenciação e nicho regional.
- **Critérios de aceite:**
  1. Mínimo de 3 concorrentes ou alternativas mapeados.
  2. Nicho geográfico definido (Fortaleza/CE).
  3. Diferenciais do Inversia documentados frente à concorrência.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** Declaração §10 (risco competitivo) | Cronograma 12/02

#### US-004 — Definir escopo inicial do MVP e nicho
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** definir o escopo inicial do MVP e categorias de serviço, **para** limitar o protótipo ao nicho de manutenção residencial.
- **Critérios de aceite:**
  1. Categorias de serviço listadas (infiltração, alvenaria, hidráulica, impermeabilização, pintura).
  2. Escopo MVP alinhado às 13 necessidades funcionais (Declaração §5).
  3. Itens fora de escopo do semestre explicitados.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** Declaração §5 | documentação.md §O que é

#### US-005 — Formar equipe e definir papéis
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 2
- **Como** equipe, **quero** formalizar papéis (Danilo, Ygor, Rafael, Gabriel), **para** distribuir responsabilidades nas sprints.
- **Critérios de aceite:**
  1. Papéis documentados neste backlog e em `SPRINT_PLANNING.md`.
  2. Acordo da equipe sobre responsabilidades por visão do protótipo.
  3. Canal de comunicação da equipe definido.
- **Marco:** Formação de equipes — 05/02
- **Fonte:** Cronograma 05/02

#### US-006 — Preparar pitch de apresentação
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Todos
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** preparar pitch de apresentação, **para** expor a ideia Inversia à turma em 12/02.
- **Critérios de aceite:**
  1. Apresentação com problema, solução, personas e escopo.
  2. Duração adequada ao tempo da aula.
  3. Todos os integrantes participam da apresentação.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** Cronograma 12/02

#### US-007 — Esboço inicial de jornada do usuário
- **Épico:** E01
- **Fase acadêmica:** Concepção
- **Sprint:** 1
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Como** UX, **quero** esboçar a jornada do contratante (publicação → proposta → contratação → avaliação), **para** guiar o protótipo.
- **Critérios de aceite:**
  1. Jornada do contratante com etapas principais documentadas.
  2. Jornada do prestador esboçada (descoberta → proposta → execução).
  3. Fluxo alinhado às telas C1–C11 e P1–P9.
- **Marco:** Apresentação das ideias — 12/02
- **Fonte:** documentação.md §Fluxos | Cronograma 12/02

---

### E02 — PM Canvas, Processo e Ferramentas (Sprint 2)

#### US-008 — Construir PM Canvas completo
- **Épico:** E01/E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** Product Owner, **quero** construir o PM Canvas, **para** consolidar visão, métricas, stakeholders e riscos do produto.
- **Critérios de aceite:**
  1. PM Canvas com blocos preenchidos (proposta, personas, jornada, métricas, canais, parceiros, recursos, custos, receita).
  2. Modelo de receita documentado (taxa 8–12%, Plano Pro, juros parcelamento).
  3. Artefato apresentável ao professor.
- **Marco:** Construção do PM Canvas — 24/02 e 26/02
- **Fonte:** Cronograma 24/02, 26/02 | documentação.md §Modelo de Negócio

#### US-009 — Definir processo de software
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** definir o processo de software (Scrum adaptado ao semestre), **para** orientar sprints e cerimônias.
- **Critérios de aceite:**
  1. Processo documentado com sprints de 2 semanas.
  2. Cerimônias definidas (planning, review, retrospectiva adaptadas às aulas).
  3. DoR e DoD referenciados em `SPRINT_PLANNING.md`.
- **Marco:** Processo de software — 19/02
- **Fonte:** Cronograma 19/02 — Processo de software

#### US-010 — Selecionar stack do protótipo
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 2
- **Como** desenvolvedor, **quero** selecionar e documentar a stack do protótipo (HTML/CSS/JS puro), **para** construir protótipos navegáveis sem backend.
- **Critérios de aceite:**
  1. Stack definida: HTML, CSS, JavaScript, Google Fonts (Inter).
  2. Stack futura documentada (FastAPI, PostgreSQL, React Native) como Won't do semestre.
  3. Justificativa de escolha registrada.
- **Marco:** Ferramentas e técnicas — 05/02, 19/02
- **Fonte:** documentação.md §Contexto | Cronograma — Ferramentas e técnicas do projeto

#### US-011 — Técnicas de elicitação de requisitos
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Como** analista, **quero** aplicar técnicas de elicitação (entrevistas, questionários), **para** validar necessidades dos usuários.
- **Critérios de aceite:**
  1. Pelo menos uma técnica aplicada e documentada.
  2. Resultados incorporados à Declaração de Necessidades ou backlog.
  3. Registro de participantes ou fontes consultadas.
- **Marco:** Elicitação de requisitos — 26/02
- **Fonte:** Cronograma 26/02 — Elicitação de requisitos

#### US-012 — Mapa de stakeholders (Orbital)
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Rafael
- **Prioridade:** Should
- **Story Points:** 3
- **Como** equipe, **quero** construir mapa orbital de stakeholders, **para** visualizar influência e interesse de cada parte.
- **Critérios de aceite:**
  1. Mapa com clientes, prestadores, admin, parceiros de pagamento/geo, equipe interna.
  2. Estratégia de engajamento por quadrante documentada.
  3. Alinhado à Declaração §4.
- **Marco:** PM Canvas — 26/02
- **Fonte:** Declaração §4 | Orbital_Stakeholder_Strategy (referência externa)

#### US-013 — Matriz de riscos inicial
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** elaborar matriz de riscos inicial, **para** antecipar ameaças ao projeto acadêmico e ao produto.
- **Critérios de aceite:**
  1. Mínimo de 6 riscos mapeados (Declaração §10).
  2. Probabilidade e impacto definidos por risco.
  3. Ações de mitigação preliminares documentadas.
- **Marco:** Gerenciamento de riscos — 03/03
- **Fonte:** Declaração §10 | Cronograma 03/03 — Gerenciamento de riscos

#### US-014 — Definir paleta de cores e design system
- **Épico:** E02
- **Fase acadêmica:** Concepção
- **Sprint:** 2
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Como** UX, **quero** definir paleta e design system das três visões, **para** garantir consistência visual nos protótipos.
- **Critérios de aceite:**
  1. Cores por visão: Contratante `#2563EB`, Prestador `#FF5C1A`, Admin `#7B5EA7`.
  2. Cores compartilhadas e tipografia Inter documentadas.
  3. Guia aplicável a mobile (375×812) e web desktop.
- **Marco:** Preparação protótipo — Sprint 4
- **Fonte:** documentação.md §Paleta de Cores

---

### E03 — Escopo, Requisitos e Riscos (Sprint 3)

#### US-015 — Redigir Declaração de Necessidades
- **Épico:** E03
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** Product Owner, **quero** redigir a Declaração de Necessidades consolidada, **para** formalizar requisitos de negócio e produto.
- **Critérios de aceite:**
  1. Documento `DECLARACAO_DE_NECESSIDADES.md` completo com 13 necessidades funcionais.
  2. NFRs, riscos, premissas e critérios de sucesso incluídos.
  3. Revisado e aprovado pela equipe.
- **Marco:** Avaliação Fase Concepção — 05/03
- **Fonte:** Declaração completa | Cronograma 05/03

#### US-016 — Identificar requisitos funcionais (13 itens MVP)
- **Épico:** E03
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 5
- **Como** analista, **quero** identificar e detalhar os 13 requisitos funcionais do MVP, **para** rastrear implementação nos protótipos.
- **Critérios de aceite:**
  1. Cada requisito (Declaração §5.1–5.13) com descrição e critério verificável.
  2. Mapeamento requisito → tela(s) do protótipo.
  3. Matriz de rastreabilidade iniciada.
- **Marco:** Identificação de requisitos — 12/03, 17/03
- **Fonte:** Declaração §5 | Cronograma — Identificação de requisitos

#### US-017 — Identificar requisitos não funcionais
- **Épico:** E03
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 3
- **Como** analista, **quero** documentar requisitos não funcionais, **para** orientar qualidade do protótipo e evolução futura.
- **Critérios de aceite:**
  1. NFRs de confiabilidade, segurança, usabilidade e escalabilidade documentados (Declaração §6).
  2. NFRs aplicáveis ao protótipo (responsividade, intuitividade) destacados.
  3. NFRs de produção marcados como pós-semestre.
- **Marco:** Identificação de requisitos — 17/03
- **Fonte:** Declaração §6

#### US-020 — Refinar matriz de riscos com mitigações
- **Épico:** E03
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** refinar a matriz de riscos com planos de mitigação, **para** reduzir impacto no cronograma acadêmico.
- **Critérios de aceite:**
  1. Cada risco crítico (Declaração §10) com ação de mitigação e responsável.
  2. Riscos acadêmicos (atraso de entrega, escopo inflado) incluídos.
  3. Matriz atualizada e referenciada neste backlog (seção Riscos).
- **Marco:** Gerenciamento de riscos — 03/03, 24/03
- **Fonte:** Declaração §10 | Cronograma — Gerenciamento de riscos

---

### E04 — Product Backlog e Sprint Planning (Sprint 3)

#### US-018 — Gerar Product Backlog
- **Épico:** E04
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** Product Owner, **quero** gerar o Product Backlog completo, **para** priorizar e estimar o trabalho do semestre.
- **Critérios de aceite:**
  1. Arquivo `PRODUCT_BACKLOG.md` com épicos, 54 user stories, MoSCoW e SP.
  2. Stories rastreáveis a requisitos, telas e marcos acadêmicos.
  3. Backlog revisado pela equipe.
- **Marco:** Planejamento — 03/03
- **Fonte:** Cronograma 03/03 | Este documento

#### US-019 — Gerar Sprint Planning
- **Épico:** E04
- **Fase acadêmica:** Planejamento
- **Sprint:** 3
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** Product Owner, **quero** gerar o planejamento de sprints, **para** distribuir tarefas entre Danilo, Ygor, Rafael e Gabriel.
- **Critérios de aceite:**
  1. Arquivo `SPRINT_PLANNING.md` com 9 sprints, datas, marcos e responsáveis.
  2. Capacidade ~20–24 SP/sprint documentada.
  3. Referências cruzadas com este backlog.
- **Marco:** Planejamento — 03/03
- **Fonte:** Cronograma 03/03 | SPRINT_PLANNING.md

---

### E10 (parcial) — Refinamento e Validação (Sprint 4)

#### US-021 — Documentar user stories detalhadas
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** Product Owner, **quero** detalhar user stories com critérios de aceite completos, **para** guiar construção dos protótipos.
- **Critérios de aceite:**
  1. Stories de protótipo (Sprints 5–8) com critérios testáveis.
  2. Formato consistente em todo o backlog.
  3. Dependências entre stories identificadas.
- **Marco:** Ativos metodológicos — 10/03, 31/03
- **Fonte:** Cronograma — Construção dos ativos metodológicos

#### US-022 — Validar requisitos com professor e colegas
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Todos
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** validar requisitos com professor e colegas, **para** confirmar aderência antes da Avaliação 1.
- **Critérios de aceite:**
  1. Feedback de validação registrado.
  2. Ajustes incorporados ao backlog ou Declaração.
  3. Checklist de validação de artefatos concluído.
- **Marco:** Validação — 26/03, 31/03
- **Fonte:** Cronograma 26/03, 31/03 — Validação de artefatos

#### US-023 — Verificar rastreabilidade requisito → story → tela
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** analista, **quero** verificar rastreabilidade entre requisitos, stories e telas, **para** garantir cobertura completa.
- **Critérios de aceite:**
  1. Matriz requisito (RF-01–RF-13) → story → tela preenchida.
  2. Lacunas identificadas e endereçadas no backlog.
  3. Documento de rastreabilidade no repositório.
- **Marco:** Verificação — 26/03
- **Fonte:** Declaração §5 | Cronograma — Verificação de requisitos

#### US-024 — Wireframes de baixa fidelidade (3 visões)
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 5
- **Como** UX, **quero** criar wireframes de baixa fidelidade das três visões, **para** acelerar construção do protótipo de alta fidelidade.
- **Critérios de aceite:**
  1. Wireframes das jornadas principais: contratante, prestador, admin.
  2. Fluxos de navegação indicados.
  3. Aprovados pela equipe antes da Sprint 5.
- **Marco:** Preparação Avaliação 1 — 07/04
- **Fonte:** Cronograma 03/03–04/04

#### US-025 — Estrutura inicial index.html e navegação entre visões
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** desenvolvedor, **quero** implementar `index.html` com navegação entre visões, **para** servir como entrada do protótipo.
- **Critérios de aceite:**
  1. Página de entrada com escolha entre Contratante, Prestador e Admin.
  2. Links para versões mobile e web onde aplicável.
  3. Navegação funcional no browser.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** VisualizacaoPrototipo/index.html

#### US-026 — Preparar apresentação Avaliação 1
- **Épico:** E10
- **Fase acadêmica:** Planejamento
- **Sprint:** 4
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** preparar apresentação da Avaliação 1, **para** demonstrar artefatos de requisitos e início do protótipo WEB.
- **Critérios de aceite:**
  1. Slides com requisitos, backlog, sprint plan e demo parcial.
  2. Roteiro de demonstração definido.
  3. Material pronto até 07/04.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** Cronograma 07/04

---

### E05 — Protótipo WEB: Administrador (Sprints 5–6)

#### US-027 — Admin A1 Dashboard (KPIs, funil, heatmap)
- **Épico:** E05
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 5
- **Requisito:** RF-13 (Painel administrativo)
- **Como** administrador, **quero** visualizar dashboard com KPIs, funil de conversão e mapa de calor, **para** monitorar a operação da plataforma.
- **Critérios de aceite:**
  1. Tela A1 com 5 KPIs, funil, gráfico semanal e alertas.
  2. Mapa de calor por região (Fortaleza).
  3. Navegação via sidebar funcional.
  4. Tema roxo `#7B5EA7` aplicado.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** documentação.md A1 | admim.html

#### US-028 — Admin A2 Gestão de Prestadores (curadoria)
- **Épico:** E05
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 5
- **Requisito:** RF-13
- **Como** administrador, **quero** aprovar ou rejeitar prestadores com pré-validação IA, **para** garantir qualidade da rede.
- **Critérios de aceite:**
  1. Tela A2 com tabela de prestadores e status.
  2. Ações: aprovar, rejeitar, solicitar documentação.
  3. Indicador de pré-validação IA visível.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** documentação.md A2 | regra de negócio #10

#### US-036 — Admin A3–A6 (contratos, disputas, jurídico, rede)
- **Épico:** E05
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 6
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 5
- **Requisito:** RF-13
- **Como** administrador, **quero** monitorar contratos, mediar disputas, escalar casos jurídicos e analisar crescimento da rede, **para** operar a plataforma ponta a ponta.
- **Critérios de aceite:**
  1. A3: tabela de contratos com indicador de risco e escrow total.
  2. A4: central de disputas com prazo 30 dias e painel 3 colunas.
  3. A5: gestão jurídica com exportação PDF e timeline.
  4. A6: análise de rede com mapa de calor e gaps de oferta.
- **Marco:** Protótipo WEB completo — 30/04
- **Fonte:** documentação.md A3–A6

---

### E06 — Protótipo WEB: Contratante (Sprints 5–6)

#### US-029 — Cliente web C1–C2 (splash, home)
- **Épico:** E06
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Requisito:** RF-01 (Cadastro/login)
- **Como** contratante web, **quero** acessar onboarding e home com pedidos ativos, **para** iniciar ou acompanhar demandas.
- **Critérios de aceite:**
  1. C1: splash/onboarding com proposta de valor.
  2. C2: home com saudação, CTA "Criar pedido com IA" e lista de pedidos.
  3. Layout web desktop responsivo, tema azul.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** documentação.md C1–C2 | cliente-web.html

#### US-030 — Cliente web C3–C4 (chat IA, escopo gerado)
- **Épico:** E06
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 5
- **Requisito:** RF-02 (Publicação de pedido)
- **Como** contratante, **quero** criar escopo via chat com IA e revisar antes de publicar, **para** registrar demanda com clareza.
- **Critérios de aceite:**
  1. C3: chat conversacional com chips, upload de fotos e barra de progresso.
  2. C4: escopo estruturado com galeria, localização (endereço completo) e botão publicar.
  3. Localização exibe endereço residencial, não descrição física do problema (Correções Problema 6).
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** documentação.md C3–C4 | regra #1

#### US-031 — Cliente web C5 (feed de propostas)
- **Épico:** E06
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Requisito:** RF-05 (Comparação de propostas)
- **Como** contratante, **quero** visualizar feed de propostas recebidas com filtros, **para** avaliar opções de prestadores.
- **Critérios de aceite:**
  1. Cards com preço, prazo, garantia e avaliação.
  2. Filtros e opção de comparar até 3 propostas.
  3. Ordenação por avaliação, preço e prazo funcional.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** documentação.md C5 | Correções (ordenação)

#### US-032 — Apresentação Avaliação 1 (07/04)
- **Épico:** E10
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 5
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** apresentar artefatos de requisitos e início do protótipo WEB, **para** cumprir a Avaliação 1.
- **Critérios de aceite:**
  1. Apresentação conduzida em 07/04 com requisitos, backlog e demo parcial.
  2. Admin A1–A2 e Cliente C1–C5 demonstrados.
  3. Feedback do professor registrado.
- **Marco:** Avaliação 1 — 07/04
- **Fonte:** Cronograma 07/04

#### US-033 — Cliente web C6–C11 (detalhe, comparar, chat, contrato, checkout, avaliação)
- **Épico:** E06
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 6
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-05, RF-06, RF-07, RF-08
- **Como** contratante, **quero** comparar propostas, alinhar com prestador, assinar contrato, pagar e avaliar, **para** concluir a jornada de contratação.
- **Critérios de aceite:**
  1. C6: detalhe com perfil, portfólio e avaliações corretas por prestador.
  2. C7: comparação lado a lado (2–3 colunas).
  3. C8: chat/alinhamento com botão "Prosseguir para contrato".
  4. C9: smart contract com assinatura; botões separados de assinar e ir para pagamento (Correções Problema 10).
  5. C10: checkout PIX (QR code), cartão (campos), parcelamento só no cartão; sem boleto.
  6. C11: confirmação de pagamento antes de home; avaliação pós-conclusão.
  7. Fluxo C5 → C6 → C8 → C9 → C10 → confirmação (Correções Problema 9, 13).
- **Marco:** Protótipo WEB completo — 30/04
- **Fonte:** documentação.md C6–C11 | Correções Problemas 1–4, 8–13

---

### E07 — Protótipo WEB: Prestador (Sprint 6)

#### US-034 — Prestador web P1–P5 (onboarding, feed, detalhe, proposta, status)
- **Épico:** E07
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 6
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-01, RF-03, RF-04, RF-09
- **Como** prestador web, **quero** me cadastrar, ver pedidos filtrados, enviar proposta e acompanhar status, **para** captar e converter oportunidades.
- **Critérios de aceite:**
  1. P1: onboarding em 3 passos (dados, categorias/regiões, documentos).
  2. P2: feed com KPIs, filtros por categoria funcionais e cards de compatibilidade.
  3. P3: detalhe do pedido com escopo, galeria e info do cliente.
  4. P4: envio de proposta com preço, prazo, descrição e garantia obrigatória.
  5. P5: minhas propostas com status Enviada/Visualizada/Escolhida e filtros funcionais.
- **Marco:** Protótipo WEB completo — 30/04
- **Fonte:** documentação.md P1–P5 | fornecedor-web.html

#### US-035 — Prestador web P6–P9 (chat, contrato, andamento, recebimento)
- **Épico:** E07
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 6
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 5
- **Requisitos:** RF-06, RF-07, RF-08, RF-12
- **Como** prestador, **quero** alinhar com cliente, assinar contrato, executar serviço e receber pagamento, **para** completar o ciclo de prestação.
- **Critérios de aceite:**
  1. P6: chat com checklist e prosseguir para contrato.
  2. P7: smart contract com obrigações e assinatura.
  3. P8: serviço em andamento com timeline de marcos.
  4. P9: recebimento com resumo financeiro (bruto/taxa/líquido) e avaliação do cliente.
- **Marco:** Protótipo WEB completo — 30/04
- **Fonte:** documentação.md P6–P9

#### US-037 — Integrar navegação web e consistência visual
- **Épico:** E05/E06/E07
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 6
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** integrar navegação entre telas web e garantir consistência visual, **para** entregar protótipo WEB navegável coeso.
- **Critérios de aceite:**
  1. Todos os fluxos web navegáveis sem links quebrados.
  2. Dados mock consistentes entre cliente-web e fornecedor-web (preço, endereço Fortaleza, garantia, prazo).
  3. Design system aplicado uniformemente.
- **Dependências:** US-033, US-034, US-035, US-036
- **Marco:** Avaliação 2 — 05/05
- **Fonte:** Correções Problemas 14–18

---

### E08 — Protótipo MOBILE: Contratante (Sprints 7–8)

#### US-038 — Revisão final protótipo WEB antes da Avaliação 2
- **Épico:** E10
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 7
- **Responsável:** Todos
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** revisar e corrigir o protótipo WEB, **para** apresentá-lo na Avaliação 2.
- **Critérios de aceite:**
  1. Checklist de navegação web concluído.
  2. Bugs críticos web resolvidos.
  3. Demo ensaiada para 05/05.
- **Marco:** Avaliação 2 — 05/05
- **Fonte:** Cronograma 05/05

#### US-039 — Cliente mobile C1–C4 (onboarding, home, chat IA, escopo)
- **Épico:** E08
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 7
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-01, RF-02
- **Como** contratante mobile, **quero** onboarding, home, chat IA e revisão de escopo no phone frame, **para** criar pedidos pelo celular.
- **Critérios de aceite:**
  1. Phone frame 375×812px com bottom nav (Home, Chat IA, Pedidos, Alertas, Perfil).
  2. C1–C4 implementadas conforme documentação.md.
  3. Menu de navegação oculto antes do login/cadastro (Correções §Mobile Cliente).
  4. Botões do chat IA sem distorção visual.
- **Marco:** Avaliação 2 — 05/05 (paralelo)
- **Fonte:** documentação.md C1–C4 | cliente.html

#### US-040 — Cliente mobile C5–C7 (propostas, detalhe, comparar)
- **Épico:** E08
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 7
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-05, RF-06
- **Como** contratante mobile, **quero** receber, detalhar e comparar propostas, **para** escolher o melhor prestador.
- **Critérios de aceite:**
  1. C5: feed com ordenação funcional; empty state quando não há propostas.
  2. C6: "Ver perfil" exibe prestador correto do card selecionado.
  3. C7: comparação lado a lado; botão "Escolher" segue fluxo C6 → C8 → C9.
  4. Pedido "Aguardando Proposta" abre empty state, não feed de propostas.
- **Marco:** Sprint 7
- **Fonte:** documentação.md C5–C7 | Correções §Mobile Cliente

#### US-043 — Cliente mobile C8–C11 (chat, contrato, pagamento, confirmação)
- **Épico:** E08
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 8
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-06, RF-07, RF-08
- **Como** contratante mobile, **quero** alinhar, assinar, pagar e acompanhar serviço, **para** concluir contratação pelo celular.
- **Critérios de aceite:**
  1. C8: chat/alinhamento; "Enviar mensagem" vai para chat, não contrato.
  2. C9: contrato scrollável; assinatura única; botão "Ir para pagamento".
  3. C10: PIX com QR e chave; cartão com campos; parcelamento só no cartão; sem boleto.
  4. Confirmação de pagamento antes de home; "Acompanhar pedido" vai para timeline, não avaliação.
  5. Aba Pedidos exibe histórico de pedidos, não propostas recebidas.
- **Marco:** Apresentação Mobile — 21/05
- **Fonte:** documentação.md C8–C11 | Correções Problemas 1–9

---

### E09 — Protótipo MOBILE: Prestador (Sprint 8)

#### US-044 — Prestador mobile P1–P5 (cadastro, feed, detalhe, proposta, status)
- **Épico:** E09
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 8
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 8
- **Requisitos:** RF-01, RF-03, RF-04
- **Como** prestador mobile, **quero** login/cadastro, feed filtrado, envio e acompanhamento de propostas, **para** operar pelo celular.
- **Critérios de aceite:**
  1. P1: opções "Criar Conta" e "Fazer Login" na entrada.
  2. P2: filtros por categoria (Hidráulica etc.) funcionais; detalhes variados por pedido.
  3. Home exibe pedidos abertos; aba Pedidos exibe em andamento/aceitos.
  4. P5: filtros Enviadas/Escolhidas funcionais.
- **Marco:** Apresentação Mobile — 21/05
- **Fonte:** documentação.md P1–P5 | Correções §Mobile Prestador

#### US-045 — Prestador mobile P6–P9 (chat, contrato, andamento, recebimento)
- **Épico:** E09
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 8
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 5
- **Requisitos:** RF-06, RF-07, RF-08, RF-12
- **Como** prestador mobile, **quero** chat, contrato, execução e recebimento no celular, **para** completar serviços em campo.
- **Critérios de aceite:**
  1. P6–P7: chat e contrato navegáveis.
  2. P8: serviço em andamento acessível a partir de pedido "Em andamento".
  3. P9: recebimento e avaliação do cliente.
  4. Aba Chat lista pedidos em andamento com chat por pedido.
- **Marco:** Apresentação Mobile — 21/05
- **Fonte:** documentação.md P6–P9

---

### E10 — Validação, Correções e Encerramento (Sprints 7–9)

#### US-041 — Apresentação protótipos WEB
- **Épico:** E10
- **Fase acadêmica:** Protótipo WEB
- **Sprint:** 7
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** apresentar protótipos WEB navegáveis, **para** cumprir a Avaliação 2.
- **Critérios de aceite:**
  1. Demo das três visões web conduzida em 05/05.
  2. Fluxos principais demonstrados ao professor.
  3. Feedback registrado para correções.
- **Marco:** Avaliação 2 — 05/05
- **Fonte:** Cronograma 05/05

#### US-042 — Documentação parcial do protótipo
- **Épico:** E10
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 7
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** equipe, **quero** documentar telas, fluxos e regras de negócio, **para** facilitar validação e manutenção.
- **Critérios de aceite:**
  1. `VisualizacaoPrototipo/documentação.md` atualizado com telas web e mobile.
  2. Fluxos de navegação documentados por visão.
  3. Regras de negócio listadas.
- **Marco:** Sprint 7
- **Fonte:** documentação.md

#### US-046 — Correções críticas de navegação e pagamento
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 8
- **Responsável:** Gabriel
- **Prioridade:** Should
- **Story Points:** 5
- **Como** equipe, **quero** corrigir problemas críticos de navegação, PIX, cartão e fluxo Escolher, **para** melhorar fidelidade do protótipo.
- **Critérios de aceite:**
  1. Problemas 1–4, 8–9, 11–13 de `Correções_Prototipo.txt` resolvidos.
  2. Fluxo C5 → C6 → C8 → C9 respeitado em mobile e web.
  3. PIX exibe QR code; boleto removido; parcelamento condicional.
- **Marco:** Avaliação 3 — 28/05
- **Fonte:** Correções_Prototipo.txt Problemas 1–13

#### US-047 — Unificar dados mock entre views
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 8
- **Responsável:** Gabriel
- **Prioridade:** Should
- **Story Points:** 3
- **Como** equipe, **quero** unificar dados mock (preço, endereço, garantia, prazo, nome), **para** eliminar inconsistências entre mobile e web.
- **Critérios de aceite:**
  1. Preço único por serviço em todas as views (Problema 14).
  2. Endereço Fortaleza/CE consistente (Problema 15).
  3. Garantia, nome do prestador e prazo unificados (Problemas 16–18).
- **Marco:** Avaliação 3 — 28/05
- **Fonte:** Correções_Prototipo.txt Problemas 14–18

#### US-048 — Apresentação protótipos Mobile
- **Épico:** E10
- **Fase acadêmica:** Protótipo MOBILE
- **Sprint:** 8
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** apresentar protótipos mobile navegáveis, **para** cumprir apresentação de 21/05.
- **Critérios de aceite:**
  1. Demo mobile contratante e prestador em 21/05.
  2. Phone frames demonstrados corretamente.
  3. Feedback registrado.
- **Marco:** Apresentação Mobile — 21/05
- **Fonte:** Cronograma 21/05

#### US-049 — Verificar requisitos implementados nos protótipos
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Gabriel
- **Prioridade:** Must
- **Story Points:** 5
- **Como** analista, **quero** verificar se os 13 requisitos funcionais estão representados nos protótipos, **para** confirmar a verificação de requisitos do projeto.
- **Critérios de aceite:**
  1. Matriz RF-01–RF-13 × tela × status (implementado/parcial/não aplicável).
  2. Lacunas documentadas com justificativa.
  3. Relatório de verificação no repositório.
- **Marco:** Avaliações 4 e 5 — 02/06, 09/06, 11/06
- **Fonte:** Declaração §5 | Cronograma — Verificação de requisitos

#### US-050 — Validar artefatos com usuários e colegas
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Ygor
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** validar protótipos com usuários ou colegas, **para** confirmar a validação de artefatos do projeto.
- **Critérios de aceite:**
  1. Sessão de validação realizada ou simulada com registro.
  2. Feedback consolidado e priorizado.
  3. Ajustes críticos encaminhados ao backlog.
- **Marco:** Avaliações 4 e 5
- **Fonte:** Cronograma — Validação de artefatos

#### US-051 — Correções finais pós-avaliação
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Rafael
- **Prioridade:** Must
- **Story Points:** 5
- **Como** equipe, **quero** aplicar correções finais após avaliações, **para** concluir a avaliação dos protótipos do projeto.
- **Critérios de aceite:**
  1. Itens de feedback do professor endereçados ou documentados como wont-fix.
  2. Protótipo estável para demonstração final.
  3. Regressões evitadas em fluxos core.
- **Marco:** Avaliação 3 — 28/05; Avaliações 4 e 5
- **Fonte:** Cronograma — Avaliação dos protótipos

#### US-052 — Finalizar documentação completa do repositório
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 5
- **Como** equipe, **quero** consolidar toda a documentação do repositório, **para** entregar projeto completo em 17/06.
- **Critérios de aceite:**
  1. Backlog, sprint plan, declaração e documentação do protótipo atualizados.
  2. Índice ou guia de navegação do repositório.
  3. Artefatos referenciados e rastreáveis.
- **Marco:** Fim do período — 17/06
- **Fonte:** Cronograma 18/06

#### US-053 — Preparar apresentação final e incorporar feedback
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Danilo
- **Prioridade:** Must
- **Story Points:** 3
- **Como** equipe, **quero** preparar apresentação final e incorporar feedback de 16/06, **para** encerrar o projeto.
- **Critérios de aceite:**
  1. Apresentação final com visão completa do semestre.
  2. Feedback de 16/06 incorporado ou respondido.
  3. Todos os integrantes participam.
- **Marco:** Feedback — 16/06
- **Fonte:** Cronograma 16/06

#### US-054 — Aprovação da solução (checklist de aprovação)
- **Épico:** E10
- **Fase acadêmica:** Validação
- **Sprint:** 9
- **Responsável:** Todos
- **Prioridade:** Must
- **Story Points:** 2
- **Como** equipe, **quero** concluir checklist de aprovação da solução, **para** formalizar entrega do projeto.
- **Critérios de aceite:**
  1. Checklist de aprovação da solução preenchido (requisitos, protótipos, documentação, avaliações).
  2. Aprovação registrada pela equipe.
  3. Repositório pronto para submissão final.
- **Marco:** Aprovação — 02/06, 09/06, 11/06
- **Fonte:** Cronograma — Aprovação da solução

---

## Matriz de rastreabilidade — Requisitos funcionais (RF)

| ID | Requisito (Declaração §5) | Stories principais | Telas |
|----|---------------------------|-------------------|-------|
| RF-01 | Cadastro, login e recuperação de senha | US-029, US-034, US-039, US-044 | C1, P1 |
| RF-02 | Publicação de pedido de serviço | US-030, US-039 | C3–C4 |
| RF-03 | Descoberta por geo/categoria/filtros | US-034, US-044 | P2 |
| RF-04 | Envio e gestão de propostas | US-034, US-044 | P4–P5 |
| RF-05 | Comparação de propostas | US-031, US-033, US-040 | C5–C7 |
| RF-06 | Aceite de proposta e início | US-033, US-043 | C6–C9, P6–P7 |
| RF-07 | Chat pós-aceite | US-033, US-035, US-043, US-045 | C8, P6 |
| RF-08 | Avaliação pós-serviço | US-033, US-043, US-045 | C11, P9 |
| RF-09 | Perfil do prestador | US-034, US-044 | C6, P1 |
| RF-10 | Notificações de oportunidades | Protótipo (Alertas nav) | C2 nav |
| RF-11 | Edição/cancelamento de pedidos | Could — protótipo parcial | C2 |
| RF-12 | Histórico de serviços | US-043, US-045 | C2 Pedidos, P8 |
| RF-13 | Painel administrativo | US-027, US-028, US-036 | A1–A6 |

---

## Matriz de rastreabilidade — Correções do protótipo

| Problema | Descrição resumida | Story | Status esperado |
|----------|-------------------|-------|-----------------|
| 1 | PIX sem QR Code | US-046 | Corrigir Sprint 8 |
| 2 | Boleto deve ser removido | US-046 | Corrigir Sprint 8 |
| 3 | Parcelamento condicional ao cartão | US-046 | Corrigir Sprint 8 |
| 4 | "Acompanhar pedido" vai para rating | US-043 | Corrigir Sprint 8 |
| 5 | Aba Pedidos deveria exibir histórico | US-043 | Corrigir Sprint 8 |
| 6 | Localização incorreta no escopo | US-030 | Corrigir Sprint 5/6 |
| 7 | Smart Contract difícil de visualizar | US-043 | Corrigir Sprint 8 |
| 8 | Chat completo onde deveria haver verificação | US-033 | Corrigir Sprint 6 |
| 9 | Botão "Escolher" pula etapas | US-046 | Corrigir Sprint 8 |
| 10 | Botão "Assinar contrato e pagar" (web) | US-033 | Corrigir Sprint 6 |
| 11 | PIX sem QR Code (web) | US-046 | Corrigir Sprint 8 |
| 12 | Cartão sem campos (web) | US-033 | Corrigir Sprint 6 |
| 13 | Confirmação de pagamento pulada (web) | US-033 | Corrigir Sprint 6 |
| 14 | Preço divergente mobile/web | US-047 | Corrigir Sprint 8 |
| 15 | Endereço divergente | US-047 | Corrigir Sprint 8 |
| 16 | Garantia divergente | US-047 | Corrigir Sprint 8 |
| 17 | Nome do prestador divergente | US-047 | Corrigir Sprint 8 |
| 18 | Prazo divergente | US-047 | Corrigir Sprint 8 |

---

## Backlog futuro pós-semestre (Won't now)

Itens derivados de `documentação.md` §Contexto de Desenvolvimento, fora do escopo acadêmico 2026.1:

| ID | Item | Prioridade futura |
|----|------|-------------------|
| BF-01 | Backend API REST com FastAPI | Must |
| BF-02 | Banco de dados PostgreSQL | Must |
| BF-03 | App mobile React Native | Must |
| BF-04 | Integração real gateway de pagamento (PIX/cartão) | Must |
| BF-05 | Integração APIs de geolocalização | Should |
| BF-06 | IA conversacional real para escopo | Should |
| BF-07 | Smart contract on-chain (blockchain) | Could |
| BF-08 | Notificações push em produção | Should |
| BF-09 | Deploy e CI/CD em ambiente cloud | Must |
| BF-10 | Testes automatizados E2E | Should |

---

## NFRs e riscos

### Requisitos não funcionais (Declaração §6)

| ID | Categoria | Requisito | Aplicável ao semestre |
|----|-----------|-----------|----------------------|
| NFR-01 | Desempenho | Tempo de resposta adequado | Parcial (protótipo local) |
| NFR-02 | Disponibilidade | Alta disponibilidade operacional | Won't (sem produção) |
| NFR-03 | Segurança | Proteção de dados de autenticação | Won't (sem backend) |
| NFR-04 | Usabilidade | Interface intuitiva e responsiva | **Must** |
| NFR-05 | Usabilidade | Onboarding simples | **Must** |
| NFR-06 | Escalabilidade | Arquitetura evolutiva | Documentar apenas |
| NFR-07 | Observabilidade | Logs, latência, erros | Won't (sem produção) |

### Riscos mapeados (Declaração §10)

| Risco | Impacto | Mitigação | Responsável |
|-------|---------|-----------|-------------|
| Baixa adesão de prestadores | Alto | Foco em nicho Fortaleza; curadoria no admin | Danilo |
| Baixa adesão de clientes | Alto | Protótipo demonstrável; jornada simplificada | Ygor |
| Matching impreciso | Médio | Filtros geo/categoria no protótipo | Rafael |
| Fraude / má-fé | Médio | Fluxo de curadoria A2; escrow simulado | Gabriel |
| Risco jurídico | Médio | Smart contract e termos no protótipo | Danilo |
| Concorrência consolidada | Alto | Diferenciação IA + escrow documentada | Todos |
| Atraso no cronograma acadêmico | Alto | Sprints alinhadas a marcos; priorização MoSCoW | Danilo |
| Escopo inflado | Alto | Won't explícito para backend; foco em protótipo | Danilo |

---

## KPIs e métricas de sucesso

Referência: Declaração §11 e PM Canvas.

| KPI | Descrição | Meta (semestre) | Sprint de medição |
|-----|-----------|-----------------|-------------------|
| KPI-01 | Artefatos entregues no prazo | 100% dos marcos acadêmicos | Sprints 1–9 |
| KPI-02 | Cobertura de requisitos no protótipo | ≥ 90% dos RF-01–RF-13 representados | Sprint 9 (US-049) |
| KPI-03 | Protótipos navegáveis | WEB + MOBILE completos | Sprint 8 |
| KPI-04 | Correções críticas resolvidas | ≥ 80% dos problemas de Correções | Sprint 8–9 |
| KPI-05 | Avaliações concluídas | Avaliações 1–5 + feedback 16/06 | Sprint 9 |
| KPI-06 | Satisfação do professor/avaliador | Aprovação da solução | Sprint 9 |

---

## Resumo do backlog

| Métrica | Valor |
|---------|-------|
| Total de épicos | 10 (E01–E10) |
| Total de user stories | 54 (US-001–US-054) |
| Story points totais | ~218 SP |
| Must | 48 stories |
| Should | 4 stories (US-012, US-046, US-047 + parcial US-042) |
| Could | 0 no semestre (BF pós-semestre) |
| Won't (semestre) | 10 itens (BF-01–BF-10) |

---