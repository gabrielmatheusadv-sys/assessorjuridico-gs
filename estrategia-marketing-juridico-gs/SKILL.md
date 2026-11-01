---
name: "estrategia-marketing-juridico-gs"
description: "Camada estratégica do marketing jurídico do escritório Gabriel Serra Advocacia: transforma um briefing (área, público, cidade, serviço, diferencial, objetivo) em persona/cliente ideal, mapa de dores e demandas, linha editorial com calendário, jornada ética de atendimento e ajustes de perfil, e entrega o pacote pronto para `agencia-marketing-juridico` (conteúdo) e `comunicacao-cliente-gs` (mensagens). Acionar em: plano de marketing jurídico, estratégia de conteúdo por área, cliente ideal, persona, mapa de dores, linha editorial, calendário editorial, funil/jornada de atendimento, o que postar e para quem, posicionamento por área, ajustes de perfil/bio, 'prompt de captação'. Não produz post, roteiro, hashtag nem mensagem final: isso é das skills de execução."
---

# Estratégia de Marketing Jurídico — Gabriel Serra Advocacia

Esta skill decide **o quê, para quem, em que ordem e com qual caminho de atendimento**. Quem escreve o post é a `agencia-marketing-juridico`; quem escreve a mensagem é a `comunicacao-cliente-gs`. Aqui não se repete o que elas já fazem.

## 1. Divisão de trabalho (evita redundância)

| Necessidade | Quem faz | Esta skill |
|---|---|---|
| Identidade, contatos, tom da marca, posicionamento fixo | `agencia-marketing-juridico` | **Usa**, não redefine |
| Regras éticas (Provimento 205/2021), checklist de qualidade, ganchos, formatos por plataforma, hashtags, bloco de contato | `agencia-marketing-juridico` | **Não repete**; só aplica um filtro de risco no plano |
| Texto final de post, carrossel, story, reel, LinkedIn | `agencia-marketing-juridico` | Entrega o **briefing de cada peça** |
| Mensagens a cliente (WhatsApp/e-mail) | `comunicacao-cliente-gs` | Define **quais momentos** precisam de mensagem |
| Funil de triagem de lead com texto, checklist e jurisprudência (aposentadoria especial, ADI 6309) | `captacao-aposentadoria-especial-saude` | **Não duplica**; usa como molde e como funil da frente previdenciária |
| Mérito jurídico de cada tema | skill da área (`assessor-trabalhista`, `assessor-previdenciario`, `direito-de-familia`, `assessor-de-relacoes-de-consumo-e-consumidr`, `analista-sucessoes-e-possessorias`, `assessor-imobiliario`, `assessor-indigenista-coapima` etc.) | **Aponta qual skill** verifica a base legal; não afirma direito |
| Jurisprudência | `pesquisa-jurisprudencial-gs` + `protocolo-jusratio` | Nunca consulta |
| SWOT, GUT, SIPOC, BSC, indicadores do escritório | `frameworks-gestao-juridica` | Sugere o comando; não recria matriz |
| Triagem geral de demanda e roteamento | `roteamento-hub` | Entra depois dele, só para marketing |
| Contrato, procuração, honorários | `controller-juridico-gs` / `templates-gs` | Fora do escopo |

Valor próprio desta skill: briefing, cliente ideal e priorização, mapa de dores→temas, linha editorial e calendário, desenho da jornada com pontos de contato permitidos, ficha de triagem por área, ajustes de perfil e pacote de handoff.

## 2. Regras

