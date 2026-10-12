# Visão da Demanda (VD) — Sistema de Gestão das Feiras Livres de Fortaleza

> **Exemplo didático preenchido conforme o template LAPIS v2.1.** Base documental: [Solicitação da Prefeitura](PropostaFeiraLivre.md) e [VD anterior](exemplo-feira-livre-visao.md). Valores, frequência e demais avaliações herdadas da VD anterior são classificações do exemplo, **não aprovações da Prefeitura**. Fluxos e testes são detalhados em artefatos próprios.

## Identificação e Histórico

| Campo | Informação |
| --- | --- |
| Nome e identificador da demanda | Sistema de Gestão das Feiras Livres de Fortaleza — código a definir |
| Tipo | Novo sistema |
| Sistema ou produto relacionado | Novo Sistema de Gestão das Feiras Livres de Fortaleza |
| Área solicitante | Prefeitura de Fortaleza — Secretaria Municipal responsável pelas feiras (denominação formal a definir) |
| Responsável pela elaboração | Equipe LAPIS (conforme VD original) |
| Responsável pela validação | A definir pela Prefeitura |
| Situação do documento | Em revisão — exemplo didático sem aprovação formal |
| Versão e data | 1.1 — 12/10/2026 (adaptada ao template LAPIS v2.1) |

| Data | Versão | Descrição da alteração | Autor |
| --- | --- | --- | --- |
| 12/04/2026 | 1.0 | Criação inicial, conforme VD anterior | Equipe LAPIS |
| 12/10/2026 | 1.1 | Reorganização no template LAPIS v2.1; rastreabilidade com solicitação original; lacunas explicitadas | Adaptação assistida por IA — requer revisão da equipe LAPIS |

## 1. Objetivo

Apoiar a Secretaria Municipal responsável na **gestão das feiras livres de Fortaleza**, mediante registro e acompanhamento de feiras, feirantes, barracas e taxas, oferecendo aos fiscais consulta aos feirantes autorizados e melhorando a organização e o controle administrativo.

## 2. Contexto, Problema e Descrição Sumária da Demanda

- **Situação atual:** o controle de feirantes, a organização das barracas, as autorizações e o pagamento de taxas são feitos manualmente ou por planilhas, conforme a solicitação da Prefeitura.
- **Problema ou oportunidade:** essas práticas dificultam o controle administrativo e a fiscalização e motivam a modernização da gestão das feiras.
- **Públicos afetados e impactos:** Secretaria Municipal (gestão), fiscais (consulta e fiscalização) e feirantes (cadastros, licenças e situação relacionada às taxas).
- **Evidências disponíveis:** [PropostaFeiraLivre.md](PropostaFeiraLivre.md), contexto e itens 1 a 18; [VD original](exemplo-feira-livre-visao.md), catálogo e representações. Não foram fornecidas métricas da situação atual.
- **Descrição sumária da demanda:** solução acessível em navegadores web modernos para manter cadastros de feirantes, registrar feiras e barracas, registrar pagamentos de taxas, emitir relatórios mensais de arrecadação, permitir a consulta fiscal e controlar o acesso administrativo e o histórico de alterações.

## 3. Proposta de Valor e Sucesso da Demanda

| Benefício esperado | Indicador ou evidência | Resultado desejado | Como e quando avaliar |
| --- | --- | --- | --- |
| Melhorar o controle dos feirantes e barracas | Disponibilidade e consistência dos registros por feira | Cadastro e vinculação de barracas utilizáveis pela Secretaria | Conferência com representantes da Secretaria na homologação; metas quantitativas a definir |
| Facilitar a fiscalização | Consulta aos feirantes autorizados por feira | Fiscais conseguem consultar os registros necessários | Validação funcional com fiscais; critérios detalhados no respectivo CDU |
| Apoiar a gestão de taxas | Registro de pagamentos e relatórios mensais de arrecadação | Secretaria obtém relatórios mensais por feira | Verificação com dados de teste e avaliação pelo setor responsável |
| Melhorar a rastreabilidade administrativa | Histórico de alterações dos cadastros | Alterações nos cadastros de feirantes podem ser consultadas/auditadas conforme regras a definir | Revisão das evidências de histórico durante homologação |

