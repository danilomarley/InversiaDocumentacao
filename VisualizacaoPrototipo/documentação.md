# ResolvAI — Documentacao do Prototipo

## O que e o ResolvAI?

ResolvAI e uma plataforma digital que conecta pessoas que precisam de servicos (contratantes) a prestadores de servico qualificados de maneira rapida, transparente e segura. O diferencial central e o uso de Inteligencia Artificial para estruturar escopos de servico detalhados, padronizar propostas e proteger ambas as partes por meio de smart contracts e pagamento com retencao (escrow).

**Foco atual:** manutencao residencial — infiltracao, alvenaria, hidraulica, impermeabilizacao, pintura.

---

## Modelo de Negocio

| Fonte de Receita | Descricao | Quem paga |
|---|---|---|
| Taxa de sucesso | 8-12% sobre o valor do servico, cobrado na liberacao do escrow | Prestador |
| Plano Pro | Assinatura mensal com selo verificado, destaque e relatorios | Prestador |
| Juros de parcelamento | Margem dos juros quando o contratante parcela | Contratante |

**Seguranca:** Smart contracts em blockchain + pagamento em escrow. Garantia obrigatoria em toda proposta. Disputas mediadas em 30 dias, com escalada juridica automatica.

---

## Estrutura de Arquivos

```
index.html          → Pagina de entrada — escolha entre as 3 visoes
cliente.html        → Visao do Contratante (mobile, tema azul, 11 telas)
fornecedor.html     → Visao do Prestador (mobile, tema laranja, 9 telas)
admim.html          → Visao do Administrador (web desktop, tema roxo, 6 telas)
documentacao.md     → Este arquivo
```

**Total: 26 telas** — 11 mobile (cliente) + 9 mobile (prestador) + 6 web (administrador)

Para rodar: basta abrir `index.html` no navegador. Nao precisa de servidor.

---

## Paleta de Cores por Visao

| Visao | Cor Primaria | Hex | Plataforma |
|---|---|---|---|
| Contratante | Azul | `#2563EB` | Mobile (375x812px phone frame) |
| Prestador | Laranja | `#FF5C1A` | Mobile (375x812px phone frame) |
| Administrador | Roxo | `#7B5EA7` | Web Desktop (sidebar + conteudo) |

**Cores compartilhadas:**
- Fundo escuro (body): `#0F1C2E`
- Sucesso: `#10B981`
- Alerta: `#F59E0B`
- Erro: `#EF4444`
- Tipografia: Inter (Google Fonts)

---

## Visao 1 — Contratante (`cliente.html`)

**Plataforma:** Mobile — phone frame centralizado (375x812px, border-radius 44px)
**Tema:** Azul (`#2563EB`)
**Bottom Nav:** Home, Chat IA, Pedidos, Alertas, Perfil

### Telas (11)

| # | Tela | Fase da Jornada |
|---|---|---|
| C1 | Splash / Onboarding | Descoberta — 3 slides com proposta de valor |
| C2 | Home / Discovery | Descoberta — saudacao + CTA "Criar pedido com IA" + pedidos ativos |
| C3 | Chat com IA | Criacao do Escopo — chat conversacional com chips, upload de fotos, barra de progresso |
| C4 | Escopo Gerado | Revisao — resumo estruturado, galeria de fotos, editar/publicar |
| C5 | Feed de Propostas | Recebimento — cards com preco/prazo/garantia, filtros, comparar |
| C6 | Detalhe da Proposta | Comparacao — perfil completo, portfolio, avaliacoes, aceitar |
| C7 | Comparar Propostas | Comparacao — 2-3 colunas lado a lado, scroll horizontal |
| C8 | Chat com Prestador | Alinhamento — chat interno, checklist, "Prosseguir para contrato" |
| C9 | Smart Contract | Assinatura — resumo, clausulas simples, assinatura digital |
| C10 | Checkout / Pagamento | Pagamento — PIX/Cartao/Boleto, parcelamento, aviso escrow |
| C11 | Confirmacao + Avaliacao | Avaliacao — confirmar conclusao, estrelas, comentario, disputa |

### Fluxo de Navegacao

```
C1 → C2 (apos onboarding)
C2 → C3 (CTA "Criar novo pedido com IA")
C3 → C4 (100% progresso → "Ver escopo gerado")
C4 → C5 ("Publicar pedido")
C5 → C6 (tap no card) | C5 → C7 (selecionar 2-3 + "Comparar")
C6 → C8 ("Enviar mensagem") | C6 → C9 ("Escolher esta proposta")
C7 → C9 ("Escolher" em qualquer coluna)
C8 → C9 ("Prosseguir para contrato")
C9 → C10 (ambos assinaram → checkout)
C10 → C2 (pagamento confirmado → home com pedido "Em andamento")
C11 → C2 (apos avaliacao)
```