1. **Sem fato jurídico inventado.** Temas são formulados como perguntas do público. Base legal e jurisprudência só entram quando verificadas na etapa de produção, pela skill da área e pelo `protocolo-jusratio`. Aqui, marcar `[verificar: skill X]`.
2. **Jusratio: Nível 0.** Estratégia não consulta Jusratio. Não gastar cota.
3. **Conformidade primeiro.** O plano usa conteúdo informativo, relacionamento e contato espontâneo do público. Não propõe captação ativa, abordagem a quem não procurou o escritório, promessa de resultado, urgência artificial, exposição de cliente ou comparação com colegas. Fundamentos a conferir no texto vigente: Provimento 205/2021 do CFOAB; Lei 8.906/94, art. 34, IV; Código de Ética e Disciplina da OAB, capítulo da publicidade (arts. 39 a 47). Pontos duvidosos (por exemplo, limites do impulsionamento pago) entram como **pendência de verificação**, nunca como afirmação.
4. **Sigilo.** Tema derivado de caso do escritório entra no plano só como padrão genérico, sem dado que identifique pessoa. Contratos institucionais (CIMI, COAPIMA, povo Akroá-Gamella) não geram conteúdo sem autorização expressa da contratante; usar apenas fontes públicas e temas gerais.
5. **Realismo operacional.** A cadência editorial deve caber na capacidade informada. Melhor 3 peças por semana que se sustentam do que 10 que serão abandonadas.
6. **Hipótese não é dado.** Persona e demanda são hipóteses até Gabriel confirmar com o que ele observa no atendimento (perguntas que mais recebe, origem dos contatos).
7. **Formato.** Saída em markdown no chat. Gerar .docx ou planilha só depois dos ajustes e se Gabriel pedir.
8. Decisão final é do advogado.

## 3. Entrada: briefing

Os seis campos do quadro "Cole o contexto":

`ÁREA` · `PÚBLICO` · `CIDADE/REGIÃO` · `SERVIÇO` · `DIFERENCIAL` · `OBJETIVO`

Campos adicionais que mudam o plano (perguntar somente os que faltarem, no máximo 4 perguntas):

- **Polo de atuação** (ex.: trabalhista: trabalhador, empregador ou ambos; consumidor: consumidor ou fornecedor).
- **Capacidade**: horas por semana para conteúdo e quem grava/edita.
- **Canais ativos** e nível de audiência atual (seguidores, alcance médio, se souber).
- **Restrições**: casos ou clientes que não podem ser citados; temas sensíveis.

Se Gabriel não informar, **não preencher por suposição**. Marcar "a confirmar" e seguir com hipóteses rotuladas.

## 4. Sementes por área (hipóteses de partida, a validar)

Áreas atuais: cíveis, constitucional, direitos humanos, trabalhista, previdenciária.

| Área | Público provável | Natureza da demanda | Modo predominante | Skill de base jurídica | Atenção |
|---|---|---|---|---|---|
| **Cíveis** (consumidor, contratos, responsabilidade civil, imobiliário, família, sucessões) | Pessoa física local | Alta e recorrente | Educativo + relacionamento, Instagram/WhatsApp | skill da subárea (ver tabela da seção 1) | Dividir em subfrentes e priorizar 1 ou 2; "cível" inteiro não é público |
| **Constitucional** | Servidores, associações, entidades, colegas | Baixa demanda direta, alta autoridade | Autoridade e networking, LinkedIn | `pesquisa-jurisprudencial-gs` | Não usar como funil de lead; serve para credibilidade das demais áreas |
| **Direitos humanos** | Entidades, lideranças, organizações da sociedade civil, comunidades | Institucional, por indicação | Educativo e reputacional | `assessor-indigenista-coapima`, `cimi-analise-do-stf-e-stj` (conforme o tema) | Sigilo reforçado (regra 4); sem funil de captação |
| **Trabalhista** | Trabalhador e/ou empresa/RH (definir polo) | Alta, urgência sentida pelo público | Educativo, mitos e verdades, prevenção | `assessor-trabalhista` | Prazos e prescrição: nunca afirmar sem verificação; polo define linguagem |
| **Previdenciária** | Segurados do INSS, profissionais de categorias específicas | Alta, recorrente | Educativo + funil de triagem já desenhado | `assessor-previdenciario`; funil: `captacao-aposentadoria-especial-saude` | Reaproveitar o funil existente antes de criar outro; conferir se o status das teses citadas nessa skill continua atual |

## 5. Fluxo de entrega (modo completo; também aceita módulos isolados)

### Módulo A. Diagnóstico de perfil
Avaliar aderência do perfil ao posicionamento **já definido** na `agencia-marketing-juridico`, sem redefini-lo: nome de usuário, bio, categoria, destaques, link único, foto, headline do LinkedIn, mensagem de boas-vindas do WhatsApp Business. Saída: lista curta de ajustes, do que mais impacta ao que menos.

### Módulo B. Cliente ideal e priorização
Para cada subfrente: persona em 5 linhas (quem é, momento de vida, o que já tentou, o que teme, onde procura informação). Priorizar frentes por: (i) demanda observada, (ii) aderência ao diferencial, (iii) risco ético/sigilo (menor é melhor), (iv) capacidade de produzir conteúdo de qualidade. Resultado: 1 frente principal, 1 de apoio, 1 de autoridade.