> As metas numéricas de benefício e a linha de base **não constam dos documentos de origem**; precisam ser levantadas. O limite de três segundos é condição de qualidade, não meta de benefício.

## 4. Partes Interessadas

| Parte interessada | Papel e interesse | Responsabilidade | Representante |
| --- | --- | --- | --- |
| Prefeitura de Fortaleza / Secretaria Municipal | Solicitante e gestora das feiras | Definir e validar necessidades e regras operacionais; gerenciar feiras e cadastros | Ana Lima (identificada na VD anterior; representação a confirmar) |
| Feirantes | Público afetado / possível usuário | Manter-se regularizados e cumprir obrigações relacionadas às taxas | A definir |
| Fiscal Municipal | Usuário de fiscalização | Consultar a regularidade de feirantes por feira | José Silva (identificado na VD anterior; representação a confirmar) |
| Equipe de desenvolvimento | Construção e manutenção | Especificar, implementar e testar a solução contratada | Equipe LAPIS (VD anterior; atribuição real a confirmar) |

## 5. Usuários e Atores Externos

| ID | Usuário, sistema ou dispositivo | Objetivo ou papel na interação | Contexto de uso relevante |
| --- | --- | --- | --- |
| AT-01 | Administrador/servidor da Secretaria Municipal | Manter cadastros, feiras, barracas, pagamentos e relatórios | Acesso às funções administrativas autenticadas |
| AT-02 | Fiscal Municipal | Consultar feirantes autorizados numa feira | Consulta de apoio à fiscalização |
| AT-03 | Feirante | Público interessado em licenças e taxas; interação direta com a solução **a confirmar** | Solicitação menciona feirantes como titulares de registros; VD anterior também sugere operações próprias ainda não confirmadas |
| AT-04 | Sistema da Prefeitura para validação de licenças | Possível integração citada na VD anterior | **Hipótese não confirmada** na solicitação da Prefeitura |

> Personas do Feirante e do Fiscal aparecem na VD anterior. Seu detalhamento é opcional e não precisa ser duplicado neste documento.

## 6. Escopo e Entregas Previstas

### 6.1. Incluído na demanda

- Cadastro, alteração e remoção de feirantes.
- Registro das feiras por bairro e associação de até uma barraca por feirante em cada feira.
- Registro de pagamento de taxas municipais e relatórios mensais de arrecadação.
- Consulta, pelos fiscais, dos feirantes autorizados para uma feira.
- Autenticação para funcionalidades administrativas e histórico de alterações nos cadastros dos feirantes.
- Atendimento às condições de uso via navegador, desempenho, base de dados e conformidade descritas na seção 9.

### 6.2. Fora do escopo

- **Não há exclusões formalmente informadas nas fontes.** Não presumir exclusão de qualquer capacidade sem acordo com a Secretaria. O escopo de emissão de licenças, pagamentos eletrônicos e funções de autosserviço dos feirantes precisa ser decidido (seção 10).

### 6.3. Evoluções futuras — opcionais

- **Sem evolução futura aprovada.** A VD anterior apresenta solicitar licença, pagar taxa e consultar próxima feira pelo feirante, além de configurar feira e emitir licença pela Secretaria. São **candidatas à avaliação**, não entregas comprometidas nem evoluções confirmadas.

### 6.4. Entregas e marcos — quando conhecidos

| Entrega ou marco | Resultado previsto | Data ou condição | Natureza do prazo |
| --- | --- | --- | --- |
| Desenvolvimento do sistema | Sistema com as capacidades acordadas | Até 6 meses após contratação | Prazo máximo **estimado** na solicitação; detalhamento a confirmar |
| Homologação e aceite | Verificação com responsáveis da Prefeitura | A definir | Marco proposto para planejamento; sem data definida |

## 7. Necessidades e Catálogo de Funcionalidades

**Fontes:** `PF-01` = [PropostaFeiraLivre.md](PropostaFeiraLivre.md), itens numerados; `VD-1.0` = [exemplo anterior](exemplo-feira-livre-visao.md). IDs `NEC-` e `F-` são novos identificadores estáveis do exemplo 2.1; a coluna de especificação registra o **CDU a elaborar**, sem afirmar que o arquivo exista.

