# Case de Canais Digitais | WhatsApp Maxpar / Autoglass

**Análise de Negócios · Discovery · Mapeamento de Processos · Jornada do Usuário · MVP · Backlog · BDD**

Projeto de estudo e evolução de atendimento digital ligado a **seguros auto**, serviços ao segurado/beneficiário e direcionamento ao **e-commerce da Autoglass**, conforme o [quadro original do Miro](https://miro.com/app/board/uXjVNlaxnuE=/).

O case reúne investigação da jornada existente, desenho de opções de atendimento no WhatsApp da Maxpar, cenários de resposta, regras de negócio, estudo de futuras funcionalidades e provas de conceito (POCs).

> ### 🔎 Acesse o projeto original no Miro
>
[**Abrir quadro completo e navegável — Discovery, jornadas, MVP, histórias de usuário e POCs**](https://miro.com/app/board/uXjVNlaxnuE=/)

Endereço oficial do quadro identificado no Miro. Explore os fluxos, as conexões, as telas e os conteúdos detalhados no Miro.

A fonte visual oficial é o [quadro no Miro](https://miro.com/app/board/uXjVNlaxnuE=/).
> **Observação:** esta página é uma organização de case para portfólio.


> **Os fluxos, as tarefas, imagens e os dados originais não foram alterados.** A fonte visual e funcional continua sendo o [quadro do Miro](https://miro.com/app/board/uXjVNlaxnuE=/).


## Navegue pelo projeto

| Etapa | Conteúdo disponível |
| --- | --- |
| **1. Discovery** | [Análise dos canais e oportunidades de melhoria no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764581172626138) |
| **2. Canvas MVP** | [Quadro visual de análise e referências](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764581793445322) |
| **3. Jornada de atendimento** | [Fluxo completo no GitHub — 43 etapas e 36 ligações](./docs/FLUXO_MIRO_JORNADA_COMPLETA.md) · [Miro original](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764581758623044) |
| **4. Requisitos / BDD** | [10 cenários de usuário e regras originais](./docs/CENARIOS_E_REGRAS_ORIGINAIS.md) |
| **5. Estudo de backlog** | [Fluxo completo no GitHub — 34 etapas e 24 ligações](./docs/FLUXO_MIRO_BACKLOG_COMPLETO.md) · [Miro original](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764581755947826) |
| **6. POC 01** | [Frame no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764582022045353) · [Vídeo demonstrativo](https://youtu.be/u4LxF7WXEUY) |
| **7. POC 02** | [Frame no Miro com a sequência de telas](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764582024733080) |
| **Documentação completa** | [Contexto, jornada, backlog, comportamentos e evidências](./docs/CASE_MAXPAR_AUTOGLASS.md) |

## Objetivo de negócio

Analisar e estruturar uma jornada de atendimento via WhatsApp que **oriente o usuário ao canal adequado**, diferencie o atendimento para segurados e não segurados e reduza ambiguidades na navegação.

No quadro, o **WhatsApp da Maxpar Serviços** conduz o contato inicial e apresenta informações de assistência relacionadas ao seguro. O encaminhamento à **Autoglass** é documentado nos casos voltados a **compra de peças automotivas**, incluindo o direcionamento ao e-commerce.


## Canais digitais e jornada analisados

| Canal ou ponto de contato | Papel identificado no quadro | Oportunidade documentada |
| --- | --- | --- |
| **WhatsApp da Maxpar** | Primeiro contato com segurados ou não segurados, apresentação de menu e mensagens de orientação | Tornar as opções claras, tratar respostas inválidas e oferecer transbordo para atendimento humano |
| **Portal do Segurado (Maxpar)** | Consulta e abertura de atendimento, com orientação para selecionar o card **Segurado & Corretor** e a seguradora | Facilitar o direcionamento correto, evitando navegação confusa |
| **E-commerce Autoglass** | Canal indicado para quem busca compra de peças automotivas | Informar o destino adequado aos não segurados e na mensagem de encerramento |
| **Canais complementares** | Atendimento humano, assistência 24 horas e Linktree relacionados à jornada | Orientar sobre horários, meios de contato e alternativas para cada necessidade |

**AS IS — pontos observados no Discovery:** registros de interações sem resposta ou sem direcionamento, necessidade de informação de horário de atendimento e existência de diferentes pontos de contato. São observações do quadro, não medições de desempenho.

**Evolução estudada / TO BE:** jornada com menu orientado ao perfil, mensagens compreensíveis, tratamento de opções inválidas, direcionamento para atendimento humano e estudo de menu de serviços (**Assistência Dia e Noite, Seguradoras, Oficina e voltar**).

**POCs:** o quadro inclui protótipos e demonstração do fluxo. A existência de um MVP ou POC **não significa, por si só, implantação em produção**.

## Jornada documentada no Miro

```mermaid
flowchart LR
    A["Início: WhatsApp Maxpar"] --> B["Saudação + menu"]
    B --> C{"Perfil do usuário"}
    C -->|"Segurado"| D["Abertura/status e orientações"]
    D --> E["Vidros e acessórios / portal do segurado"]
    E --> F["Opção de atendente humano"]
    C -->|"Não segurado"| G["Direcionamento ao e-commerce Autoglass"]
    B -.-> H["Opção inválida: orientar"]
    H -.-> I["Nova tentativa inválida: encerrar"]
```

**Importante:** essa é uma **visão executiva simplificada**, não uma alteração do fluxograma original. Consulte o [fluxo completo no Miro](https://miro.com/app/board/uXjVNlaxnuE=/?moveToWidget=3458764581758623044), que contém todos os caminhos, decisões, mensagens e conexões.

## Escopo funcional e oportunidades observadas

- **Discovery:** análise dos canais digitais, possíveis falhas de direcionamento, horários e continuidade do atendimento.
- **Jornada do usuário:** diferenciação entre segurado e não segurado, instruções do WhatsApp e orientação ao portal e e-commerce.
- **Regras de negócio:** até duas tentativas para opção inválida e encerramento com mensagem após a segunda falha.
- **Transbordo:** disponibilização da opção de atendimento humano, conforme a jornada modelada.
- **Backlog / MVP:** estudo de opções de Assistência Dia e Noite, Seguradoras, Oficina e retorno ao menu, com detalhamento de algumas ramificações no Miro.
- **POCs:** referências de telas e demonstração vinculadas ao quadro original.

O quadro contém **cenários denominados “Sou segurado” e “Sou cliente” em documentos diferentes**. Mantive ambos como registrados na fonte, em vez de presumir que são equivalentes.

## Vídeo e evidências do projeto

**POC 01 — demonstração mantida:**

https://youtu.be/u4LxF7WXEUY

**Quadro completo, com todos os fluxos, telas, prints, canvas e POCs — endereço oficial:**  
https://miro.com/app/board/uXjVNlaxnuE=/

**Imagem original também mantida no material anterior:**

![Imagem original do README](https://github.com/BertaT2C/Projeto_Miro_CanaisDigitais/assets/99225701/6f24e789-c788-4b21-8fab-bcef793fd9ea)

## Meu papel e competências demonstradas

**Business Analysis | Discovery | Jornada do Usuário | AS IS / TO BE | Mapeamento de Processos | Requisitos Funcionais | BDD | Critérios de Aceite | Backlog | MVP | Stakeholder Management | Miro | Canais Digitais | Chatbots | WhatsApp**

Esse case demonstra como a **análise da operação, o mapeamento visual e a escrita de regras e cenários** ajudam a estruturar decisões de produto e melhorias na experiência de atendimento.

## Arquivos de referência e preservação

- [Case detalhado Maxpar / Autoglass](./docs/CASE_MAXPAR_AUTOGLASS.md)
- [Jornada completa extraída do Miro — etapas, conexões e mensagens](./docs/FLUXO_MIRO_JORNADA_COMPLETA.md)
- [Estudo de backlog completo extraído do Miro — etapas, conexões e mensagens](./docs/FLUXO_MIRO_BACKLOG_COMPLETO.md)
- [Cenários e regras transcritos do Miro sem mudar seu conteúdo](./docs/CENARIOS_E_REGRAS_ORIGINAIS.md)
- [README original, preservado integralmente](./DOCUMENTACAO_ORIGINAL.md)
- [Mapeamento AS IS original](./Mapeamento%20As%20is_detalhe.png)

> **Transparência do portfólio:** não foram inventados indicadores, resultados financeiros, percentuais, datas de implantação ou integrações. **Os dois fluxos textuais foram transcritos com suas conexões para o GitHub**, enquanto o quadro Miro continua sendo a referência visual original para layout, prints, canvas e POCs. Nenhum conteúdo foi editado no Miro.