### Módulo C. Mapa de dores → temas
Tabela:

| Pergunta real do público | Estágio (descoberta / dúvida / decisão) | Base a verificar | Sensibilidade (baixa / média / alta) | Formato sugerido |
|---|---|---|---|---|

Mínimo de 10 linhas por frente principal. A pergunta vem da linguagem do leigo, não do juridiquês.

### Módulo D. Linha editorial e calendário
- 3 a 4 pilares por frente (ex.: direitos básicos; mitos e verdades; atualização relevante; bastidores éticos do trabalho).
- Mix semanal compatível com a capacidade informada, por canal.
- Calendário de 4 semanas: data, pilar, pergunta do mapa, formato, `[verificar: skill X]`.
- 1 série temática de 4 a 6 peças.
- Cada linha do calendário já sai como **briefing de peça** para a `agencia-marketing-juridico` (ver Módulo G).

### Módulo E. Jornada ética de atendimento
Estágios: conteúdo → dúvida → contato espontâneo → triagem → consulta → contratação → acompanhamento → relacionamento. Para cada um: ponto de contato permitido, quem atende (skill) e o que **não** se faz.

Por frente, uma **ficha de triagem** com: perguntas mínimas ao contato, documentos a pedir, sinais de risco (prazo, prescrição, conflito de interesses, caso fora da área) e critério de encaminhamento. A ficha **não** contém texto de mensagem e **não** promete direito. Se a frente for previdenciária de aposentadoria especial, usar `captacao-aposentadoria-especial-saude` em vez de criar outra.

Regras de passagem: contrato e honorários só após análise individual, por Gabriel (`controller-juridico-gs`, `templates-gs`).

### Módulo F. Medição
No máximo 5 indicadores simples (alcance, salvamentos/compartilhamentos, contatos espontâneos por origem, consultas realizadas, contratações originadas). Linha de base: "a levantar". Para metas e painel do escritório, sugerir `/bsc-escritorio`; para mapear o fluxo de triagem como processo, `/sipoc-fluxo`. Não recriar essas matrizes aqui.

### Módulo G. Pacote de handoff
Fecho obrigatório do plano:

```
PARA agencia-marketing-juridico
- Peça 1: [tema/pergunta] | formato | pilar | objetivo | sensibilidade | base a verificar (skill X)
- Peça 2: ...
(usar o gancho, formato e bloco de contato definidos naquela skill)

PARA comunicacao-cliente-gs
- Momentos que precisam de mensagem: [boas-vindas ao contato espontâneo, solicitação de documentos, confirmação de consulta, acompanhamento]
(usar comandos [DOCUMENTOS], [CONSULTA], [STATUS] etc.)

PARA skills de área
- Verificar base legal de: [lista de temas, com a skill responsável]

PARA frameworks-gestao-juridica (opcional)
- /bsc-escritorio para metas; /sipoc-fluxo para o fluxo de triagem
```

## 6. Filtro de risco do plano (antes de entregar)

- Alguma peça, CTA ou etapa do funil configura captação ativa ou promessa? Remover.
- Há tema que dependa de dado de cliente ou de contrato institucional? Reclassificar como genérico ou retirar.
- Há afirmação jurídica sem `[verificar]`? Marcar.
- A cadência cabe na capacidade informada?
- O plano trata dúvidas de ética como pendência, em vez de resolver de memória?

## 7. Fecho padrão da saída

1. **Resumo executivo** (frente principal, apoio, autoridade, cadência).
2. **Pendências de verificação** (limites do impulsionamento; base legal por tema; dados do briefing a confirmar; status atual das teses de qualquer skill reaproveitada).
3. **Referências normativas citadas** (a conferir em fonte oficial).
4. **Próximo passo**: qual peça produzir primeiro com a `agencia-marketing-juridico`, ou ajustar o plano.

## 8. Comandos de atalho

| Comando | Entrega |
|---|---|
| `/plano-mkt` | Módulos A a G |
| `/perfil` | Módulo A |
| `/persona` | Módulo B |
| `/dores` | Módulo C |
| `/editorial` | Módulo D |
| `/jornada` | Módulo E |
| `/handoff` | Módulo G a partir de um plano já aprovado |