| ID | Necessidade | Fonte ou evidência | Públicos ou atores relacionados |
| --- | --- | --- | --- |
| NEC-01 | Manter registros atualizados dos feirantes | PF-01 itens 1 e 6 | AT-01, AT-03 |
| NEC-02 | Organizar feiras e barracas por localidade | PF-01 itens 2, 15 e 17; VD-1.0 | AT-01, AT-03 |
| NEC-03 | Controlar pagamentos e arrecadação de taxas | PF-01 itens 4, 5 e 16 | AT-01, AT-03 |
| NEC-04 | Apoiar a fiscalização de participantes autorizados | PF-01 itens 3 e 14 | AT-02, AT-01 |
| NEC-05 | Controlar o acesso administrativo e rastrear alterações cadastrais | PF-01 itens 9 e 10 | AT-01, AT-02 |

| ID | Funcionalidade e resultado esperado | Necessidade | Atores (IDs) | Prioridade | Valor | Frequência | Escopo ou entrega | Especificação |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| F-01 | Cadastrar feirante com nome, CPF, produto e telefone | NEC-01 | AT-01 | A definir | Alto | Alta | Incluída | CDU-01 — a elaborar |
| F-02 | Atualizar ou remover cadastro de feirante | NEC-01 | AT-01 | A definir | Médio | Média | Incluída | CDU-02 — a elaborar |
| F-03 | Registrar feira por bairro | NEC-02 | AT-01 | A definir | Alto | Média | Incluída | CDU-03 — a elaborar |
| F-04 | Associar barraca a feirante por feira | NEC-02 | AT-01 | A definir | Alto | Alta | Incluída | CDU-04 — a elaborar |
| F-05 | Registrar pagamento de taxa municipal | NEC-03 | AT-01 | A definir | Alto | Alta | Incluída | CDU-05 — a elaborar |
| F-06 | Gerar relatórios mensais de arrecadação por feira | NEC-03 | AT-01 | A definir | Alto | Baixa (mensal) | Incluída | CDU-06 — a elaborar |
| F-07 | Consultar feirantes autorizados em uma feira | NEC-04 | AT-02 | A definir | Alto | Alta | Incluída | CDU-07 — a elaborar |
| F-08 | Autenticar usuários da Prefeitura para acessar funções administrativas | NEC-05 | AT-01, AT-02 | A definir | Alto | Alta (por acesso, a confirmar) | Incluída | CDU-08 — a elaborar |
| F-09 | Registrar histórico de alterações dos cadastros de feirantes | NEC-05 | AT-01 | A definir | Médio | Alta (por alteração, a confirmar) | Incluída | CDU-09 — a elaborar |

> **Valor e frequência:** estimativas do exemplo anterior (alta/média/mensal/sempre), adaptadas à escala qualitativa v2.1. A prioridade não estava explicitamente definida e permanece **A definir**. Para F-08/F-09, “sempre” no exemplo anterior expressava ocorrência condicionada ao evento, e não volume medido; a frequência precisa de validação. A participação direta do feirante em F-05 permanece não confirmada — a fonte obriga o **registro** do pagamento, não necessariamente sua realização no sistema.

> **Candidatas sem inclusão confirmada:** solicitação de licença, emissão de licença, pagamento direto pelo feirante, consulta da próxima feira e configuração de feira aparecem no diagrama da VD 1.0, mas não constam de forma inequívoca como funções exigidas nos itens 1–18 da solicitação. Não receberam identificadores `F-` até haver decisão de escopo.

## 8. Visão Geral da Solução e Impactos

- **Responsabilidades da solução:** apoiar gestão cadastral, organização das feiras, associação de barracas, controle de taxas, relatórios, consultas fiscais, autenticação administrativa e histórico de alterações.
- **Sistemas ou dispositivos externos:** sistema de validação de licenças da Prefeitura foi proposto na VD anterior, mas sua existência, interface e necessidade de integração não estão confirmadas.
- **Integrações principais:** **A definir**; não considerar a API representada nos diagramas anteriores como contrato aprovado.
- **Diagrama de contexto:** não obrigatório; a visão de atores e capacidades está coberta pelas seções 5 e 7. Pode ser elaborada se facilitar a validação do escopo.
- **Arquitetura e contratos detalhados:** documento técnico a elaborar. A VD anterior incluía diagramas de componentes e implantação com escolhas de API REST, balanceadores, servidores e bancos específicos; **essas decisões não são confirmadas pela solicitação** e não integram esta VD.

