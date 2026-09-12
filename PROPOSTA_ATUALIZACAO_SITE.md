# Proposta de atualização — site Transistir

**Data da análise:** 12 de setembro de 2026  
**Escopo:** vitrine pública em `transistir.github.io`, comparada aos materiais de trabalho em `Nextcloud/transistir`.

## Diagnóstico

O site atual é uma página estática com manifesto e quatro cartões de projetos:

1. CadeiaDominial;
2. Kutary;
3. IA Local Audio;
4. TerraLab v2.

Os cartões levam apenas a repositórios no GitHub. As descrições são curtas e não mostram o estágio, a finalidade pública, parceiros, entregas recentes ou a abordagem da Transistir. O último commit do site é de março de 2026, enquanto o Nextcloud registra atividades e entregas até setembro de 2026.

Há também um descompasso de nome e contexto: o trabalho da COIAB passa a ser apresentado como **COIAB-App**, substituindo as referências anteriores a Kutary/Ekanãdyby. O aplicativo se baseia no CoMapeo e é desenvolvido em parceria com a Awana Digital. O sistema de cadeia dominial passou a ser referido como **Umbelino** na proposta de Fase 3.

## O que está desatualizado ou ausente

| Frente | Como aparece hoje | O que os materiais recentes mostram | Atualização recomendada |
| --- | --- | --- | --- |
| Umbelino / CadeiaDominial | Uma linha: “Ferramenta para análise de cadeias dominiais”. | Fase 2 em execução para análise fundiária em Terras Indígenas; entregas de interface e desenvolvimento funcional; proposta de Fase 3 com IA auto-hospedada, OCR e importação assistida. | Atualizar o cartão, mencionar análise fundiária e rastreabilidade; criar estudo de caso. Só anunciar Fase 3 como “em proposta”, nunca como entregue. |
| COIAB-App / Kutary | “Aplicação completa com frontend e backend”. | Projeto em execução para um app móvel de coleta de dados territoriais indígenas, baseado no CoMapeo e realizado em parceria com a Awana Digital; prevê customização, testes de campo e formação. | Renomear o cartão para “COIAB-App”; trocar linguagem técnica genérica por finalidade, parceria e princípios local-first/offline. |
| TerraLab / IEB | Descrição longa, mas fixa e focada somente no GeoNode. | Consultoria para monitoramento do projeto Danida: formulário e indicadores concluídos (P2), recomendação validada de estações modulares e abertas (P5), e continuidade prevista em dashboard, integração e acesso. | Reescrever o cartão e criar página de caso com resultados, sem expor dados, infraestrutura ou detalhes internos do IEB. |
| Prática da Transistir | Manifesto e projetos, sem uma síntese dos serviços. | As três frentes mostram competências recorrentes: software territorial, dados e visualização, tecnologias apropriadas, co-design, sistemas locais e IA sob controle institucional. | Incluir uma seção “Como trabalhamos” e uma página/contato para novos projetos. |
| Presença institucional | Não há contato, links institucionais, metadescrição nem atualização visível. | O site não oferece próximo passo para quem quer contratar, colaborar ou conhecer o trabalho. | Adicionar contato institucional aprovado, GitHub e/ou rede social, metadescrição, imagem de compartilhamento e ano/atualização no rodapé. |

## Conteúdo público proposto

### Chamada principal

> Tecnologia social para territórios, dados e autonomia.

> Desenvolvemos ferramentas digitais e infraestruturas apropriadas junto a organizações e comunidades: do monitoramento territorial à análise fundiária, de dados geoespaciais a sistemas locais e abertos.

Essa chamada aproxima a página inicial do manifesto, mas explica de forma imediata o que a Transistir faz.

### Seção “Como trabalhamos”

Usar quatro princípios curtos, extraídos de padrões presentes nos projetos:

- **Cocriação:** tecnologia desenhada com quem a utiliza e sustenta no território.
- **Autonomia:** prioridade para soluções abertas, documentadas, reparáveis e sem dependências desnecessárias.
- **Cuidado com os dados:** segurança, rastreabilidade e controle institucional, sobretudo em dados territoriais sensíveis.
- **Continuidade:** entregamos software, formação e documentação para que o trabalho permaneça vivo após o projeto.

### Cartões de projetos — texto inicial

#### Umbelino — análise de cadeias dominiais

Sistema web para apoiar a análise fundiária de imóveis sobrepostos a Terras Indígenas. Organiza registros, documentos e relações dominiais para dar mais rastreabilidade à investigação territorial.

**Situação sugerida:** Em evolução  
**Link:** repositório atual, caso seja público e representativo. Caso não seja, trocar por “Conheça o projeto” em uma página interna.

