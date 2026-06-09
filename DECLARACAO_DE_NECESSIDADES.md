# Declaração de Necessidades — Solução Inversia Marketplace de Oportunidades

## 1) Objetivo da declaração
Consolidar, a partir dos artefatos do repositório, as necessidades de negócio, de usuários e de produto para orientar decisões de escopo, implementação do MVP e evolução da plataforma.

## 2) Contexto da solução
A solução proposta é um **marketplace digital de serviços** para conectar clientes (demandantes) e prestadores (fornecedores), reduzindo atritos de descoberta, contratação e acompanhamento de serviços.

### Meta estratégica consolidada
Entregar um MVP funcional capaz de viabilizar:
- cadastro e autenticação de usuários;
- publicação e descoberta de demandas de serviço;
- envio e comparação de propostas;
- contratação e comunicação entre as partes;
- mecanismos de confiança (avaliações e histórico);
- operação inicial com tração mínima de mercado.

## 3) Problemas que a solução precisa resolver
1. Dificuldade de clientes em encontrar prestadores confiáveis.
2. Baixa visibilidade de prestadores autônomos para novas oportunidades.
3. Processo de contratação despadronizado e disperso (canais informais).
4. Baixa segurança percebida nas transações e na escolha de profissionais.
5. Falta de histórico e reputação estruturados para tomada de decisão.

## 4) Stakeholders e necessidades principais
## 4.1 Clientes (demandantes)
Precisam de:
- registrar demandas com clareza (texto e fotos);
- receber propostas aderentes ao problema e à região;
- comparar propostas em um único painel;
- contratar com segurança e continuar conversa no mesmo fluxo;
- avaliar prestadores e consultar histórico de serviços.

## 4.2 Prestadores (fornecedores)
Precisam de:
- visualizar pedidos de serviço em aberto com filtros úteis;
- enviar proposta com valor, prazo e abordagem técnica;
- construir reputação (perfil, portfólio e avaliações);
- receber notificações rápidas de oportunidades relevantes;
- controlar raio de atendimento para reduzir deslocamentos inviáveis.

## 4.3 Equipe interna e operação
Precisam de:
- painel administrativo para acompanhar uso, qualidade e incidentes;
- suporte a onboarding e moderação;
- dados para decisões de produto, growth e retenção.

## 4.4 Parceiros e terceiros
Precisam de:
- integração estável com pagamentos e serviços de geolocalização;
- conformidade com termos legais e responsabilidades bem definidas.

## 5) Necessidades funcionais (MVP)
1. **Cadastro, login e recuperação de senha** para perfis distintos.
2. **Publicação de pedido de serviço** (descrição detalhada e mídia).
3. **Descoberta de serviços/pedidos por geolocalização**, categoria e filtros.
4. **Envio e gestão de propostas** (valor, prazo, descrição).
5. **Comparação de propostas** em painel centralizado pelo cliente.
6. **Aceite de proposta e início de atendimento**.
7. **Canal de chat** entre cliente e prestador após aceite.
8. **Avaliação pós-serviço** (nota e comentário).
9. **Perfil do prestador** com portfólio e raio de atendimento.
10. **Notificações de novas oportunidades** para prestadores.
11. **Edição/cancelamento de pedidos** ainda em aberto.
12. **Histórico de serviços** para clientes e prestadores.
13. **Painel administrativo** para gestão operacional básica.

## 6) Necessidades não funcionais
## 6.1 Confiabilidade e desempenho
- Disponibilidade operacional elevada para fase inicial.
- Tempo de resposta adequado para não comprometer conversão.
- Observabilidade mínima (erros, latência, disponibilidade).

## 6.2 Segurança e confiança
- Proteção de dados de autenticação.
- Controles contra fraude e abuso de plataforma.
- Rastreabilidade de ações críticas.
- Termos de uso e políticas claras sobre responsabilidade da intermediação.

## 6.3 Usabilidade e acessibilidade
- Interface intuitiva e responsiva (web/mobile).
- Fluxos simples para primeiro uso (onboarding de cliente e prestador).

## 6.4 Escalabilidade e evolução
- Arquitetura que permita crescimento progressivo sem reescrita estrutural.
- Estrutura de dados preparada para evolução de matching inteligente.

## 7) Necessidades de negócio e operação
1. Validar rapidamente o modelo de marketplace com métricas de tração.
2. Garantir massa crítica mínima de oferta e demanda (evitar cold start).
3. Definir estratégia de monetização de forma aderente ao comportamento dos prestadores.
4. Estabelecer rotinas de aquisição, ativação e retenção.
5. Criar processos de suporte, moderação e resolução de conflitos.

## 8) Premissas relevantes
- Usuários possuem acesso à internet e smartphone.
- Prestadores terão interesse em adesão inicial.
- APIs externas (pagamento/mapas) estarão disponíveis e estáveis.
- Equipe central estará disponível ao longo do ciclo do MVP.

## 9) Restrições identificadas
- Orçamento limitado para construção e lançamento do MVP.
- Janela de execução curta para entrada no mercado.
- Equipe enxuta, exigindo priorização rígida.
- Dependência de terceiros para partes críticas (pagamento e geolocalização).

## 10) Riscos críticos que geram necessidades adicionais
1. **Baixa adesão inicial de prestadores**  
   Necessidade: estratégia ativa de onboarding e incentivo inicial.
2. **Baixa adesão de clientes demandantes**  
   Necessidade: estratégia de lançamento orientada a geração de primeiras demandas.
3. **Matching com baixa precisão**  
   Necessidade: começar com filtros confiáveis e evoluir algoritmo por iteração.
4. **Fraude e má-fé de prestadores**  
   Necessidade: validação cadastral, moderação e políticas de resposta.
5. **Risco jurídico por falhas de execução do serviço**  
   Necessidade: estrutura contratual e termos de uso robustos.
6. **Pressão competitiva de players consolidados**  
   Necessidade: diferenciação clara e foco inicial de nicho/região.

## 11) Critérios de sucesso da solução (referência para acompanhamento)
- Crescimento consistente de cadastros de clientes e prestadores.
- Geração recorrente de pedidos e propostas com taxa de conversão saudável.
- Redução de tempo entre abertura de demanda e primeira proposta útil.
- Evolução da satisfação dos usuários (avaliações e recorrência).
- Estabilidade técnica mínima para suportar campanhas de aquisição.

## 12) Declaração consolidada de necessidades
A solução Inversia necessita de um MVP de marketplace que conecte clientes e prestadores de forma confiável, simples e escalável, cobrindo ponta a ponta da jornada (publicação da necessidade, proposta, contratação, comunicação e avaliação), com foco em:
- geração rápida de liquidez de mercado (oferta + demanda);
- mecanismos concretos de confiança e segurança;
- experiência operacional fluida para usuários e equipe interna;
- base tecnológica e de negócio apta para validação do modelo e evolução contínua.

---

## Fontes analisadas no repositório
- `PM Canvas.pdf`
- `User History - Inversia.xlsx`
- `Matriz de riscos.xlsx`
- `Jornada do usuário.pdf` (conteúdo predominantemente visual/imagem)
- `Mapa de.pdf` (conteúdo predominantemente visual/imagem)
- `Orbital_Stakeholder_Strategy.odp` (conteúdo predominantemente visual/imagem)