### 8.1. Sistemas e processos impactados

| Sistema ou processo | Impacto esperado | Responsável ou dependência | Situação |
| --- | --- | --- | --- |
| Cadastro de feirantes | Substituição/apoio ao controle manual ou por planilha | Secretaria Municipal | Processo atual descrito na solicitação |
| Organização de feiras e barracas | Registro de feiras e associação de barracas | Secretaria Municipal | Processo atual descrito na solicitação |
| Controle de taxas | Registro de pagamentos e relatórios mensais | Secretaria / arrecadação (área específica a definir) | Necessidade descrita; integração a confirmar |
| Fiscalização municipal | Consulta de feirantes autorizados por feira | Fiscais municipais | Necessidade descrita na solicitação |
| Sistema de validação de licenças da Prefeitura | Possível intercâmbio para validação | Prefeitura, área técnica a definir | **Hipótese da VD anterior** |

### 8.2. Representações visuais — opcionais

- **Mapa de histórias / diagrama geral de casos de uso:** o exemplo anterior contém mapa de histórias e diagrama de interações. Podem ser preservados como referências históricas, **mas incluem funções pendentes de confirmação**; revisar antes de reaproveitar.
- **Protótipo de baixa fidelidade:** não fornecido; opcional.
- **Diagramas de componentes e implantação:** presentes na VD anterior; mover para documentação técnica quando as escolhas de arquitetura forem analisadas, em vez de tomá-los como decisões aprovadas.

## 9. Condições Gerais da Demanda

| Tipo | Condição e impacto na demanda | Responsável ou fonte | Referência, se houver |
| --- | --- | --- | --- |
| Qualidade | Operar em navegadores web modernos | Prefeitura | PF-01 item 7; especificação detalhada a elaborar |
| Qualidade | Consultas devem responder em até **3 segundos** | Prefeitura | PF-01 item 8; condições de medição a definir |
| Restrição técnica | Utilizar banco de dados relacional | Prefeitura | PF-01 item 11 |
| Premissa | Prefeitura dispõe de servidores para hospedar a solução | Prefeitura | PF-01 item 13; disponibilidade/capacidade a confirmar |
| Regra geral | Participação na feira condicionada à licença válida emitida pela Prefeitura | Prefeitura | PF-01 item 14; detalhamento de validação a elaborar |
| Regra geral | No máximo uma barraca registrada por feirante **em cada feira** | Prefeitura | PF-01 item 15; regra detalhada a elaborar |
| Regra geral | Valores das taxas obedecem à legislação municipal vigente | Prefeitura | PF-01 item 16; normas e atualizações a identificar |
| Regra geral | Feiras ocorrem nos dias/horários definidos pela Secretaria | Prefeitura | PF-01 item 17; detalhamento a elaborar |
| Restrição legal | Atender à legislação municipal aplicável às feiras livres | Prefeitura | PF-01 item 18; atos específicos a identificar |
| Prazo | Desenvolvimento estimado em até seis meses após contratação | Prefeitura | PF-01 item 12; validação no planejamento |

## 10. Riscos e Questões em Aberto

| ID | Tipo | Risco ou questão | Impacto | Próxima ação | Responsável e prazo | Situação |
| --- | --- | --- | --- | --- | --- | --- |
| PQ-01 | Dúvida | Quem aprova a VD e representa formalmente a Secretaria? | Ausência de aceite formal | Identificar responsável autorizado | Prefeitura — a definir | Aberto |
| PQ-02 | Dúvida | O feirante acessará o sistema para solicitar licença, pagar taxa ou consultar feiras? | Mudança em atores, escopo e interfaces | Validar funcionalidades adicionais da VD 1.0 | Secretaria — a definir | Aberto |
| PQ-03 | Dúvida | A emissão de licenças e a integração para validá-las fazem parte da entrega? | Dependência de sistemas e regras externas | Confirmar processo de licenciamento e integração | Secretaria / TI — a definir | Aberto |
| PQ-04 | Dúvida | Qual a ordem de prioridade das nove funcionalidades? | Planejamento de entregas | Priorizar com envolvidos | Secretaria — a definir | Aberto |
| PQ-05 | Dúvida | Quais metas de negócio e valores de referência permitem avaliar os benefícios? | Dificuldade de medir sucesso | Levantar linha de base e metas | Secretaria — a definir | Aberto |
| PQ-06 | Dúvida | Qual legislação específica rege taxas, funcionamento e licenças? | Risco de aplicação incorreta de regras | Referenciar atos municipais vigentes | Secretaria / jurídico — a definir | Aberto |
| PQ-07 | Dúvida | Como medir o tempo máximo de 3 segundos (carga, consultas e ambiente)? | Aceite não reproduzível | Definir cenários de desempenho | TI / Secretaria — a definir | Aberto |
| PQ-08 | Premissa a confirmar | Servidores da Prefeitura são adequados ao sistema? | Risco de implantação | Avaliar ambiente disponível | TI da Prefeitura — a definir | Aberto |
| PQ-09 | Dúvida | Há necessidade de trilha de auditoria além de histórico de alterações cadastrais? | Aumento de escopo e requisitos de segurança | Definir abrangência do histórico | Secretaria — a definir | Aberto |