**Observação editorial:** a Fase 3 de OCR e IA deve ser apresentada apenas como proposta/em planejamento, condicionada à autorização da contratante.

#### COIAB-App — monitoramento territorial indígena

Aplicativo móvel para coleta e organização de dados de monitoramento territorial indígena. Desenvolvido pela COIAB em parceria com a Awana Digital, o COIAB-App se baseia no CoMapeo e prioriza tecnologias locais, colaborativas e aptas a funcionar em contextos de conectividade limitada.

**Situação sugerida:** Em desenvolvimento  
**Link:** somente para o repositório público aprovado. O atual `Kutary_app` não corresponde ao conjunto de repositórios baseado em CoMapeo usado na fase atual; não apontar para ele sem validação.

**Observação editorial:** obter autorização da COIAB e da Awana Digital para usar marcas, telas, nomes institucionais e a descrição da parceria.

#### TerraLab — monitoramento socioambiental

Evolução do ambiente TerraLab/GeoNode para organizar indicadores, atividades e evidências de iniciativas socioambientais. O trabalho inclui formulários com validação e rastreabilidade, visualização de dados e desenho de tecnologias abertas para monitoramento em campo.

**Situação sugerida:** Em evolução  
**Link:** repositório público aprovado ou página de estudo de caso.

**Resultado que pode ser comunicado:** recomendação técnica de estações meteorológicas e de qualidade do ar modulares, abertas, documentadas e de manutenção acessível — sem divulgar localizações, arquitetura operacional ou dados do IEB.

#### IA Local Audio

Manter o cartão, mas revisar sua descrição e disponibilidade: não há material recente correspondente na pasta analisada. Confirmar se o repositório está ativo, demonstrável e adequado à vitrine. Se não estiver, mover para “Experimentos” ou retirar temporariamente.

## Arquitetura recomendada para o site

Sem necessidade de trocar a tecnologia nesta primeira atualização:

```text
Início
├── O que fazemos / Como trabalhamos
├── Projetos
│   ├── Umbelino
│   ├── COIAB-App
│   ├── TerraLab
│   └── IA Local Audio ou Experimentos
├── Manifesto
└── Contato
```

Cada projeto principal deve ganhar uma página interna curta, com: contexto, desafio, abordagem, resultados/etapa atual, parceiros (quando autorizados), tecnologias e link público. Isso evita que a página inicial exponha detalhes de contratos, prazos ou materiais sensíveis.

## Plano de implementação

### Etapa 1 — atualização essencial

1. Reescrever a abertura e os três cartões prioritários.
2. Renomear Kutary para COIAB-App e atualizar a descrição com a parceria COIAB–Awana Digital e a base CoMapeo.
3. Adicionar status textual (“Em desenvolvimento”, “Em evolução” ou “Concluído”) e mês/ano da atualização.
4. Incluir contato e metadados básicos para busca e compartilhamento.
5. Revisar links do GitHub: manter somente repositórios públicos, ativos e representativos.

### Etapa 2 — portfólio com contexto

1. Criar três páginas de estudo de caso, uma para cada frente prioritária.
2. Produzir 1–3 imagens aprovadas por projeto: telas sem dados sensíveis, diagrama ou fotografia autorizada.
3. Publicar versões em português e inglês; a tradução precisa ser editorial, não apenas literal.
4. Adicionar uma seção compacta de serviços/capacidades.

### Etapa 3 — manutenção

1. Separar os dados dos projetos do HTML em um arquivo simples, para facilitar atualizações.
2. Definir revisão trimestral e, por projeto, um responsável por confirmar texto, status, link e imagem.
3. Registrar no rodapé a data da última atualização pública.

## Decisões e autorizações necessárias antes de publicar

- Confirmação da COIAB e da Awana Digital sobre a forma pública de citar a parceria, as marcas e as imagens do **COIAB-App**.
- Autorização do IEB e da UFPA/FADESP/Ministério dos Povos Indígenas para citar projetos, parceiros e resultados.
- Definição dos repositórios públicos corretos para Umbelino, COIAB-App e TerraLab.
- Escolha de canal de contato institucional a publicar.
- Confirmação sobre a permanência de **IA Local Audio** como projeto ativo do portfólio.

## Critério de sucesso

Ao fim da atualização, uma pessoa que chegue ao site deve entender em menos de um minuto: o que a Transistir faz, quais são suas três frentes mais relevantes, em que estágio cada uma está e como iniciar uma conversa — sem expor informações contratuais, pessoais ou territoriais sensíveis.