---

## Visao 2 — Prestador (`fornecedor.html`)

**Plataforma:** Mobile — phone frame centralizado (375x812px, border-radius 44px)
**Tema:** Laranja (`#FF5C1A`)
**Bottom Nav:** Home, Pedidos, Propostas, Chat, Perfil

### Telas (9)

| # | Tela | Fase da Jornada |
|---|---|---|
| P1 | Onboarding / Cadastro | Cadastro — 3 passos: dados, categorias+regioes, documentos |
| P2 | Feed de Pedidos | Descoberta — KPIs, filtros, cards com compatibilidade IA |
| P3 | Detalhe do Pedido | Analise — escopo completo, galeria, info do cliente |
| P4 | Enviar Proposta | Envio — preco/prazo/descricao/garantia obrigatoria, dica IA |
| P5 | Minhas Propostas | Acompanhamento — metricas, status: Enviada/Visualizada/Escolhida |
| P6 | Chat com Cliente | Alinhamento — chat interno, checklist, contrato |
| P7 | Smart Contract | Assinatura — obrigacoes em destaque, garantia, assinatura |
| P8 | Servico em Andamento | Execucao — timeline de marcos, upload de progresso |
| P9 | Recebimento + Avaliacao | Confirmacao — resumo financeiro (bruto/taxa/liquido), avaliar cliente |

### Fluxo de Navegacao

```
P1 → P2 (apos cadastro)
P2 → P3 (tap no card)
P3 → P4 ("Enviar proposta")
P4 → P5 (proposta enviada)
P5 → P6 (status "Escolhida" → chat)
P6 → P7 ("Prosseguir para contrato")
P7 → P8 (apos assinatura + pagamento confirmado)
P8 → P9 (cliente confirma conclusao)
P9 → P2 ("Ver novos pedidos")
```

---

## Visao 3 — Administrador (`admim.html`)

**Plataforma:** Web Desktop — sidebar (260px) + area de conteudo fluida
**Tema:** Roxo (`#7B5EA7`)
**Sidebar:** Dashboard, Prestadores, Contratos, Disputas, Juridico, Analise de Rede

### Telas (6)

| # | Tela | Fase da Jornada |
|---|---|---|
| A1 | Dashboard | Monitoramento — 5 KPIs, funil de conversao, grafico semanal, alertas, mapa de calor |
| A2 | Gestao de Prestadores | Curadoria — tabela com status, pre-validacao IA, acoes aprovar/rejeitar/solicitar |
| A3 | Monitoramento de Contratos | Contratos — tabela com risco (verde/amarelo/vermelho), escrow total, alertas de vencimento |
| A4 | Central de Disputas | Disputas — tickets com prazo 30 dias, painel 3 colunas (escopo/chat/contrato), decisoes |
| A5 | Gestao Juridica | Escalada — casos com documentacao, exportar PDF, timeline, status juridico |
| A6 | Analise de Rede | Crescimento — mapa de calor, gaps de oferta, retencao, desintermediacao, recrutamento |

### Fluxo de Admin

```
Dashboard → (qualquer secao via sidebar) — navegacao livre
Alertas no Dashboard → linkam para Contratos, Disputas e Prestadores
Disputas → "Escalar para Juridico" → Gestao Juridica
Analise de Rede → "Recrutar" → campanha direcionada
```

---

## Regras de Negocio Implementadas no Prototipo

1. **IA Conversacional:** O contratante nao preenche formulario — a IA guia a criacao do escopo via chat
2. **Propostas Padronizadas:** Toda proposta inclui preco, prazo, descricao e garantia obrigatoria
3. **Comparacao Lado a Lado:** Ate 3 propostas podem ser comparadas simultaneamente
4. **Smart Contract:** Gerado automaticamente com escopo, termos e assinatura digital de ambas as partes
5. **Escrow:** Pagamento retido ate confirmacao de conclusao pelo contratante
6. **Parcelamento:** Contratante pode parcelar; prestador recebe valor integral de uma vez
7. **Garantia Obrigatoria:** Cada proposta define prazo e condicoes de garantia incorporados ao contrato
8. **Disputas 30 dias:** Tickets abertos automaticamente quando prazo expira, com mediacao baseada em evidencias
9. **Escalada Juridica:** Casos nao resolvidos em 30 dias sao escalados com documentacao completa
10. **Selo Verificado:** Prestadores aprovados pela curadoria recebem selo de confianca

---

## Contexto de Desenvolvimento

- **Stack sugerida para producao:** Python (FastAPI) + PostgreSQL + React Native
- **Prioridade atual:** Validar o modelo com prototipo academico antes de desenvolver backend
- **Prototipo:** HTML/CSS/JS puro — sem frameworks, sem servidor, sem dependencias