## 11. Documentos Relacionados

| Documento | Conteúdo sob sua responsabilidade | Referência e situação |
| --- | --- | --- |
| Solicitação original da Prefeitura | Problema e 18 condições da demanda | [PropostaFeiraLivre.md](PropostaFeiraLivre.md) — fonte fornecida |
| VD original do exemplo | Descrições, classificações e diagramas históricos | [exemplo-feira-livre-visao.md](exemplo-feira-livre-visao.md) — versão anterior |
| Glossário Feira Livre | Definições de feirante, barraca e outros termos | [glossario-feira-livre.md](glossario-feira-livre.md) — referido na VD antiga; conteúdo não conferido nesta revisão |
| Regras de negócio compartilhadas | Licença, limite de barracas, taxas e dias/horários | A elaborar; origem PF-01 itens 14–17 |
| Requisitos de qualidade | Navegadores, tempo de resposta e demais critérios verificáveis | A elaborar; origem PF-01 itens 7–8 |
| Especificações dos casos de uso | Fluxos, exceções, regras e critérios de aceitação de F-01 a F-09 | CDU-01 a CDU-09 — a elaborar/associar a existentes após levantamento |
| Arquitetura e contratos de integração | Validar a necessidade de integração e escolhas técnicas | A definir; diagramas históricos não configuram aprovação |

## 12. Validação da Visão

### 12.1. Checklist

- [x] Objetivo, contexto e problema estão descritos a partir da solicitação.
- [ ] Benefícios e condições de sucesso foram confirmados com medidas e responsáveis.
- [ ] Responsável pela validação formal foi identificado.
- [x] Perfis de usuários e sistemas externos relevantes foram identificados ou sinalizados como hipótese.
- [ ] Escopo e exclusões foram validados; existem funcionalidades da VD antiga pendentes de decisão.
- [x] Necessidades possuem IDs e referências às fontes.
- [ ] Funcionalidades têm IDs, atores e necessidades; **prioridades precisam ser definidas**.
- [x] Valor e frequência estão separados; avaliações herdadas foram identificadas como não validadas.
- [x] Especificações têm identificadores de referência e situação **a elaborar**.
- [x] Visão geral distingue responsabilidades e integração hipotética.
- [x] Diagramas técnicos foram retirados do corpo da VD e mantidos como referências históricas.
- [x] Premissas, restrições, regras gerais e dúvidas estão registradas.
- [x] Detalhes técnicos e comportamentais estão indicados em artefatos separados.
- [ ] Revisão e validação humanas foram realizadas.

### 12.2. Critérios de conclusão e encaminhamento

**Condição atual: com pendências a resolver antes da validação formal.** Esta versão contém catálogo inicial suficiente para discussão de especificação, mas **não foi aprovada pela Prefeitura**. A equipe pode refinar casos de uso relativos às funções expressamente pedidas, sem presumir escopo adicional; a decisão de considerá-la formalmente *apta para iniciar a especificação* cabe aos responsáveis.

### 12.3. Registro da validação

| Versão | Responsável e papel | Data | Condição da VD | Resultado e ressalvas |
| --- | --- | --- | --- | --- |
| 1.1 | A definir — representante da Prefeitura | A definir | Em revisão; não validada | Confirmar escopo adicional, prioridades, metas e responsáveis — PQ-01 a PQ-09 |
